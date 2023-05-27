# Comparing `tmp/vector_vault-1.1.3.tar.gz` & `tmp/vector_vault-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_vault-1.1.3.tar", last modified: Thu May 25 06:27:28 2023, max compression
+gzip compressed data, was "vector_vault-1.2.0.tar", last modified: Sat May 27 01:28:34 2023, max compression
```

## Comparing `vector_vault-1.1.3.tar` & `vector_vault-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-25 06:27:28.750527 vector_vault-1.1.3/
--rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.1.3/LICENSE
--rw-r--r--   0 johnrood   (501) staff       (20)    15810 2023-05-25 06:27:28.750357 vector_vault-1.1.3/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)    15085 2023-05-25 06:25:59.000000 vector_vault-1.1.3/README.md
--rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-25 06:27:28.750567 vector_vault-1.1.3/setup.cfg
--rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-25 06:27:05.000000 vector_vault-1.1.3/setup.py
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-25 06:27:28.747103 vector_vault-1.1.3/vector_vault.egg-info/
--rw-r--r--   0 johnrood   (501) staff       (20)    15810 2023-05-25 06:27:28.000000 vector_vault-1.1.3/vector_vault.egg-info/PKG-INFO
--rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-25 06:27:28.000000 vector_vault-1.1.3/vector_vault.egg-info/SOURCES.txt
--rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-25 06:27:28.000000 vector_vault-1.1.3/vector_vault.egg-info/dependency_links.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-25 06:27:28.000000 vector_vault-1.1.3/vector_vault.egg-info/requires.txt
--rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-25 06:27:28.000000 vector_vault-1.1.3/vector_vault.egg-info/top_level.txt
-drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-25 06:27:28.750013 vector_vault-1.1.3/vectorvault/
--rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.1.3/vectorvault/__init__.py
--rw-r--r--   0 johnrood   (501) staff       (20)     6135 2023-05-24 22:54:17.000000 vector_vault-1.1.3/vectorvault/ai.py
--rw-r--r--   0 johnrood   (501) staff       (20)     3525 2023-05-24 23:04:10.000000 vector_vault-1.1.3/vectorvault/cloudmanager.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.1.3/vectorvault/creds.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.1.3/vectorvault/download.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.1.3/vectorvault/itemize.py
--rw-r--r--   0 johnrood   (501) staff       (20)     1079 2023-05-24 19:36:47.000000 vector_vault-1.1.3/vectorvault/signup.py
--rw-r--r--   0 johnrood   (501) staff       (20)    17795 2023-05-25 06:00:59.000000 vector_vault-1.1.3/vectorvault/vault.py
--rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.1.3/vectorvault/wrap.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-27 01:28:34.288622 vector_vault-1.2.0/
+-rw-r--r--   0 johnrood   (501) staff       (20)     1471 2023-05-23 07:06:02.000000 vector_vault-1.2.0/LICENSE
+-rw-r--r--   0 johnrood   (501) staff       (20)    17414 2023-05-27 01:28:34.288468 vector_vault-1.2.0/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)    16689 2023-05-27 01:26:36.000000 vector_vault-1.2.0/README.md
+-rw-r--r--   0 johnrood   (501) staff       (20)       38 2023-05-27 01:28:34.288659 vector_vault-1.2.0/setup.cfg
+-rw-r--r--   0 johnrood   (501) staff       (20)     1075 2023-05-27 01:28:12.000000 vector_vault-1.2.0/setup.py
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-27 01:28:34.285780 vector_vault-1.2.0/vector_vault.egg-info/
+-rw-r--r--   0 johnrood   (501) staff       (20)    17414 2023-05-27 01:28:34.000000 vector_vault-1.2.0/vector_vault.egg-info/PKG-INFO
+-rw-r--r--   0 johnrood   (501) staff       (20)      406 2023-05-27 01:28:34.000000 vector_vault-1.2.0/vector_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)        1 2023-05-27 01:28:34.000000 vector_vault-1.2.0/vector_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       62 2023-05-27 01:28:34.000000 vector_vault-1.2.0/vector_vault.egg-info/requires.txt
+-rw-r--r--   0 johnrood   (501) staff       (20)       12 2023-05-27 01:28:34.000000 vector_vault-1.2.0/vector_vault.egg-info/top_level.txt
+drwxr-xr-x   0 johnrood   (501) staff       (20)        0 2023-05-27 01:28:34.288277 vector_vault-1.2.0/vectorvault/
+-rw-r--r--   0 johnrood   (501) staff       (20)      702 2023-05-24 19:36:19.000000 vector_vault-1.2.0/vectorvault/__init__.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     6135 2023-05-24 22:54:17.000000 vector_vault-1.2.0/vectorvault/ai.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     3525 2023-05-27 01:27:47.000000 vector_vault-1.2.0/vectorvault/cloudmanager.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1849 2023-05-24 09:44:23.000000 vector_vault-1.2.0/vectorvault/creds.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1299 2023-05-20 06:06:51.000000 vector_vault-1.2.0/vectorvault/download.py
+-rw-r--r--   0 johnrood   (501) staff       (20)     1542 2023-05-22 19:15:18.000000 vector_vault-1.2.0/vectorvault/itemize.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      890 2023-05-26 00:54:12.000000 vector_vault-1.2.0/vectorvault/signup.py
+-rw-r--r--   0 johnrood   (501) staff       (20)    17812 2023-05-25 07:36:53.000000 vector_vault-1.2.0/vectorvault/vault.py
+-rw-r--r--   0 johnrood   (501) staff       (20)      991 2023-05-20 06:06:45.000000 vector_vault-1.2.0/vectorvault/wrap.py
```

### Comparing `vector_vault-1.1.3/LICENSE` & `vector_vault-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.3/PKG-INFO` & `vector_vault-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_vault
-Version: 1.1.3
+Version: 1.2.0
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -48,15 +48,15 @@
 >> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 <br>
 
 # Interact with your Vault:
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="60%" height="60%" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/2acebcaa-f5dd-44c9-8bba-c10723bc7064/Vector+Vault+Vault+2000.png" width="60%" height="60%" />
 </p>
 
 Install Vector Vault:
 ```
 pip install vector-vault
 ```
 <br>
