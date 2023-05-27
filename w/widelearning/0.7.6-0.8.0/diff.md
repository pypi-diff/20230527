# Comparing `tmp/widelearning-0.7.6.tar.gz` & `tmp/widelearning-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "widelearning-0.7.6.tar", max compression
+gzip compressed data, was "widelearning-0.8.0.tar", max compression
```

## Comparing `widelearning-0.7.6.tar` & `widelearning-0.8.0.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0      354 2023-05-11 16:39:33.911395 widelearning-0.7.6/pyproject.toml
--rw-r--r--   0        0        0    78951 2023-05-11 16:37:44.468704 widelearning-0.7.6/widelearning.py
--rw-r--r--   0        0        0      505 2023-05-11 16:39:42.287555 widelearning-0.7.6/setup.py
--rw-r--r--   0        0        0      514 2023-05-11 16:39:42.287791 widelearning-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1979 2023-05-27 13:49:07.193982 widelearning-0.8.0/README.md
+-rw-r--r--   0        0        0      402 2023-05-27 13:50:22.159447 widelearning-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    84277 2023-05-27 13:42:51.958454 widelearning-0.8.0/widelearning.py
+-rw-r--r--   0        0        0     2502 2023-05-27 13:50:44.568480 widelearning-0.8.0/setup.py
+-rw-r--r--   0        0        0     2606 2023-05-27 13:50:44.568858 widelearning-0.8.0/PKG-INFO
```

### Comparing `widelearning-0.7.6/widelearning.py` & `widelearning-0.8.0/widelearning.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pandas as pd
 import os
 import shutil
 import glob
 import math as m
 import requests
 
+# 1.  
 def txt_kernel(file_path):	
     f = open(file_path, 'r')
 	
     weights = []
 
     for i in f:
         weights.append(i.strip().split(','))
@@ -23,14 +24,15 @@
             ii[i1] = [[int(elem)]]
             
     with open('kernel.txt', 'w') as file:
         file.write(str(weights))
 
     return weights 
 
+# 2.
 def add_kernel(path, init_kernel):
     ff = open(path, 'r')
     
     w1 = init_kernel
 
     weights = []
 
@@ -48,43 +50,46 @@
         for j in range(len(w1)):
             w1[i][j][0].append(weights[i][j])
 
     with open('kernel.txt', 'w') as file:
         file.write(str(w1))
         
     return w1
-    
+
+# 3.    
 # horizontal(32, [-7,-5,-3,-1,1,3,5,7])
 def horizontal(dim, values):
     horizontal = []
     for i in range(dim):
         row = []
         for j in range(dim):
             row.append(values[i % len(values)])
         horizontal.append(row)
         
     with open('horizontal.txt', 'w') as f:
         for row in horizontal:
             f.write(','.join(str(x) for x in row) + ',\n')
     return horizontal
 
+# 4.
 # vertical(32, [-7,-5,-3,-1,1,3,5,7])	
 def vertical(dim, values):
     vertical = []
     for i in range(dim):
         row = []
         for j in range(dim):
             row.append(values[j % len(values)])
         vertical.append(row)
         
     with open('vertical.txt', 'w') as f:    
         for row in vertical:
             f.write(','.join(str(x) for x in row) + ',\n')
     return vertical
 
+# 5.
 # diagonal([-7, -5, -3, -1], [1, 3, 5, 7], 1, 32)	
 def diagonal(up, down, d, dimension):
 
     matrix = [[0 for i in range(dimension)] for j in range(dimension)] 
     for i in range(dimension):
         for j in range(dimension):
             if i == j: 
@@ -105,29 +110,31 @@
     with open('diagonal2.txt', 'w') as file:
         for i in matrix2:
             for j in i:
                 file.write(str(j) + ',')
             file.write('\n')
     
     return matrix
-    
+
+# 6.     
 def show_kernel(N, name):
 
     ff = name.layers[N].get_weights()
 
     for nn in range(len(ff[0][0][0][0])):
       print('\n' + f'Номер сверточного ядра: {nn}')
       for kk in range(len(ff[0][0][0])):
         print(f'-----------ЦВЕТОВОЙ КАНАЛ №{kk}-----------')
         for i in range(len(ff[0])):
           for j in range(len(ff[0][i])):
             print(ff[0][i][j][kk][nn], end=',')
           print()
         print('\n')
-        
+
+# 7.        
 def txt_kernel_rgb(k1, k2, k3): 
 
     f1 = open(k1, 'r')
     f2 = open(k2, 'r')
     f3 = open(k3, 'r')
 	
     w1 = []
@@ -173,14 +180,15 @@
         for j in range(len(w1[0])):
             w1[i][j].append(w3[i][j])
 			
     return w1
 
 #w1 = txt_kernel_rgb('k1.txt', 'k2.txt', 'k3.txt')
 
+# 8. 
 def add_kernel_rgb(k1, k2, k3, w):
 
     f1 = open(k1, 'r')
     f2 = open(k2, 'r')
     f3 = open(k3, 'r')
 	
     w11 = []
@@ -231,15 +239,15 @@
         for j in range(len(w1)):
             w[i][j][2].append(w33[i][j])
 	########################################
 	
     return w
 
 #w2 = add_kernel_rgb('k3.txt', 'k2.txt', 'k1.txt', weights1)
-        
+# 9.       
 def select_top(path, label):
     # label - название столбца с метками классов ('Wine')
     # z - индекс в переборе меток классов
     all_classes = pd.read_csv(path)#('wine_train.csv')
     all_classes.drop(all_classes.columns[0], axis=1, inplace=True)
 
     uniq = pd.unique(all_classes[[label]].values.ravel('K'))
@@ -1208,14 +1216,15 @@
             weights[zz]+=step  
         
             print()
             
     print(weights_all)
     return weights_all
 
+# 10.  
 def select_top_binary(path, label):
     all_classes_main = pd.read_csv(path)
     all_classes_main.drop(all_classes_main.columns[0], axis=1, inplace=True)
     
     uniq = pd.unique(all_classes_main[[label]].values.ravel('K'))
     uniq = list(uniq)
     
@@ -1361,23 +1370,25 @@
         print('OTHER - ', other) 
         print('СУММА отсеченных сверху и снизу = ', sum_up_down)
         print(weights)
         print('DISTANCE = ', distance)
         print('+++++++++++++++++++++++++++++++++++++++')
         print()      
 
-def grad_boost_binary(path, t, oth, l, s, from_initial, weights_main):
+# 11.
+def grad_binary(path, t, oth, l, s, weights_main):
     #path = 'trainW07_1.csv'
     #t = ['low']
     #oth = ['middle']
     #l = 'UNS'
     #s = 1
     #from_initial = 1
     #weights_main = [-663.0, -8850.0, -610.0, -16520.0, -1202.0] 
-    
+    from_initial = 1
+
     for zz_i in range(len(weights_main)):
         zz = zz_i
         step = s
         label = l
         top = t
         other = oth
         
@@ -1796,20 +1807,21 @@
                 break
                 
                 
             weights[zz]+=step  
  
                 
 # grad("trainW08_4.csv", ['very_low'], ['high', 'low', 'middle'], 'UNS', [-837.2851063829785, 1654.2510638297872, -485.82978723404267, 1729.021276595745, 19057.587234042556])
-def grad(path, t, oth, l, weights):
+# 12. 
+def grad(path, t, oth, l, s, weights):
     #path = "trainW08_4.csv"#"kahraman_train.csv"
     #t = ['high']#['very_low']
     #oth = ['very_low', 'low', 'middle']#['high', 'low', 'middle']
     #l = 'UNS'