@@ -83,15 +83,15 @@
 3. Add the data to the Vault
 4. Get vectors embeddings 
 5. Save to the cloud vault
 
 ```
 from vectorvault import Vault
 
-vault = Vault(user='your_email', api_key='your_api_key', vault='name_of_vault)
+vault = Vault(user='your@email.com', api_key='your_api_key', vault='name_of_vault)
 
 text_data = 'some data'
 
 vault.add(text_data)
 
 vault.get_vectors()
 
@@ -151,34 +151,35 @@
 for result in similar_data:
     print(result['data'])
     print(result['metadata'])
 ```
 
 <br>
 
-To add meta data to your vault, just include it as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so there is always a name field in the metadata)
+## Metadata
+To add meta data to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so there is always a name field in the metadata)
 ```
-metadata = {
+meta = {
     'name': 'Lifestyle in LA',
     'country': 'United State',
     'city': 'LA' 
 }
 
-vault.add(more_text_data, metadata)
+vault.add(text, meta)
 
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
 
 To add just the 'name' field to the metadata, call the `name` param in `add()` like this:
 ```
-vault.add(more_text_data, name='Lifestyle in LA')
+vault.add(text, name='Lifestyle in LA')
 
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
@@ -186,20 +187,66 @@
 To find the name later:
 ```
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['metadata']['name'])
 ```
+<br>
+
+### Add Any Meta Fields & Retrieve later
+Here we open the popular book by George Orwell, "1984", from a .txt file. We read the file and save all the book's text to a variable called "text". Then we create a dictionary containing all the information about the book. Then we save all that to the vault. When you call the vault later, you can reference any of the metadata. When referencing the vault with `get_similar()` or `get_chat(text, get_context=True)` the vault will return sample texts from the book, and if the vault has many books in it, you may want to know where that sample is coming from. The metadata is how you will know.
+
+
+```
+with open('1984.txt', 'r') as file:
+    text = file.read()
+
+book_metadata = {
+    'title': '1984',
+    'author': 'George Orwell',
+    'genre': 'Dystopian',
+    'publication_year': 1949,
+    'publisher': 'Secker & Warburg',
+    'ISBN': '978-0451524935',
+    'language': 'English',
+    'page_count': 328
+}
+
+vault.add(text, book_metadata)
+
+vault.get_vectors()
+
+vault.save()
+```
+
+<br>
+
+To find the metadata later:
+```
+similar_data = vault.get_similar("How will the government control you in the future?") 
+
+for result in similar_data:
+    print(result['metadata']['title'])
+    print(result['metadata']['author'])
+    print(result['metadata']['genre'])
+    # etc...
+```
+^ list is always returned. So you can break it down like above or like below...
+
+```
+similar_data = vault.get_similar("How will the government control you in the future?") 
+print(similar_data[0]['metadata']['title'])
+```
 
 <br>
 <br>
 
 ### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
-Retrieving items from the vault, or texts, is useful when using it supply context to a large language model, chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
+Retrieving items from the vault, is useful when using it supply context to a large language model, like chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
 ```
 question = "This text will be used find contextually similar references in the vault"
 
 answer = vault.get_chat(question, get_context=True)  
 print(answer)
 ```
 The following line will send chatgpt the question for response and not interact with the vault in any way
@@ -218,51 +265,49 @@
 science_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science')
 
 print(science_vault.get_vaults())
 ```
 >> Output: ['biology', 'physics', 'chemistry']
 
 
-
 ## Access vaults within vaults
 
 - biology vault within science vault
 ```
-biology_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/biology')
+biology_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/biology')
 ```
 
-
-
 - chemistry vault within science vault
 ```
-chemistry_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry')
+chemistry_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry')
 
 print(chemistry_vault.get_vaults())
 ```
 >> Output: ['reactions', 'formulas', 'lab notes']
 
 
-
 - lab notes vault within chemistry vault
 ```
-lab_notes_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry/lab notes')
+lab_notes_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
 
 <br>
 <br>
 
-# `get_chat()`
+# ChatGPT
+## With `get_chat()` you can use ChatGPT standalone or with Vault data integrated
+
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
 </p>
 <br>
 
-Chat get response from OpenAI's ChatGPT. 
-Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
-Enter your text, add optional chat history, and optionally choose a summary response (default: summmary=False)
+Get chat response from OpenAI's ChatGPT. 
+Rate limiting, auto retries, and chat histroy slicing auto-built-in so you can create complex chat capability without getting complicated. 
+Enter your text, optionally add chat history, and optionally choose a summary response instead (default: summmary=False)
 
 - Example Signle Usage: 
 `response = vault.get_chat(text)`
 
 - Example Chat: 
 `response = vault.get_chat(text, chat_history)`
 
@@ -382,15 +427,15 @@
 
 # Build an AI Cusomter Service Chat Bot
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/dceb5c7d-6ec6-4eda-82f2-b8848c7b519d/ai_chatbot_having_a_conversation.png" width="60%" height="60%" />
 </p>
 <br>
 
-In the following code, we will add all the customer conversations that a support team has ever had to a vault. (Assumes you have all the past conversations downloaded to a single text file). Then we we will take cusotmer requests, search the database for similar questions and answers. After that, we will instruct ChatGPT to use the previous answers the support team has given to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
+In the following code, we will add all of a company's past support conversations to a vault. (The conversations are stored in a .txt file). As new people message in, we will search the vault for similar questions and answers. We take the past answers returned from the vault and instruct ChatGPT to use those previous answers to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
 ```
 from vectorvault import Vault
 
@@ -404,29 +449,34 @@
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
 
-And just like that, in a only a few lines of code we created a customer service vault based on all customer support messages. Now whenever you want to use it in the wild, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
+And just like that, in a only a few lines of code we created a customer service vault. Now whenever you want to use it in production, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
 
 ```