-    s = 1
+    #s = 1
 
     #weights = [-837.2851063829785, 1654.2510638297872, -485.82978723404267, 1729.021276595745, 19057.587234042556]
     #[-4745.458204334365, -5586.578947368422, -5510.185758513931, -8949.30959752322, -18447.66253869969]
 
     weights_all = grad_boost(path, t, oth, l, s, 1, weights)
 
     with open('weights_all==0.txt', 'w') as file:
@@ -1902,14 +1914,15 @@
             file.write(str(weights) + '\nUP = ' + str(up_main) + '\nDOWN = ' + str(down_main) + '\nDistance = ' + str(distance_main))
 
         print('++++++++++++++++++++++++++++++++++++++')
         print()
         ii += 1    
 
 # data_int('forest.csv', 'dec_forest.txt', 'forest')           
+# 13. 
 def data_int(path, decimal, name):
     data = pd.read_csv(path) 
 
     decimal_places = open(decimal, 'r')
 
     dec = []
 
@@ -1973,55 +1986,69 @@
         lstm.append(i)
     
     data_train = data.drop(labels = lstm,axis = 0)
     data_train.to_csv(f'{name}_train.csv')
     
     return data
 
-def generate_fa(data_folder, weights_folder, label):
-
+# 14. 
+# scale_weights('UNS', 'data/', 'weights/')
+def scale_weights(label, data_folder, weights_folder):
+    
+    os.mkdir('scale')
+    os.mkdir('result')
+    os.mkdir('all_weights')
+    
     w = []
 
     # Сортируем список файлов в папке по алфавиту
     files1 = sorted(os.listdir(weights_folder))
     files2 = sorted(os.listdir(data_folder))
 
     for i in range(1, len(files1)+1):
         filename = f"w_{i}.txt"
 
+    #for file_name in files1:#os.listdir(weights_folder):
+    #    if file_name.endswith('.txt'):
         file_path = os.path.join(weights_folder, filename)
+            #print()
         with open(file_path, 'r') as file:
             lines = file.readlines()
             w.append(lines[0])           
+                
+    #print(w)
 
     weights = []
 
     for i in range(len(w)):
         string = w[i].replace("'", "").replace("\n", "")
         string1 = string.split(',')
 
-    ww = []
+        ww = []
+
+        for j in range(len(string1)):
+            z = string1[j].replace("'", "").replace("\n", "").replace("[", "").replace("]", "")
+            ww.append(float(z))
 
-    for j in range(len(string1)):
-        z = string1[j].replace("'", "").replace("\n", "").replace("[", "").replace("]", "")
-        ww.append(float(z))
+        weights.append(ww)
 
-    weights.append(ww)
+    ##print(weights)
 
     ii = 0
 
     for i1 in range(1, len(files2)+1):
         filename = f"train_{i1}.csv"
         file_path = os.path.join(data_folder, filename)
         data = pd.read_csv(file_path)
 
         print('I = ', ii)
             
         # Рабочий ход
         data['Scalar_calc'] = ""
+        #data['Scaled_prod'] = ""
         cl = data.columns
         columns = []
         for j in range(2, len(cl)):
             if(cl[j]=='N'):
                 break
             else:
                 columns.append(cl[j])
@@ -2034,14 +2061,15 @@
             for j in range(2, len(cl)):
                 if(cl[j]=='N'):
                     break
                 else:
                     columns.append(cl[j])
                         
         print(columns)
+        #print()
             
         for i in range(len(data)):
             xx = data.iloc[i]
             x = []
             for u in range(len(columns)):
                 x.append(xx[columns[u]])
             f = np.array(weights[ii])
@@ -2049,17 +2077,19 @@
             scalar = np.dot(f, g)
             data['Scalar_calc'][i]=scalar
         data = data.sort_values(by='Scalar_calc', ascending=False)
         data.to_csv('data.csv')
         data = pd.read_csv('data.csv')
         data.drop(data.columns[0], axis=1, inplace=True)
         firstindex = data[label][0]