-question = 'customer question text string'
+question = 'customer question'
 
 answer = vault.get_chat(question, get_context=True)
 ```
 
-That's all it takes to create an ai customer service chatbot that responds to your customers as well as any support rep!
+That's all it takes to create an AI customer service chatbot that responds as well as any support rep!
 
 
 <br>
 <br>
 
-If have any questions, leave a message/comment on github repo. 
+---
+<br>
+<br>
+
+If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
+
 
 <br>
 
 Open the "examples" folder and try out the Google Colab tutorials we have.
 
 Happy coding!
 <p align="center">
```

### Comparing `vector_vault-1.1.3/README.md` & `vector_vault-1.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 >> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 <br>
 
 # Interact with your Vault:
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="60%" height="60%" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/2acebcaa-f5dd-44c9-8bba-c10723bc7064/Vector+Vault+Vault+2000.png" width="60%" height="60%" />
 </p>
 
 Install Vector Vault:
 ```
 pip install vector-vault
 ```
 <br>
@@ -64,15 +64,15 @@
 3. Add the data to the Vault
 4. Get vectors embeddings 
 5. Save to the cloud vault
 
 ```
 from vectorvault import Vault
 
-vault = Vault(user='your_email', api_key='your_api_key', vault='name_of_vault)
+vault = Vault(user='your@email.com', api_key='your_api_key', vault='name_of_vault)
 
 text_data = 'some data'
 
 vault.add(text_data)
 
 vault.get_vectors()
 
@@ -132,34 +132,35 @@
 for result in similar_data:
     print(result['data'])
     print(result['metadata'])
 ```
 
 <br>
 
-To add meta data to your vault, just include it as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so there is always a name field in the metadata)
+## Metadata
+To add meta data to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so there is always a name field in the metadata)
 ```
-metadata = {
+meta = {
     'name': 'Lifestyle in LA',
     'country': 'United State',
     'city': 'LA' 
 }
 
-vault.add(more_text_data, metadata)
+vault.add(text, meta)
 
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
 
 To add just the 'name' field to the metadata, call the `name` param in `add()` like this:
 ```
-vault.add(more_text_data, name='Lifestyle in LA')
+vault.add(text, name='Lifestyle in LA')
 
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
@@ -167,20 +168,66 @@
 To find the name later:
 ```
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['metadata']['name'])
 ```
+<br>
+
+### Add Any Meta Fields & Retrieve later
+Here we open the popular book by George Orwell, "1984", from a .txt file. We read the file and save all the book's text to a variable called "text". Then we create a dictionary containing all the information about the book. Then we save all that to the vault. When you call the vault later, you can reference any of the metadata. When referencing the vault with `get_similar()` or `get_chat(text, get_context=True)` the vault will return sample texts from the book, and if the vault has many books in it, you may want to know where that sample is coming from. The metadata is how you will know.
+
+
+```
+with open('1984.txt', 'r') as file:
+    text = file.read()
+
+book_metadata = {
+    'title': '1984',
+    'author': 'George Orwell',
+    'genre': 'Dystopian',
+    'publication_year': 1949,
+    'publisher': 'Secker & Warburg',
+    'ISBN': '978-0451524935',
+    'language': 'English',
+    'page_count': 328
+}
+
+vault.add(text, book_metadata)
+
+vault.get_vectors()
+
+vault.save()
+```
+
+<br>
+
+To find the metadata later:
+```
+similar_data = vault.get_similar("How will the government control you in the future?") 
+
+for result in similar_data:
+    print(result['metadata']['title'])
+    print(result['metadata']['author'])
+    print(result['metadata']['genre'])
+    # etc...
+```
+^ list is always returned. So you can break it down like above or like below...
+
+```
+similar_data = vault.get_similar("How will the government control you in the future?") 
+print(similar_data[0]['metadata']['title'])
+```
 
 <br>
 <br>
 
 ### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
-Retrieving items from the vault, or texts, is useful when using it supply context to a large language model, chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
+Retrieving items from the vault, is useful when using it supply context to a large language model, like chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
 ```
 question = "This text will be used find contextually similar references in the vault"
 
 answer = vault.get_chat(question, get_context=True)  
 print(answer)
 ```
 The following line will send chatgpt the question for response and not interact with the vault in any way
@@ -199,51 +246,49 @@
 science_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science')
 
 print(science_vault.get_vaults())
 ```
 >> Output: ['biology', 'physics', 'chemistry']
 
 
-
 ## Access vaults within vaults
 
 - biology vault within science vault
 ```
-biology_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/biology')
+biology_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/biology')
 ```
 
-
-
 - chemistry vault within science vault
 ```
-chemistry_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry')
+chemistry_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry')
 
 print(chemistry_vault.get_vaults())
 ```
 >> Output: ['reactions', 'formulas', 'lab notes']
 
 
-
 - lab notes vault within chemistry vault
 ```
-lab_notes_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry/lab notes')
+lab_notes_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
 
 <br>
 <br>
 
-# `get_chat()`
+# ChatGPT
+## With `get_chat()` you can use ChatGPT standalone or with Vault data integrated
+
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
 </p>
 <br>
 
-Chat get response from OpenAI's ChatGPT. 
-Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
-Enter your text, add optional chat history, and optionally choose a summary response (default: summmary=False)
+Get chat response from OpenAI's ChatGPT. 
+Rate limiting, auto retries, and chat histroy slicing auto-built-in so you can create complex chat capability without getting complicated. 
+Enter your text, optionally add chat history, and optionally choose a summary response instead (default: summmary=False)
 
 - Example Signle Usage: 
 `response = vault.get_chat(text)`
 
 - Example Chat: 
 `response = vault.get_chat(text, chat_history)`
 
@@ -363,15 +408,15 @@
 
 # Build an AI Cusomter Service Chat Bot
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/dceb5c7d-6ec6-4eda-82f2-b8848c7b519d/ai_chatbot_having_a_conversation.png" width="60%" height="60%" />
 </p>
 <br>
 
-In the following code, we will add all the customer conversations that a support team has ever had to a vault. (Assumes you have all the past conversations downloaded to a single text file). Then we we will take cusotmer requests, search the database for similar questions and answers. After that, we will instruct ChatGPT to use the previous answers the support team has given to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
+In the following code, we will add all of a company's past support conversations to a vault. (The conversations are stored in a .txt file). As new people message in, we will search the vault for similar questions and answers. We take the past answers returned from the vault and instruct ChatGPT to use those previous answers to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
 ```
 from vectorvault import Vault
 
@@ -385,29 +430,34 @@
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
 
-And just like that, in a only a few lines of code we created a customer service vault based on all customer support messages. Now whenever you want to use it in the wild, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
+And just like that, in a only a few lines of code we created a customer service vault. Now whenever you want to use it in production, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
 
 ```
-question = 'customer question text string'
+question = 'customer question'
 
 answer = vault.get_chat(question, get_context=True)
 ```
 
-That's all it takes to create an ai customer service chatbot that responds to your customers as well as any support rep!
+That's all it takes to create an AI customer service chatbot that responds as well as any support rep!
 
 
 <br>
 <br>
 
-If have any questions, leave a message/comment on github repo. 
+---
+<br>
+<br>
+
+If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
+
 
 <br>
 
 Open the "examples" folder and try out the Google Colab tutorials we have.
 
 Happy coding!
 <p align="center">
```

### Comparing `vector_vault-1.1.3/setup.py` & `vector_vault-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="vector_vault",
-    version="1.1.3",
+    version="1.2.0",
     packages=find_packages(),
     author="VectorVault.io",
     author_email="john@johnrood.com",
     description="VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/John-Rood/VectorVault",