+        #f'firstindex{ii}' = data[label][0]
         print(data.head())
         print('LENGTH_data = ', len(data))
-        print('LABEL = ', firstindex)#
+        print('LABEL = ', firstindex)#data[label][0])#f'firstindex{ii}')
+        #print('++++++++++++++++++++++++++++\n')
             
         up = 0
         for i1 in range(len(data)):
             if(data[label][i1]==firstindex):
                 up += 1
             else:
                 break
@@ -2074,54 +2104,104 @@
                 down += 1
             else:
                 break
                     
         data_down = data.sort_values(by='Scalar_calc')
         data_down.to_csv('down.csv')
         data_down = pd.read_csv('down.csv')
- 
+            
+        #for l in range(down):
+        #    d_down = data_down['Scalar_calc'][l]
+            
         print('UP = ', up)
         print('DOWN = ', down)
             
         if(len(data) == (up + down)):
             u1 = data['Scalar_calc'][up-1]
             u2 = data_down['Scalar_calc'][down-1]
         else:
             u1 = (data['Scalar_calc'][up]+data['Scalar_calc'][up-1])/2
             u2 = (data_down['Scalar_calc'][down]+data_down['Scalar_calc'][down-1])/2
         print(u1)
         print(u2)
-
+        
+        #os.mkdir('scale')
+        #os.mkdir('result')
+            
+        #print(weights[ii])
+        #scale = []
         scaled_w = []
         for k in range(len(weights[ii])):
             w1 = 2*weights[ii][k]/(u1 - u2)
             scaled_w.append(w1)
         w2 = -2*u2/(u1-u2)-1
         scaled_w.append(w2)
+            #scale.append(scaled_w)
         print(scaled_w)
             
         with open(f'scale/sw_{ii}.txt', 'w') as ff:
             ff.write(str(scaled_w))
             
         data.drop(data.columns[0], axis=1, inplace=True)
                 
         data.to_csv(f'result/data_res_{ii}.csv')
             
         print('++++++++++++++++++++++++++++\n')
             
         
         ii += 1
+        
+    ######################################
+    scale = 'scale'
+    w = []
 
-    ##########################################
+    files1 = sorted(os.listdir(scale))
 
-    label = 'target'
+    for i in range(len(files1)):
+        filename = f"sw_{i}.txt"
+        file_path = os.path.join(scale, filename)
+        with open(file_path, 'r') as file:
+            lines = file.readlines()
+            w.append(lines[0]) 
+    
+        weights = []
+
+    for i in range(len(w)):
+        string = w[i].replace("'", "").replace("\n", "")
+        string1 = string.split(',')
+
+        ww = []
+
+        for j in range(len(string1)):
+            z = string1[j].replace("'", "").replace("\n", "").replace("[", "").replace("]", "")
+            ww.append(float(z))
 
-    data_folder = 'result/'
+        weights.append(ww)
+        
+    formatted_data = []
+    for row in weights:
+        formatted_row = [str(element) + ',' for element in row]
+        formatted_data.append(formatted_row)
+
+    result = '\n'.join([', '.join(row) for row in formatted_data])
+
+    with open("all_weights/weights.txt", "w") as file:
+        file.write(result)
 
-    weights_folder = 'scale/'
+    with open("all_weights/weights.txt", "r") as f:
+        content = f.read().replace(',,', ',')
+
+    with open("all_weights/weights.txt", "w") as f:
+        f.write(content)
+    
+    return scaled_w
+
+# 15.
+# generate_fa('UNS', 'result', 'scale')
+def generate_fa(label, data_folder, weights_folder):
 
     w = []
 
     files1 = sorted(os.listdir(weights_folder))
     files2 = sorted(os.listdir(data_folder))
 
     for i in range(0, len(files1)):