```

### Comparing `vector_vault-1.1.3/vector_vault.egg-info/PKG-INFO` & `vector_vault-1.2.0/vector_vault.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-vault
-Version: 1.1.3
+Version: 1.2.0
 Summary: VectorVault: Simplified vector database management in the cloud for machine learning and generative ai workflows
 Home-page: https://github.com/John-Rood/VectorVault
 Author: VectorVault.io
 Author-email: john@johnrood.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: Other/Proprietary License
@@ -48,15 +48,15 @@
 >> `get_vectors()` utilizes openai embeddings api and internally batches vector embeddings with OpenAI's text-embeddings-ada-002 model, and comes with auto rate-limiting and concurrent requests for maximum processing speed
 
 
 <br>
 
 # Interact with your Vault:
 <p align="center">
-  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/3a6c60a3-79ac-467c-b640-c434499ca76d/Vector+Vault+Vault+2000.jpg" width="60%" height="60%" />
+  <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/2acebcaa-f5dd-44c9-8bba-c10723bc7064/Vector+Vault+Vault+2000.png" width="60%" height="60%" />
 </p>
 
 Install Vector Vault:
 ```
 pip install vector-vault
 ```
 <br>
@@ -83,15 +83,15 @@
 3. Add the data to the Vault
 4. Get vectors embeddings 
 5. Save to the cloud vault
 
 ```
 from vectorvault import Vault
 
-vault = Vault(user='your_email', api_key='your_api_key', vault='name_of_vault)
+vault = Vault(user='your@email.com', api_key='your_api_key', vault='name_of_vault)
 
 text_data = 'some data'
 
 vault.add(text_data)
 
 vault.get_vectors()
 
@@ -151,34 +151,35 @@
 for result in similar_data:
     print(result['data'])
     print(result['metadata'])
 ```
 
 <br>
 