@@ -2133,21 +2213,21 @@
 
     weights = []
 
     for i in range(len(w)):
         string = w[i].replace("'", "").replace("\n", "")
         string1 = string.split(',')
 
-    ww = []
+        ww = []
 
-    for j in range(len(string1)):
-        z = string1[j].replace("'", "").replace("\n", "").replace("[", "").replace("]", "")
-        ww.append(float(z))
+        for j in range(len(string1)):
+            z = string1[j].replace("'", "").replace("\n", "").replace("[", "").replace("]", "")
+            ww.append(float(z))
 
-    weights.append(ww)
+        weights.append(ww)
 
     print('        for n in range(len(data)):')
 
     ii = 0
 
     for i1 in range(0, len(files2)):
         filename = f"data_res_{i1}.csv"
@@ -2174,15 +2254,15 @@
             #############
             f = np.array(weights[ii])
             g = np.array(x)
             scalar = np.dot(f, g)
             data['Scaled_prod'][i]=scalar
             
         firstindex = data[label][0]
-
+            
         up = 0
         for i1 in range(len(data)):
             if(data[label][i1]==firstindex):
                 up += 1
             else:
                 break
                     
@@ -2196,129 +2276,152 @@
                 down += 1
             else:
                 break
                     
         data_down = data.sort_values(by='Scalar_calc')
         data_down.to_csv('down.csv')
         data_down = pd.read_csv('down.csv')
-    
+            
         t_up = data['Scaled_prod'][up-1]
         t_down = data_down['Scaled_prod'][down-1]
-
+            
         if(ii == 0):
-            if(t_up >= 1):
-                print(f'            if(data["SC{ii}"][n]>=1):\n                data["FA"][n]={firstindex}')
-            if(t_down <= -1):
-                print(f'            elif(data["SC{ii}"][n]<=-1):\n                data["FA"][n]={lastindex}')
-        else:
-            if(t_up >= 1):
-                print(f'            elif(data["SC{ii}"][n]>=1):\n                data["FA"][n]={firstindex}')
-            if(t_down <= -1):
-                print(f'            elif(data["SC{ii}"][n]<=-1):\n                data["FA"][n]={lastindex}')
+            if(round(t_up) >= 1):
+                print(f'            if(data["SC{ii}"][n]>=1):\n                data["FA"][n]="{firstindex}"')
+            if(round(t_down) <= -1):
+                print(f'            elif(data["SC{ii}"][n]<=-1):\n                data["FA"][n]="{lastindex}"')
+        else:
+            if(round(t_up) >= 1):
+                print(f'            elif(data["SC{ii}"][n]>=1):\n                data["FA"][n]="{firstindex}"')
+            if(round(t_down) <= -1):
+                print(f'            elif(data["SC{ii}"][n]<=-1):\n                data["FA"][n]="{lastindex}"')
             
                 
         ii += 1
 
-    return scaled_w
-
-def check_fa(data_folder, weights_folder, label):
-
-    label = 'target'
-
-    data_folder = 'test/'
-
-    weights_folder = 'scale/'
-
-    w = []
-
-    files1 = sorted(os.listdir(weights_folder))
-
-    for i in range(0, len(files1)):
-        filename = f"sw_{i}.txt"
-        file_path = os.path.join(weights_folder, filename)
-        with open(file_path, 'r') as file:
-            lines = file.readlines()
-            w.append(lines[0])           
+# 16. 
+# check_test('train_1.csv', 'weights.txt', 'KAHRAMAN_test.csv', 'UNS')
+def check_test(train, weights, test, label):
+    def getNameColumn(nameFileTrain):
+        with open(nameFileTrain, encoding='utf-8') as r_file:
+            # Создаем объект DictReader, указываем символ-разделитель ','
+            file_reader = csv.DictReader(r_file, delimiter = ',')
+            nameColumn  = list(file_reader.fieldnames)  #названия столбцов
+        r_file.close()
+        del nameColumn[-1]
+        del nameColumn[:2]
+        return nameColumn
+    def getCountNeuronSizeVector(nameFileTrain):
+        with open(nameFileTrain, encoding='utf-8') as r_file:
+            # Создаем объект DictReader, указываем символ-разделитель ','
+            file_reader = csv.DictReader(r_file, delimiter=',')
+            nameColumn  = list(file_reader.fieldnames)  #названия столбцов
+            sizeVector = len(nameColumn) - 1          #количество столбцов
+            countNeurons = 1
+            for row in file_reader:
+                countNeurons += 1
+        r_file.close()
+        return countNeurons, sizeVector
+    def initializingDictionaryKeys():
+        iNeuron = 1                             #инициализация
+        while iNeuron <= countNeurons:          #ключей
+            rulesLogicalInference[iNeuron] = 0  #для
+            rulesLogicalInference[-iNeuron] = 0 #правила
+            iNeuron += 1                        #логического
+        rulesLogicalInference[iNeuron * 10] = 0 #вывода
+    def initializationDictionaryValues(nameFileTrain):
+        with open(nameFileTrain, encoding='utf-8') as r_file:
+            # Создаем объект DictReader, указываем символ-разделитель ','
+            file_reader = csv.DictReader(r_file, delimiter=',')
+            nameCol = list(file_reader.fieldnames)  # названия столбцов
+            for row in file_reader:
+                iVector = 0
+                for iColumn in nameColumn:  # чтение вектора входов из обучающей выборки
+                    qq = row[iColumn]
+                    vectorArgs[iVector] = qq
+                    iVector += 1
+                vectorArgs[iVector] = 1.  # инициализация смещения единицей
+                ww = 0.0
+                iNeuron = 0
+                while iNeuron < countNeurons:               #присвоение
+                    ww = np.dot(vectorArgs, matrixWeights[iNeuron])
+                    if (ww < -1.) or (ww > 1.):             #значений
+                        ww /= abs(ww)                       #соответствующих
+                        ww *= (iNeuron + 1)                 #ключам
+                        break                               #логического
+                    iNeuron += 1                            #
+                else:                                       #
+                    ww = (countNeurons + 1) * 10            #
+                rulesLogicalInference[ww] = row[nameClass]  #вывода
+        r_file.close()
+
+    #НАЧАЛО ПРОГРАММЫ
+    nameFileTrain = train
+    nameFileWeights = weights
+    nameFileTest = test
+    nameClass = label
+    neuronsVectors = getCountNeuronSizeVector(nameFileWeights)
+    countNeurons = neuronsVectors[0]
+    sizeVector = neuronsVectors[1]
+    vectorArgs = np.zeros(sizeVector, dtype=np.float64)
+    matrixWeights = np.loadtxt(nameFileWeights, delimiter=',', dtype=np.float64, usecols=range(sizeVector))
+    nameColumn = getNameColumn(nameFileTrain)
+    rulesLogicalInference = {}
+    initializingDictionaryKeys()
+    initializationDictionaryValues(nameFileTrain)
+    
+    ####
+    zz = []
+    ####
+    with open(nameFileTest, encoding='utf-8') as r_file:
+        # Создаем объект DictReader, указываем символ-разделитель ','
+        file_reader = csv.DictReader(r_file, delimiter=',')
+        nameCol = list(file_reader.fieldnames)  # названия столбцов
+        for row in file_reader:
+            iVector = 0
+            for iColumn in nameColumn:  # чтение вектора входов из тестовой выборки
+                qq = row[iColumn]
+                vectorArgs[iVector] = qq
+                iVector += 1
+            vectorArgs[iVector] = 1.  # инициализация смещения единицей
+            ww = 0.0
+            iNeuron = 0
+            while iNeuron < countNeurons:  # присвоение
+                ww = np.dot(vectorArgs, matrixWeights[iNeuron])
+                if (ww < -1.) or (ww > 1.):  # значений
+                    ww /= abs(ww)  # соответствующих
+                    ww *= (iNeuron + 1)  # ключам
+                    break  # логического
+                iNeuron += 1  # вывода
+            else:  #
+                ww = (countNeurons + 1) * 10  #
+            if rulesLogicalInference[ww] != row[nameClass]:
+                #print(row[''])
+                zz.append(row[''])
+    
+    sizeVector += 1
+    
+    with open(test,"r", encoding='UTF8') as f:
+        reader = csv.reader(f)
+        data = list(reader)
+        row_count = len(data) - 1
+    #print(row_count)
+    
+    print('Ошибок = ', len(zz), 'из ', row_count)
+    print('Экземпляры №:', zz)
+
+# 17.
+# count_conv_operations(28, 28, 1, 14, 7, 4)
+def count_conv_operations(height, width, color_channels, kernel_size, stride, num_kernels):
+    output_height = int((height - kernel_size) / stride) + 1
+    output_width = int((width - kernel_size) / stride) + 1
+    num_operations = (output_height * output_width * kernel_size * kernel_size * num_kernels * 2)*color_channels
+    
+    no_bias = (num_operations - ((kernel_size**2)*num_kernels))*color_channels
+    print('Кол-во вычислительных операций = ', num_operations)  
+    print('Кол-во вычислительных операций (no_bias) = ', no_bias)
 