-To add meta data to your vault, just include it as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so there is always a name field in the metadata)
+## Metadata
+To add meta data to your vault, just include the meta as a parameter in `add()`. Meta is always a dict, and you can add any fields you want. (If you don't add a 'name' field, a generic one will automatically be generated, so there is always a name field in the metadata)
 ```
-metadata = {
+meta = {
     'name': 'Lifestyle in LA',
     'country': 'United State',
     'city': 'LA' 
 }
 
-vault.add(more_text_data, metadata)
+vault.add(text, meta)
 
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
 
 To add just the 'name' field to the metadata, call the `name` param in `add()` like this:
 ```
-vault.add(more_text_data, name='Lifestyle in LA')
+vault.add(text, name='Lifestyle in LA')
 
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
@@ -186,20 +187,66 @@
 To find the name later:
 ```
 similar_data = vault.get_similar("Your text input") 
 
 for result in similar_data:
     print(result['metadata']['name'])
 ```
+<br>
+
+### Add Any Meta Fields & Retrieve later
+Here we open the popular book by George Orwell, "1984", from a .txt file. We read the file and save all the book's text to a variable called "text". Then we create a dictionary containing all the information about the book. Then we save all that to the vault. When you call the vault later, you can reference any of the metadata. When referencing the vault with `get_similar()` or `get_chat(text, get_context=True)` the vault will return sample texts from the book, and if the vault has many books in it, you may want to know where that sample is coming from. The metadata is how you will know.
+
+
+```
+with open('1984.txt', 'r') as file:
+    text = file.read()
+
+book_metadata = {
+    'title': '1984',
+    'author': 'George Orwell',
+    'genre': 'Dystopian',
+    'publication_year': 1949,
+    'publisher': 'Secker & Warburg',
+    'ISBN': '978-0451524935',
+    'language': 'English',
+    'page_count': 328
+}
+
+vault.add(text, book_metadata)
+
+vault.get_vectors()
+
+vault.save()
+```
+
+<br>
+
+To find the metadata later:
+```
+similar_data = vault.get_similar("How will the government control you in the future?") 
+
+for result in similar_data:
+    print(result['metadata']['title'])
+    print(result['metadata']['author'])
+    print(result['metadata']['genre'])
+    # etc...
+```
+^ list is always returned. So you can break it down like above or like below...
+
+```
+similar_data = vault.get_similar("How will the government control you in the future?") 
+print(similar_data[0]['metadata']['title'])
+```
 
 <br>
 <br>
 
 ### Use `get_chat()` with `get_context=True` to get response from chatgpt referencing vault data
-Retrieving items from the vault, or texts, is useful when using it supply context to a large language model, chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
+Retrieving items from the vault, is useful when using it supply context to a large language model, like chatgpt for instance, to get a contextualized response. The follow example searches the vault for 4 similar results and then give those to chatgpt as context, asking chatgpt answer the question using the vault data.
 ```
 question = "This text will be used find contextually similar references in the vault"
 
 answer = vault.get_chat(question, get_context=True)  
 print(answer)
 ```
 The following line will send chatgpt the question for response and not interact with the vault in any way
@@ -218,51 +265,49 @@
 science_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science')
 
 print(science_vault.get_vaults())
 ```
 >> Output: ['biology', 'physics', 'chemistry']
 
 
-
 ## Access vaults within vaults
 
 - biology vault within science vault
 ```
-biology_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/biology')
+biology_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/biology')
 ```
 
-
-
 - chemistry vault within science vault
 ```
-chemistry_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry')
+chemistry_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry')
 
 print(chemistry_vault.get_vaults())
 ```
 >> Output: ['reactions', 'formulas', 'lab notes']
 
 
-
 - lab notes vault within chemistry vault
 ```
-lab_notes_vault = Vault(user='your_user_id', api_key='your_api_key', vault='science/chemistry/lab notes')
+lab_notes_vault = Vault(user='your@email.com', api_key='your_api_key', vault='science/chemistry/lab notes')
 ```
 
 <br>
 <br>
 
-# `get_chat()`
+# ChatGPT
+## With `get_chat()` you can use ChatGPT standalone or with Vault data integrated
+
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/74776e31-4bfd-4d6b-837b-674790ca4288/wisdomandwealth_Electric_Yellow_and_Dark_Blue_-_chat_messages_g_c81a4325-5347-44a7-879d-a58a6d115446.png" width="60%" height="60%" />
 </p>
 <br>
 
-Chat get response from OpenAI's ChatGPT. 
-Rate limiting, auto retries, and chat histroy slicing built-in so you can chat with ease. 
-Enter your text, add optional chat history, and optionally choose a summary response (default: summmary=False)
+Get chat response from OpenAI's ChatGPT. 
+Rate limiting, auto retries, and chat histroy slicing auto-built-in so you can create complex chat capability without getting complicated. 
+Enter your text, optionally add chat history, and optionally choose a summary response instead (default: summmary=False)
 
 - Example Signle Usage: 
 `response = vault.get_chat(text)`
 
 - Example Chat: 
 `response = vault.get_chat(text, chat_history)`
 
@@ -382,15 +427,15 @@
 
 # Build an AI Cusomter Service Chat Bot
 <p align="center">
   <img src="https://images.squarespace-cdn.com/content/646ad2edeaaf682a9bbc36da/dceb5c7d-6ec6-4eda-82f2-b8848c7b519d/ai_chatbot_having_a_conversation.png" width="60%" height="60%" />
 </p>
 <br>
 
-In the following code, we will add all the customer conversations that a support team has ever had to a vault. (Assumes you have all the past conversations downloaded to a single text file). Then we we will take cusotmer requests, search the database for similar questions and answers. After that, we will instruct ChatGPT to use the previous answers the support team has given to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
+In the following code, we will add all of a company's past support conversations to a vault. (The conversations are stored in a .txt file). As new people message in, we will search the vault for similar questions and answers. We take the past answers returned from the vault and instruct ChatGPT to use those previous answers to answer this new question. (NOTE: This will also work based on a customer FAQ, or customer support response templates).
 
 <br>
 
 ### Create the Customer Service Vault
 ```
 from vectorvault import Vault
 
@@ -404,29 +449,34 @@
 vault.get_vectors()
 
 vault.save()
 ```
 
 <br>
 
-And just like that, in a only a few lines of code we created a customer service vault based on all customer support messages. Now whenever you want to use it in the wild, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
+And just like that, in a only a few lines of code we created a customer service vault. Now whenever you want to use it in production, just connect to that vault, and use the `get_chat()` with `get_context=True`. When you call `get_chat(text, get_context=True)` it will take the customer's question, search the vault to find the most similar questions and answers, then have ChatGPT reply to the customer using that information.
 
 ```
-question = 'customer question text string'
+question = 'customer question'
 
 answer = vault.get_chat(question, get_context=True)
 ```
 
-That's all it takes to create an ai customer service chatbot that responds to your customers as well as any support rep!
+That's all it takes to create an AI customer service chatbot that responds as well as any support rep!
 
 
 <br>
 <br>
 
-If have any questions, leave a message/comment on github repo. 
+---
+<br>
+<br>
+
+If have any questions, drop a message in our [Discord channel](https://discord.gg/AkMsP9Uq), happy to help.
+
 
 <br>
 
 Open the "examples" folder and try out the Google Colab tutorials we have.
 
 Happy coding!
 <p align="center">
```

### Comparing `vector_vault-1.1.3/vectorvault/__init__.py` & `vector_vault-1.2.0/vectorvault/__init__.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.3/vectorvault/ai.py` & `vector_vault-1.2.0/vectorvault/ai.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.3/vectorvault/cloudmanager.py` & `vector_vault-1.2.0/vectorvault/cloudmanager.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.3/vectorvault/creds.py` & `vector_vault-1.2.0/vectorvault/creds.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.3/vectorvault/download.py` & `vector_vault-1.2.0/vectorvault/download.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.3/vectorvault/itemize.py` & `vector_vault-1.2.0/vectorvault/itemize.py`

 * *Files identical despite different names*

### Comparing `vector_vault-1.1.3/vectorvault/signup.py` & `vector_vault-1.2.0/vectorvault/signup.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,11 @@
         'first': first_name,
         'last': last_name,
         'email': email,
         'password': password
     }
     response = requests.post(url, headers=headers, data=data)
 