-    weights = []
 
-    for i in range(len(w)):
-        string = w[i].replace("'", "").replace("\n", "")
-        string1 = string.split(',')
 
-    ww = []
 
-    for j in range(len(string1)):
-        z = string1[j].replace("'", "").replace("\n", "").replace("[", "").replace("]", "")
-        ww.append(float(z))
-
-    weights.append(ww)
-
-    for file_name in os.listdir(data_folder):
-        if file_name.endswith('.csv'):
-            file_path = os.path.join(data_folder, file_name)
-            data = pd.read_csv(file_path)
-            
-            
-            
-            for k1 in range(len(weights)):
-                data[f'SC{k1}'] = ""
-            
-                cl = data.columns
-                columns = []
-                for j in range(2, len(cl)):
-                    if(cl[j]=='N'):
-                        break
-                    else:
-                        columns.append(cl[j])
-
-                for i in range(len(data)):
-                    xx = data.iloc[i]
-                    x = []
-                    for u in range(len(columns)):
-                        x.append(xx[columns[u]])
-                    #############
-                    x.append(1)
-                    #############
-                    f = np.array(weights[k1])
-                    g = np.array(x)
-                    scalar = np.dot(f, g)
-                    data[f'SC{k1}'][i]=scalar
-            
-            data['FA']=""
-
-    # Место для вставки сгенерированного кода
-            
-            for n in range(len(data)):
-                if(data["SC0"][n]>=1):
-                    data["FA"][n]=1
-                elif(data["SC0"][n]<=-1):
-                    data["FA"][n]=0
-                elif(data["SC1"][n]>=1):
-                    data["FA"][n]=2
-                elif(data["SC1"][n]<=-1):
-                    data["FA"][n]=0
-                elif(data["SC2"][n]>=1):
-                    data["FA"][n]=0
-                elif(data["SC2"][n]<=-1):
-                    data["FA"][n]=1
-            
-    ########################################
-            
-            mistakes = []
-            data['check']=""
-            for n1 in range(len(data)):
-                if((data['target'][n1]==data['FA'][n1])==True):
-                    data['check'][n1]=0
-                else:
-                    data['check'][n1]=1
-                    mistakes.append(data['N'][n1])
-            
-            data.to_csv('final/data_test.csv')
-            print(data.head())
-            print('+++++++++++++++++++')
-            print('Ошибок: ', data['check'].sum(), '/', len(data))
-            print(mistakes)
-
-    return data
```