-    # Always print the response status code and body
-    print(f"Response status code: {response.status_code}")
-    print(f"Response body: {response.text}")  # prints raw response content
-
     if response.status_code != 200:
         return {}
 
     return response.json()
```

### Comparing `vector_vault-1.1.3/vectorvault/vault.py` & `vector_vault-1.2.0/vectorvault/vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,22 +23,22 @@
 from concurrent.futures import ThreadPoolExecutor
 from .cloudmanager import CloudManager
 from .ai import AI
 from .itemize import itemize, name, name_vecs, get_item, build_return, get_vectors
 
 
 class Vault:
-    def __init__(self, user: str, api_key: str, vault: str = None, dims: int = 1536, verbose: bool = False):
+    def __init__(self, user: str = None, api_key: str = None, vault: str = None, dims: int = 1536, verbose: bool = False):
         self.vault = vault.strip() if vault else 'home'
         self.vectors = get_vectors(dims)
         self.dims = dims
         try:
             self.cloud_manager = CloudManager(user, api_key, self.vault)
         except:
-            print('API KEY FAILED! Using vault without cloud access. `get_chat()` will still work')
+            print('API KEY NOT FOUND! Using Vault without cloud access. `get_chat()` will still work')
             # user can still use the get_chat() function without an api key
             pass
         self.x = 0
         self.x_checked = False
         self.verbose = verbose
         self.items = []
         self.last_time = None
```

### Comparing `vector_vault-1.1.3/vectorvault/wrap.py` & `vector_vault-1.2.0/vectorvault/wrap.py`

 * *Files identical despite different names*

