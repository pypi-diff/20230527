# Comparing `tmp/pyplAI-1.0.2.tar.gz` & `tmp/pyplAI-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplAI-1.0.2.tar", last modified: Sat Mar 25 17:24:34 2023, max compression
+gzip compressed data, was "pyplAI-1.0.3.tar", last modified: Sat May 27 11:19:44 2023, max compression
```

## Comparing `pyplAI-1.0.2.tar` & `pyplAI-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-03-25 17:24:34.959329 pyplAI-1.0.2/
--rw-rw-rw-   0        0        0     1079 2023-03-18 12:31:53.000000 pyplAI-1.0.2/LICENSE.md
--rw-rw-rw-   0        0        0       28 2023-03-18 13:51:35.000000 pyplAI-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    18167 2023-03-25 17:24:34.956329 pyplAI-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    16661 2023-03-23 22:38:41.000000 pyplAI-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-25 17:24:34.940329 pyplAI-1.0.2/pyplAI/
--rw-rw-rw-   0        0        0    27127 2023-03-25 16:41:11.000000 pyplAI-1.0.2/pyplAI/Algoritmos.py
--rw-rw-rw-   0        0        0      129 2023-03-25 14:58:03.000000 pyplAI-1.0.2/pyplAI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-25 17:24:34.955346 pyplAI-1.0.2/pyplAI.egg-info/
--rw-rw-rw-   0        0        0    18167 2023-03-25 17:24:34.000000 pyplAI-1.0.2/pyplAI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-03-25 17:24:34.000000 pyplAI-1.0.2/pyplAI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-25 17:24:34.000000 pyplAI-1.0.2/pyplAI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-03-25 17:24:34.000000 pyplAI-1.0.2/pyplAI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-25 17:24:34.960333 pyplAI-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1769 2023-03-25 17:22:48.000000 pyplAI-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:19:44.749609 pyplAI-1.0.3/
+-rw-rw-rw-   0        0        0     1079 2023-03-18 12:31:53.000000 pyplAI-1.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0       28 2023-03-18 13:51:35.000000 pyplAI-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    18195 2023-05-27 11:19:44.748508 pyplAI-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    16988 2023-05-27 11:13:52.000000 pyplAI-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-27 11:19:44.733947 pyplAI-1.0.3/pyplAI/
+-rw-rw-rw-   0        0        0    27131 2023-05-27 11:14:19.000000 pyplAI-1.0.3/pyplAI/Algoritmos.py
+-rw-rw-rw-   0        0        0      129 2023-03-25 14:58:03.000000 pyplAI-1.0.3/pyplAI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-27 11:19:44.748508 pyplAI-1.0.3/pyplAI.egg-info/
+-rw-rw-rw-   0        0        0    18195 2023-05-27 11:19:44.000000 pyplAI-1.0.3/pyplAI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-05-27 11:19:44.000000 pyplAI-1.0.3/pyplAI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-27 11:19:44.000000 pyplAI-1.0.3/pyplAI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-27 11:19:44.000000 pyplAI-1.0.3/pyplAI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-27 11:19:44.749609 pyplAI-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1769 2023-05-27 11:17:18.000000 pyplAI-1.0.3/setup.py
```

### Comparing `pyplAI-1.0.2/LICENSE.md` & `pyplAI-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyplAI-1.0.2/PKG-INFO` & `pyplAI-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplAI
-Version: 1.0.2
+Version: 1.0.3
 Summary: Biblioteca para Python con algoritmos de resolución de juegos de mesa (minimax, MCTS, SO-ISMCTS y MO-ISMCTS)
 Home-page: https://github.com/plss12/pyplAI
 Author: Pedro Luis Soto Santos
 Author-email: pepoluis712@gmail.com
 License: MIT
 Keywords: python,articial intelligence,AI,games,board games,minimax,alpha-beta,monte carlo,monte carlo tree search,UCT,game theory,information set,perfect information,imperfect information
 Classifier: Development Status :: 4 - Beta
@@ -22,36 +22,36 @@
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # pyplAI
 
 ## Introducción
-Esta biblioteca para Python es el resultado final de un Trabajo de Fin de Grado centrado en la implementación de algoritmos de *Monte Carlo Tree Search* (MCTS) y *minimax* para diferentes tipos de juegos de mesa, entre ellos, según clasifica la teoría de juegos, los juegos de información perfecta, como lo son *el ajedrez* o *las damas*, en los que en todo momento cualquier jugador puede ver toda la información del juego, como los posibles movimientos del rival, y juegos de información imperfecta, como lo son la mayoría de juegos de cartas como por ejemplo *el Uno* o *la brisca*, en el que los jugadores solo conocen información propia, como sus cartas, o información general del juego, como el estado de la mesa, pero desconocen la información del rival, como las cartas de los demás jugadores.
+Esta biblioteca para *Python* es el resultado final de un Trabajo de Fin de Grado centrado en la implementación de algoritmos de *Monte Carlo Tree Search (MCTS)* y *minimax* para diferentes tipos de juegos de mesa, entre ellos, según clasifica la teoría de juegos, los juegos de información perfecta, como lo son el *ajedrez* o las *damas*, en los que en todo momento cualquier jugador puede ver toda la información del juego, como los posibles movimientos del rival, y juegos de información imperfecta, como lo son la mayoría de juegos de cartas como por ejemplo el *Uno* o la *brisca*, en el que los jugadores solo conocen información propia, como sus cartas, o información general del juego, como el estado de la mesa, pero desconocen la información del rival, como las cartas de los demás jugadores.
 
 ### Juegos de Información Perfecta
 
-Para este tipo de juegos se han implementado los algoritmos de MCTS con UCT [[1]](#MCTS) y minimax con la técnica de poda de alfa-beta [[2]](#Minimax). Además, como ejemplos para ver el correcto uso de la biblioteca, se han creado diferentes juegos de mesa, entre ellos, *TicTacToe* (3 en raya), *Ultimate TicTacToe* [[3]](#UltimateTicTacToe) y *las damas*.
+Para este tipo de juegos se han implementado los algoritmos de *MCTS con UCT* [[1]](#MCTS) y *minimax* con la técnica de *poda de alfa-beta* [[2]](#Minimax). Además, como ejemplos para ver el correcto uso de la biblioteca, se han creado diferentes juegos de mesa, entre ellos, el *Tic-Tac-Toe* (3 en raya), el *Ultimate Tic-Tac-Toe* [[3]](#UltimateTicTacToe) y las *damas*.
 
 ### Juegos de Información Imperfecta
 
-Para este segundo tipo de juegos se han implementado dos algoritmos, el *Single Observer Information Set Monte Carlo Tree Search* [[4]](#ISMCTS) (SO-ISMCTS) y el *Multiple Observer Information Set Monte Carlo Tree Search* [[4]](#ISMCTS) (MO-ISMCTS). El primero de estos algoritmos genera un único árbol desde el punto de vista del jugador al que le toca jugar. Por otro lado, el segundo algoritmo crea un árbol para cada uno de los jugadores y agrupa las acciones que son indiferenciables desde el punto de vista de este jugador, es decir, si un jugador puede realizar varios movimientos que no aportarían información a los rivales, agrupa estos movimientos como si fuesen uno solo, creando un único nodo en el árbol de los jugadores rivales.
+Para este segundo tipo de juegos se han implementado dos algoritmos, el *Single Observer Information Set Monte Carlo Tree Search (SO-ISMCTS)* [[4]](#ISMCTS) y el *Multiple Observer Information Set Monte Carlo Tree Search (MO-ISMCTS)* [[4]](#ISMCTS). El primero de estos algoritmos genera un único árbol desde el punto de vista del jugador al que le toca jugar. Por otro lado, el segundo algoritmo crea un árbol para cada uno de los jugadores y agrupa las acciones que son indiferenciables desde el punto de vista de este jugador, es decir, si un jugador puede realizar varios movimientos que no aportarían información a los rivales, agrupa estos movimientos como si fuesen uno solo, creando un único nodo en el árbol de los jugadores rivales.
 
 Un ejemplo serían los juegos en los que un jugador intercambia una de las cartas de su mano con cualquier carta de la baraja, cuando el jugador efectúa este intercambio los demás jugadores no reciben ningún tipo de información sobre el intercambio de cartas, por lo que su conocimiento sobre el estado del juego no cambia. 
 
-Para estos algoritmos también se han desarrollado varios juegos como ejemplos de uso de la biblioteca, aunque ambos algoritmos se pueden usar en todos los juegos de información imperfecta, se ha diferenciado entre juegos para el SO-ISMCTS y el MO-ISMCTS. Para el primer algoritmo se ha creado *el juego de la escoba*, *el Stratego* y *el blackJack*, y para el segundo se ha desarrollado *el holjjak* (juego de adivinar las canicas del rival) y *el phantom* (variante del 4 en raya en el que no se ven los movimientos del rival).
+Para estos algoritmos también se han desarrollado varios juegos como ejemplos de uso de la biblioteca, aunque ambos algoritmos se pueden usar en todos los juegos de información imperfecta, se ha diferenciado entre juegos para el *SO-ISMCTS* y el *MO-ISMCTS*. Para el primer algoritmo se ha creado el juego de la *escoba*, el *Stratego* y el *blackJack*, y para el segundo se ha desarrollado el *holjjak* (juego de adivinar las canicas del rival) y el *phantom* (variante del 4 en raya en el que no se ven los movimientos del rival).
 
 ## Manual de Uso
 El primer paso necesario para poder usar esta biblioteca es descargarla. Se puede descargar la biblioteca desde la consola usando el comando: 
 
 ``` python
 pip install pyplAI
 ```
 
-Tras esto, ya se puede importar en el archivo de Python del juego al que queramos implementarla.
+Tras esto, ya se puede importar en el archivo de *Python* del juego al que queramos implementarla.
 
 ``` python
 import pyplAI
 ```
 
 ### Clase sobre el Estado del Juego
 Para poder usar esta biblioteca es imprescindible que haya una clase que guarde la información necesaria sobre el estado del juego. Aunque se puede dar a esta clase el nombre que se desee, en este manual se utilizará una clase llamada *Juego* a modo de ejemplo.
@@ -201,15 +201,15 @@
         def heuristica(self, jugador):
                     .
                     .
                     .
             return evaluacion
 ```
 
-Por ejemplo, para el juego de *las damas* una posible heurística sería contar el número de fichas del jugador y restarle el número de fichas del rival. Hay multitud de posibles heurísticas para cada uno de los juegos, y se debe tener un conocimiento sobre el juego para poder crear una buena heurística, ya que la heurística tendrá un gran peso a la hora de decidir cuál es el mejor movimiento.
+Por ejemplo, para el juego de las *damas* una posible heurística sería contar el número de fichas del jugador y restarle el número de fichas del rival. Hay multitud de posibles heurísticas para cada uno de los juegos, y se debe tener un conocimiento sobre el juego para poder crear una buena heurística, ya que la heurística tendrá un gran peso a la hora de decidir cuál es el mejor movimiento.
 
 Al igual que en el método *gana_jugador*, el argumento *jugador* debe ser un número entero positivo, desde el 1, para el primer jugador, hasta *n*, para el último jugador, siendo *n* el número total de jugadores.
 
 ### Constructor Algoritmo
 
 Una vez tengamos todos estos métodos solamente debemos llamar a la biblioteca y al constructor del algoritmo que se desee utilizar. A esta llamada le pasaremos como argumentos los métodos necesarios para el uso de este algoritmo junto con algunas otras variables que detallaremos a continuación:
 
@@ -271,30 +271,30 @@
               Juego.es_movimiento_visible,
               numeroJugadores, 
               tiempoEjecucion)
 ```
 
 **•	Modo *verbose*:**
 
-Si queremos ver algunos detalles cuando ejecutemos el algoritmo, se debe añadir un *True* como último argumento en la llamada al constructor. Este modo mostrará información útil del algoritmo por consola, como por ejemplo, tiempo de ejecución, número de nodos creados y visitados y demás características propias de cada uno de los algoritmos. Un ejemplo de como quedaría la creación del algoritmo de MCTS con este argumento extra sería el siguiente:
+Si queremos ver algunos detalles cuando ejecutemos el algoritmo, se debe añadir un *True* como último argumento en la llamada al constructor. Este modo mostrará información útil del algoritmo por consola, como por ejemplo, tiempo de ejecución, número de nodos creados y visitados y demás características propias de cada uno de los algoritmos. Un ejemplo de como quedaría la creación del algoritmo de *MCTS* con este argumento extra sería el siguiente:
 
 ``` python
   mcts = pyplAI.MCTS(
          Juego.aplica_movimiento,
          Juego.obtiene_movimientos, 
          Juego.es_estado_final, 
          Juego.gana_jugador, 
          numeroJugadores, 
          tiempoEjecucion,
          True)
 ```
 
 ### Ejecución Algoritmo
 
-Una vez tengamos el objeto del algoritmo que se quiere utilizar solamente se debe llamar a su método *ejecuta* y pasarle como argumento el objeto que contiene el estado actual del juego, esto devolverá el mejor movimiento encontrado durante el tiempo de computación dado, para los algoritmos de *Monte Carlo*, o la profundidad de búsqueda, en el caso del algoritmo *minimax*. A continuación, se mostrará el código de ejemplo en el que se usa el algoritmo de *MCTS* para obtener un movimiento y seguidamente aplicarlo al juego, obtiendo así un nuevo estado del juego:
+Una vez tengamos el objeto del algoritmo que se quiere utilizar solamente se debe llamar a su método *ejecuta* y pasarle como argumento el objeto que contiene el estado actual del juego, esto devolverá el mejor movimiento encontrado durante el tiempo de computación dado, para los algoritmos de *Monte Carlo*, o la profundidad de búsqueda, en el caso del algoritmo *minimax*. A continuación, se mostrará el código de ejemplo en el que se usa el algoritmo de *MCTS* para obtener un movimiento y seguidamente aplicarlo al juego, obteniendo así un nuevo estado del juego:
 
 ``` python
   def main():
       juego = Juego()
       movimiento = mcts.ejecuta(juego)
       juego = aplica_movimiento(movimiento)
 ```
```

### Comparing `pyplAI-1.0.2/README.md` & `pyplAI-1.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,298 +1,298 @@
-# pyplAI
-
-## Introducción
-Esta biblioteca para Python es el resultado final de un Trabajo de Fin de Grado centrado en la implementación de algoritmos de *Monte Carlo Tree Search* (MCTS) y *minimax* para diferentes tipos de juegos de mesa, entre ellos, según clasifica la teoría de juegos, los juegos de información perfecta, como lo son *el ajedrez* o *las damas*, en los que en todo momento cualquier jugador puede ver toda la información del juego, como los posibles movimientos del rival, y juegos de información imperfecta, como lo son la mayoría de juegos de cartas como por ejemplo *el Uno* o *la brisca*, en el que los jugadores solo conocen información propia, como sus cartas, o información general del juego, como el estado de la mesa, pero desconocen la información del rival, como las cartas de los demás jugadores.
-
-### Juegos de Información Perfecta
-
-Para este tipo de juegos se han implementado los algoritmos de MCTS con UCT [[1]](#MCTS) y minimax con la técnica de poda de alfa-beta [[2]](#Minimax). Además, como ejemplos para ver el correcto uso de la biblioteca, se han creado diferentes juegos de mesa, entre ellos, *TicTacToe* (3 en raya), *Ultimate TicTacToe* [[3]](#UltimateTicTacToe) y *las damas*.
-
-### Juegos de Información Imperfecta
-
-Para este segundo tipo de juegos se han implementado dos algoritmos, el *Single Observer Information Set Monte Carlo Tree Search* [[4]](#ISMCTS) (SO-ISMCTS) y el *Multiple Observer Information Set Monte Carlo Tree Search* [[4]](#ISMCTS) (MO-ISMCTS). El primero de estos algoritmos genera un único árbol desde el punto de vista del jugador al que le toca jugar. Por otro lado, el segundo algoritmo crea un árbol para cada uno de los jugadores y agrupa las acciones que son indiferenciables desde el punto de vista de este jugador, es decir, si un jugador puede realizar varios movimientos que no aportarían información a los rivales, agrupa estos movimientos como si fuesen uno solo, creando un único nodo en el árbol de los jugadores rivales.
-
-Un ejemplo serían los juegos en los que un jugador intercambia una de las cartas de su mano con cualquier carta de la baraja, cuando el jugador efectúa este intercambio los demás jugadores no reciben ningún tipo de información sobre el intercambio de cartas, por lo que su conocimiento sobre el estado del juego no cambia. 
-
-Para estos algoritmos también se han desarrollado varios juegos como ejemplos de uso de la biblioteca, aunque ambos algoritmos se pueden usar en todos los juegos de información imperfecta, se ha diferenciado entre juegos para el SO-ISMCTS y el MO-ISMCTS. Para el primer algoritmo se ha creado *el juego de la escoba*, *el Stratego* y *el blackJack*, y para el segundo se ha desarrollado *el holjjak* (juego de adivinar las canicas del rival) y *el phantom* (variante del 4 en raya en el que no se ven los movimientos del rival).
-
-## Manual de Uso
-El primer paso necesario para poder usar esta biblioteca es descargarla. Se puede descargar la biblioteca desde la consola usando el comando: 
-
-``` python
-pip install pyplAI
-```
-
-Tras esto, ya se puede importar en el archivo de Python del juego al que queramos implementarla.
-
-``` python
-import pyplAI
-```
-
-### Clase sobre el Estado del Juego
-Para poder usar esta biblioteca es imprescindible que haya una clase que guarde la información necesaria sobre el estado del juego. Aunque se puede dar a esta clase el nombre que se desee, en este manual se utilizará una clase llamada *Juego* a modo de ejemplo.
-
-``` python
-  class Juego:
-          .
-          .
-          .
-```
-
-### Atributo Obligatorio *jugadorActual*
-Debido a que los algoritmos necesitan saber cuál es el jugador al cual le toca jugar en cada uno de los turnos, es obligatorio añadir un atributo *jugadorActual* en la clase del juego. Además, es muy importante que este atributo tenga este mismo nombre.
-
-``` python
-  class Juego:
-    def __init__(self):
-        self.jugadorActual = 1
-                .
-                .
-                .
-```
-
-Este atributo debe contener un valor numérico que representa el índice del jugador al que le toca jugar (empezando por 1). También, debe ir actualizándose conforme se avanza en el juego, por ejemplo, en el *3 en raya*, este atributo se debe iniciar con el valor 1, pero cuando el primer jugador realice su movimiento, se actualiza al valor 2, indicando que el segundo jugador es el que debe realizar su jugada.
-
-Además del atributo para identificar el jugador actual del estado del juego, esta clase deberá implementar ciertos métodos para poder interactuar y obtener información sobre el estado del juego. Algunos métodos son comunes para todos los algoritmos, mientras que otros algoritmos requieren de métodos específicos. Cabe destacar que estos métodos pueden ser nombrados de forma distinta a como se mostrará a continuación, pero es totalmente necesario que reciban los parámetros de entrada y devuelvan la salida tal y como se especifica en este manual.
-
-### Métodos Generales
-
-Los siguientes 4 métodos serán obligatorios para todos los algoritmos que se implementan en esta biblioteca:
-
-**•	obtiene_movimientos(self):** Devolverá una lista con todos los movimientos posibles del jugador actual del estado del juego, es recomendable devolver estos movimientos en un orden aleatorio.
-
-``` python
-  class Juego:
-          .
-          .
-          .
-        def obtiene_movimientos(self):
-                    .
-                    .
-                    .
-            return movimientos
-```
-
-**•	aplica_movimiento(self, movimiento):** Aplicará el movimiento dado al estado del juego y devolverá el estado resultante (*self*).
-
-``` python
-  class Juego:
-          .
-          .
-          .
-        def aplica_movimiento(self, movimiento):
-                    .
-                    .
-                    .
-            return self
-```
-
-**•	es_estado_final(self):** Comprueba el estado actual del juego, devolviendo *True* o *False* dependiendo de si es un estado final o no.
-
-``` python
-  class Juego:
-          .
-          .
-          .
-        def es_estado_final(self):
-                    .
-                    .
-                    .
-            return True
-              o
-            return False
-```
-
-**•	gana_jugador(self, jugador):** Comprueba si el jugador dado gana el juego en el estado actual de este, devolviendo *True* en caso de que sea ganador, o *False* en caso contrario. La variable *jugador* debe ser un número entero positivo, y se debe situar en el rango de 1, para el primer jugador del juego, hasta *n*, siendo *n* el número total de jugadores.
-
-``` python
-  class Juego:
-          .
-          .
-          .
-        def gana_jugador(self, jugador):
-                    .
-                    .
-                    .
-            return True
-              o
-            return False
-```
-
-### Métodos SO/MO-ISMCTS
-
-Además de los 4 métodos anteriores, los algoritmos de *SO-ISMCTS* y *MO-ISMCTS* necesitan un método adicional para su uso, el cuál se explica a continuación:
-
-**•	determinación(self):** Devuelve una determinación aleatoria del estado del juego, desde el punto de vista del jugador actual.
-
-``` python
-  class Juego:
-          .
-          .
-          .
-        def determinacion(self):
-                    .
-                    .
-                    .
-            return determinacion
-```
-
-Por ejemplo, para un juego de cartas en el que cada jugador tiene una mano, hay una mesa con cartas visibles, una pila de descartes y un mazo de robo inicial, el jugador actual no tiene conocimiento sobre las cartas del rival ni las cartas del mazo de robo, pero si sabe cuáles son sus cartas, las de la mesa y las que han sido mandadas a la pila de descartes, por lo que tiene la información sobre cuáles son las cartas restantes, pero aún no sabe donde se encuentran. 
-
-Con esta información, este método debe dar un estado del juego en el que aleatoriamente se distribuyan las cartas que el jugador no tiene localizadas entre las zonas en las que no sabe que cartas hay, en este caso, las zonas serían las manos de los rivales y el mazo de robo.
-
-### Métodos MO-ISMCTS
-
-Además, para el funcionamiento del algoritmo *MO-ISMCTS* se necesitará otro método adicional:
-
-**•	es_movimiento_visible(movimiento):** Este método, dado un movimiento, devuelve *True* si es un movimiento visible para los rivales, o *False* en caso contrario.
-
-``` python
-  class Juego:
-          .
-          .
-          .
-        def es_movimiento_visible(movimiento):
-                    .
-                    .
-                    .
-            return True
-              o
-            return False
-```
-
-Por ejemplo, un movimiento visible para los rivales sería jugar una carta de tu mano sobre la mesa, por lo que, haría saber a los rivales el lugar exacto de esa carta, cosa que antes no sabían. Sin embargo, un movimiento no visible sería intercambiar una carta de tu mano con el mazo de robo sin revelar ninguna de las dos. Esta acción no mostraría nueva información a ningún rival, ya que no se muestran las cartas y los rivales seguirán sin saber que cartas hay en tu mano ni que cartas hay en el mazo.
-
-### Métodos Minimax
-
-En el caso del algoritmo de *minimax*, además de los 4 métodos generales, se necesita un método que devuelva una heurística sobre el estado del juego, es decir, que evalúe su estado para saber como de bueno es desde el punto de vista de un jugador dado:
-
-**•	heuristica(self, jugador):** Este método debe devolver un número entero que refleje una evaluación sobre como de bueno es el estado del juego para un jugador dado. Esta evaluación debe ser mayor cuanto mejor sea el estado del juego para este jugador.
-
-``` python
-  class Juego:
-          .
-          .
-          .
-        def heuristica(self, jugador):
-                    .
-                    .
-                    .
-            return evaluacion
-```
-
-Por ejemplo, para el juego de *las damas* una posible heurística sería contar el número de fichas del jugador y restarle el número de fichas del rival. Hay multitud de posibles heurísticas para cada uno de los juegos, y se debe tener un conocimiento sobre el juego para poder crear una buena heurística, ya que la heurística tendrá un gran peso a la hora de decidir cuál es el mejor movimiento.
-
-Al igual que en el método *gana_jugador*, el argumento *jugador* debe ser un número entero positivo, desde el 1, para el primer jugador, hasta *n*, para el último jugador, siendo *n* el número total de jugadores.
-
-### Constructor Algoritmo
-
-Una vez tengamos todos estos métodos solamente debemos llamar a la biblioteca y al constructor del algoritmo que se desee utilizar. A esta llamada le pasaremos como argumentos los métodos necesarios para el uso de este algoritmo junto con algunas otras variables que detallaremos a continuación:
-
-**•	numeroJugadores:** Este argumento es obligatorio para todos los algoritmos,  representará el número de jugadores que contiene el juego, siendo este un número entero mayor que cero.
-
-**•	tiempoEjecucion:** Este argumento es común para todos los algoritmos de Monte Carlo, ya que, estos algoritmos necesitan un tiempo límite de ejecución antes de devolver el mejor movimiento encontrado. Este argumento debe ser un número real mayor que cero y representa el tiempo de ejecución en segundos.
-
-**•	profundidadBusqueda:** Este argumento solo es necesario en la llamada al constructor del algoritmo de *minimax*, y sirve para limitar la profundidad en el árbol de búsqueda. Este argumento debe ser un número entero mayor que cero.
-
-Sabiendo todo esto ya podemos ver como se deben hacer las llamadas a la biblioteca y los constructores para cada uno de los tipos de algoritmos. Es muy importante que se siga el orden mostrado en los argumentos de entrada. Además, recordar que *Juego* es la clase de ejemplo que contiene la información sobre el estado del juego, como el atributo *jugadorActual*, y los métodos explicados anteriormente.
-
-**•	MCTS:**
-
-``` python
-  mcts = pyplAI.MCTS(
-         Juego.aplica_movimiento,
-         Juego.obtiene_movimientos, 
-         Juego.es_estado_final, 
-         Juego.gana_jugador, 
-         numeroJugadores, 
-         tiempoEjecucion)
-```
-
-**•	Minimax:**
-
-``` python
-  minimax = pyplAI.Minimax(
-           Juego.aplica_movimiento,
-           Juego.obtiene_movimientos, 
-           Juego.es_estado_final, 
-           Juego.gana_jugador, 
-           Juego.heuristica,
-           numeroJugadores, 
-           profundidadBusqueda)
-```
-
-**•	SO-ISMCTS:**
-
-``` python
-  so_ismcts = pyplAI.SOISMCTS(
-              Juego.aplica_movimiento,
-              Juego.obtiene_movimientos, 
-              Juego.es_estado_final, 
-              Juego.gana_jugador, 
-              Juego.determinacion,
-              numeroJugadores, 
-              tiempoEjecucion)
-```
-
-**•	MO-ISMCTS:**
-
-``` python
-  mo_ismcts = pyplAI.MOISMCTS(
-              Juego.aplica_movimiento,
-              Juego.obtiene_movimientos, 
-              Juego.es_estado_final, 
-              Juego.gana_jugador, 
-              Juego.determinacion,
-              Juego.es_movimiento_visible,
-              numeroJugadores, 
-              tiempoEjecucion)
-```
-
-**•	Modo *verbose*:**
-
-Si queremos ver algunos detalles cuando ejecutemos el algoritmo, se debe añadir un *True* como último argumento en la llamada al constructor. Este modo mostrará información útil del algoritmo por consola, como por ejemplo, tiempo de ejecución, número de nodos creados y visitados y demás características propias de cada uno de los algoritmos. Un ejemplo de como quedaría la creación del algoritmo de MCTS con este argumento extra sería el siguiente:
-
-``` python
-  mcts = pyplAI.MCTS(
-         Juego.aplica_movimiento,
-         Juego.obtiene_movimientos, 
-         Juego.es_estado_final, 
-         Juego.gana_jugador, 
-         numeroJugadores, 
-         tiempoEjecucion,
-         True)
-```
-
-### Ejecución Algoritmo
-
-Una vez tengamos el objeto del algoritmo que se quiere utilizar solamente se debe llamar a su método *ejecuta* y pasarle como argumento el objeto que contiene el estado actual del juego, esto devolverá el mejor movimiento encontrado durante el tiempo de computación dado, para los algoritmos de *Monte Carlo*, o la profundidad de búsqueda, en el caso del algoritmo *minimax*. A continuación, se mostrará el código de ejemplo en el que se usa el algoritmo de *MCTS* para obtener un movimiento y seguidamente aplicarlo al juego, obtiendo así un nuevo estado del juego:
-
-``` python
-  def main():
-      juego = Juego()
-      movimiento = mcts.ejecuta(juego)
-      juego = aplica_movimiento(movimiento)
-```
-
-
-En caso de que el estado del juego no tenga ningún movimiento posible para aplicar los algoritmos devolverán *None*, y si solo hay un posible movimiento para aplicar, para ahorrar cálculos innecesarios, se devolverá el único movimiento posible.
-
-Si se tienen dudas sobre como integrar la biblioteca a juegos propios se recomienda ver los juegos del repositorio de *GitHub* ([*pyplAI*](https://github.com/plss12/pyplAI)) como ejemplos de uso. Este repositorio contiene la biblioteca y todos los juegos nombrados en la introducción de este manual, incluyendo las implementaciones de los algoritmos correspondientes con cada uno de ellos.
-
-## Contacto
-
-En caso de tener alguna duda, idea o aportación sobre la biblioteca por favor contactar al siguiente correo: [pepoluis712@gmail.com](mailto:pepoluis712@gmail.com)
-
-## Referencias
-
-<a id="MCTS"></a>
-[1] Cameron B. Browne, Edward Powley, Daniel Whitehouse, Simon M. Lucas, Peter I.Cowling, Philipp Rohlfshagen, Stephen Tavener, Diego Perez, Spyridon Samoth-rakis, and Simon Colton. A survey of monte carlo tree search methods. IEEETransactions on Computational Intelligence and AI in Games, 4(1):1–43, 2012. doi:10.1109/TCIAIG.2012.2186810. URL https://ieeexplore.ieee.org/document/6145622.
-
-<a id="Minimax"></a>
-[2] Patricio Mendoza. Alpha-beta pruning algorithm: The intelligence behind strategygames. page 9, 2022. URL https://www.researchgate.net/publication/360872512.
-
-<a id="UltimateTicTacToe"></a>
-[3] Eytan Lifshitz and David Tsurel. Ai approaches to ultimate tic-tac-toe. page 5, 2013. URL https://www.cs.huji.ac.il/w~ai/projects/2013/UlitmateTic-Tac-Toe/files/report.pdf.
-
-<a id="ISMCTS"></a>
-[4] Peter I. Cowling, Edward J. Powley, and Daniel Whitehouse. Information setmonte carlo tree search. IEEE Transactions on Computational Intelligence and AIin Games, 4(2):120–143, 2012. doi: 10.1109/TCIAIG.2012.2200894. URL https://ieeexplore.ieee.org/document/6203567.
+# pyplAI
+
+## Introducción
+Esta biblioteca para *Python* es el resultado final de un Trabajo de Fin de Grado centrado en la implementación de algoritmos de *Monte Carlo Tree Search (MCTS)* y *minimax* para diferentes tipos de juegos de mesa, entre ellos, según clasifica la teoría de juegos, los juegos de información perfecta, como lo son el *ajedrez* o las *damas*, en los que en todo momento cualquier jugador puede ver toda la información del juego, como los posibles movimientos del rival, y juegos de información imperfecta, como lo son la mayoría de juegos de cartas como por ejemplo el *Uno* o la *brisca*, en el que los jugadores solo conocen información propia, como sus cartas, o información general del juego, como el estado de la mesa, pero desconocen la información del rival, como las cartas de los demás jugadores.
+
+### Juegos de Información Perfecta
+
+Para este tipo de juegos se han implementado los algoritmos de *MCTS con UCT* [[1]](#MCTS) y *minimax* con la técnica de *poda de alfa-beta* [[2]](#Minimax). Además, como ejemplos para ver el correcto uso de la biblioteca, se han creado diferentes juegos de mesa, entre ellos, el *Tic-Tac-Toe* (3 en raya), el *Ultimate Tic-Tac-Toe* [[3]](#UltimateTicTacToe) y las *damas*.
+
+### Juegos de Información Imperfecta
+
+Para este segundo tipo de juegos se han implementado dos algoritmos, el *Single Observer Information Set Monte Carlo Tree Search (SO-ISMCTS)* [[4]](#ISMCTS) y el *Multiple Observer Information Set Monte Carlo Tree Search (MO-ISMCTS)* [[4]](#ISMCTS). El primero de estos algoritmos genera un único árbol desde el punto de vista del jugador al que le toca jugar. Por otro lado, el segundo algoritmo crea un árbol para cada uno de los jugadores y agrupa las acciones que son indiferenciables desde el punto de vista de este jugador, es decir, si un jugador puede realizar varios movimientos que no aportarían información a los rivales, agrupa estos movimientos como si fuesen uno solo, creando un único nodo en el árbol de los jugadores rivales.
+
+Un ejemplo serían los juegos en los que un jugador intercambia una de las cartas de su mano con cualquier carta de la baraja, cuando el jugador efectúa este intercambio los demás jugadores no reciben ningún tipo de información sobre el intercambio de cartas, por lo que su conocimiento sobre el estado del juego no cambia. 
+
+Para estos algoritmos también se han desarrollado varios juegos como ejemplos de uso de la biblioteca, aunque ambos algoritmos se pueden usar en todos los juegos de información imperfecta, se ha diferenciado entre juegos para el *SO-ISMCTS* y el *MO-ISMCTS*. Para el primer algoritmo se ha creado el juego de la *escoba*, el *Stratego* y el *blackJack*, y para el segundo se ha desarrollado el *holjjak* (juego de adivinar las canicas del rival) y el *phantom* (variante del 4 en raya en el que no se ven los movimientos del rival).
+
+## Manual de Uso
+El primer paso necesario para poder usar esta biblioteca es descargarla. Se puede descargar la biblioteca desde la consola usando el comando: 
+
+``` python
+pip install pyplAI
+```
+
+Tras esto, ya se puede importar en el archivo de *Python* del juego al que queramos implementarla.
+
+``` python
+import pyplAI
+```
+
+### Clase sobre el Estado del Juego
+Para poder usar esta biblioteca es imprescindible que haya una clase que guarde la información necesaria sobre el estado del juego. Aunque se puede dar a esta clase el nombre que se desee, en este manual se utilizará una clase llamada *Juego* a modo de ejemplo.
+
+``` python
+  class Juego:
+          .
+          .
+          .
+```
+
+### Atributo Obligatorio *jugadorActual*
+Debido a que los algoritmos necesitan saber cuál es el jugador al cual le toca jugar en cada uno de los turnos, es obligatorio añadir un atributo *jugadorActual* en la clase del juego. Además, es muy importante que este atributo tenga este mismo nombre.
+
+``` python
+  class Juego:
+    def __init__(self):
+        self.jugadorActual = 1
+                .
+                .
+                .
+```
+
+Este atributo debe contener un valor numérico que representa el índice del jugador al que le toca jugar (empezando por 1). También, debe ir actualizándose conforme se avanza en el juego, por ejemplo, en el *3 en raya*, este atributo se debe iniciar con el valor 1, pero cuando el primer jugador realice su movimiento, se actualiza al valor 2, indicando que el segundo jugador es el que debe realizar su jugada.
+
+Además del atributo para identificar el jugador actual del estado del juego, esta clase deberá implementar ciertos métodos para poder interactuar y obtener información sobre el estado del juego. Algunos métodos son comunes para todos los algoritmos, mientras que otros algoritmos requieren de métodos específicos. Cabe destacar que estos métodos pueden ser nombrados de forma distinta a como se mostrará a continuación, pero es totalmente necesario que reciban los parámetros de entrada y devuelvan la salida tal y como se especifica en este manual.
+
+### Métodos Generales
+
+Los siguientes 4 métodos serán obligatorios para todos los algoritmos que se implementan en esta biblioteca:
+
+**•	obtiene_movimientos(self):** Devolverá una lista con todos los movimientos posibles del jugador actual del estado del juego, es recomendable devolver estos movimientos en un orden aleatorio.
+
+``` python
+  class Juego:
+          .
+          .
+          .
+        def obtiene_movimientos(self):
+                    .
+                    .
+                    .
+            return movimientos
+```
+
+**•	aplica_movimiento(self, movimiento):** Aplicará el movimiento dado al estado del juego y devolverá el estado resultante (*self*).
+
+``` python
+  class Juego:
+          .
+          .
+          .
+        def aplica_movimiento(self, movimiento):
+                    .
+                    .
+                    .
+            return self
+```
+
+**•	es_estado_final(self):** Comprueba el estado actual del juego, devolviendo *True* o *False* dependiendo de si es un estado final o no.
+
+``` python
+  class Juego:
+          .
+          .
+          .
+        def es_estado_final(self):
+                    .
+                    .
+                    .
+            return True
+              o
+            return False
+```
+
+**•	gana_jugador(self, jugador):** Comprueba si el jugador dado gana el juego en el estado actual de este, devolviendo *True* en caso de que sea ganador, o *False* en caso contrario. La variable *jugador* debe ser un número entero positivo, y se debe situar en el rango de 1, para el primer jugador del juego, hasta *n*, siendo *n* el número total de jugadores.
+
+``` python
+  class Juego:
+          .
+          .
+          .
+        def gana_jugador(self, jugador):
+                    .
+                    .
+                    .
+            return True
+              o
+            return False
+```
+
+### Métodos SO/MO-ISMCTS
+
+Además de los 4 métodos anteriores, los algoritmos de *SO-ISMCTS* y *MO-ISMCTS* necesitan un método adicional para su uso, el cuál se explica a continuación:
+
+**•	determinación(self):** Devuelve una determinación aleatoria del estado del juego, desde el punto de vista del jugador actual.
+
+``` python
+  class Juego:
+          .
+          .
+          .
+        def determinacion(self):
+                    .
+                    .
+                    .
+            return determinacion
+```
+
+Por ejemplo, para un juego de cartas en el que cada jugador tiene una mano, hay una mesa con cartas visibles, una pila de descartes y un mazo de robo inicial, el jugador actual no tiene conocimiento sobre las cartas del rival ni las cartas del mazo de robo, pero si sabe cuáles son sus cartas, las de la mesa y las que han sido mandadas a la pila de descartes, por lo que tiene la información sobre cuáles son las cartas restantes, pero aún no sabe donde se encuentran. 
+
+Con esta información, este método debe dar un estado del juego en el que aleatoriamente se distribuyan las cartas que el jugador no tiene localizadas entre las zonas en las que no sabe que cartas hay, en este caso, las zonas serían las manos de los rivales y el mazo de robo.
+
+### Métodos MO-ISMCTS
+
+Además, para el funcionamiento del algoritmo *MO-ISMCTS* se necesitará otro método adicional:
+
+**•	es_movimiento_visible(movimiento):** Este método, dado un movimiento, devuelve *True* si es un movimiento visible para los rivales, o *False* en caso contrario.
+
+``` python
+  class Juego:
+          .
+          .
+          .
+        def es_movimiento_visible(movimiento):
+                    .
+                    .
+                    .
+            return True
+              o
+            return False
+```
+
+Por ejemplo, un movimiento visible para los rivales sería jugar una carta de tu mano sobre la mesa, por lo que, haría saber a los rivales el lugar exacto de esa carta, cosa que antes no sabían. Sin embargo, un movimiento no visible sería intercambiar una carta de tu mano con el mazo de robo sin revelar ninguna de las dos. Esta acción no mostraría nueva información a ningún rival, ya que no se muestran las cartas y los rivales seguirán sin saber que cartas hay en tu mano ni que cartas hay en el mazo.
+
+### Métodos Minimax
+
+En el caso del algoritmo de *minimax*, además de los 4 métodos generales, se necesita un método que devuelva una heurística sobre el estado del juego, es decir, que evalúe su estado para saber como de bueno es desde el punto de vista de un jugador dado:
+
+**•	heuristica(self, jugador):** Este método debe devolver un número entero que refleje una evaluación sobre como de bueno es el estado del juego para un jugador dado. Esta evaluación debe ser mayor cuanto mejor sea el estado del juego para este jugador.
+
+``` python
+  class Juego:
+          .
+          .
+          .
+        def heuristica(self, jugador):
+                    .
+                    .
+                    .
+            return evaluacion
+```
+
+Por ejemplo, para el juego de las *damas* una posible heurística sería contar el número de fichas del jugador y restarle el número de fichas del rival. Hay multitud de posibles heurísticas para cada uno de los juegos, y se debe tener un conocimiento sobre el juego para poder crear una buena heurística, ya que la heurística tendrá un gran peso a la hora de decidir cuál es el mejor movimiento.
+
+Al igual que en el método *gana_jugador*, el argumento *jugador* debe ser un número entero positivo, desde el 1, para el primer jugador, hasta *n*, para el último jugador, siendo *n* el número total de jugadores.
+
+### Constructor Algoritmo
+
+Una vez tengamos todos estos métodos solamente debemos llamar a la biblioteca y al constructor del algoritmo que se desee utilizar. A esta llamada le pasaremos como argumentos los métodos necesarios para el uso de este algoritmo junto con algunas otras variables que detallaremos a continuación:
+
+**•	numeroJugadores:** Este argumento es obligatorio para todos los algoritmos,  representará el número de jugadores que contiene el juego, siendo este un número entero mayor que cero.
+
+**•	tiempoEjecucion:** Este argumento es común para todos los algoritmos de Monte Carlo, ya que, estos algoritmos necesitan un tiempo límite de ejecución antes de devolver el mejor movimiento encontrado. Este argumento debe ser un número real mayor que cero y representa el tiempo de ejecución en segundos.
+
+**•	profundidadBusqueda:** Este argumento solo es necesario en la llamada al constructor del algoritmo de *minimax*, y sirve para limitar la profundidad en el árbol de búsqueda. Este argumento debe ser un número entero mayor que cero.
+
+Sabiendo todo esto ya podemos ver como se deben hacer las llamadas a la biblioteca y los constructores para cada uno de los tipos de algoritmos. Es muy importante que se siga el orden mostrado en los argumentos de entrada. Además, recordar que *Juego* es la clase de ejemplo que contiene la información sobre el estado del juego, como el atributo *jugadorActual*, y los métodos explicados anteriormente.
+
+**•	MCTS:**
+
+``` python
+  mcts = pyplAI.MCTS(
+         Juego.aplica_movimiento,
+         Juego.obtiene_movimientos, 
+         Juego.es_estado_final, 
+         Juego.gana_jugador, 
+         numeroJugadores, 
+         tiempoEjecucion)
+```
+
+**•	Minimax:**
+
+``` python
+  minimax = pyplAI.Minimax(
+           Juego.aplica_movimiento,
+           Juego.obtiene_movimientos, 
+           Juego.es_estado_final, 
+           Juego.gana_jugador, 
+           Juego.heuristica,
+           numeroJugadores, 
+           profundidadBusqueda)
+```
+
+**•	SO-ISMCTS:**
+
+``` python
+  so_ismcts = pyplAI.SOISMCTS(
+              Juego.aplica_movimiento,
+              Juego.obtiene_movimientos, 
+              Juego.es_estado_final, 
+              Juego.gana_jugador, 
+              Juego.determinacion,
+              numeroJugadores, 
+              tiempoEjecucion)
+```
+
+**•	MO-ISMCTS:**
+
+``` python
+  mo_ismcts = pyplAI.MOISMCTS(
+              Juego.aplica_movimiento,
+              Juego.obtiene_movimientos, 
+              Juego.es_estado_final, 
+              Juego.gana_jugador, 
+              Juego.determinacion,
+              Juego.es_movimiento_visible,
+              numeroJugadores, 
+              tiempoEjecucion)
+```
+
+**•	Modo *verbose*:**
+
+Si queremos ver algunos detalles cuando ejecutemos el algoritmo, se debe añadir un *True* como último argumento en la llamada al constructor. Este modo mostrará información útil del algoritmo por consola, como por ejemplo, tiempo de ejecución, número de nodos creados y visitados y demás características propias de cada uno de los algoritmos. Un ejemplo de como quedaría la creación del algoritmo de *MCTS* con este argumento extra sería el siguiente:
+
+``` python
+  mcts = pyplAI.MCTS(
+         Juego.aplica_movimiento,
+         Juego.obtiene_movimientos, 
+         Juego.es_estado_final, 
+         Juego.gana_jugador, 
+         numeroJugadores, 
+         tiempoEjecucion,
+         True)
+```
+
+### Ejecución Algoritmo
+
+Una vez tengamos el objeto del algoritmo que se quiere utilizar solamente se debe llamar a su método *ejecuta* y pasarle como argumento el objeto que contiene el estado actual del juego, esto devolverá el mejor movimiento encontrado durante el tiempo de computación dado, para los algoritmos de *Monte Carlo*, o la profundidad de búsqueda, en el caso del algoritmo *minimax*. A continuación, se mostrará el código de ejemplo en el que se usa el algoritmo de *MCTS* para obtener un movimiento y seguidamente aplicarlo al juego, obteniendo así un nuevo estado del juego:
+
+``` python
+  def main():
+      juego = Juego()
+      movimiento = mcts.ejecuta(juego)
+      juego = aplica_movimiento(movimiento)
+```
+
+
+En caso de que el estado del juego no tenga ningún movimiento posible para aplicar los algoritmos devolverán *None*, y si solo hay un posible movimiento para aplicar, para ahorrar cálculos innecesarios, se devolverá el único movimiento posible.
+
+Si se tienen dudas sobre como integrar la biblioteca a juegos propios se recomienda ver los juegos del repositorio de *GitHub* ([*pyplAI*](https://github.com/plss12/pyplAI)) como ejemplos de uso. Este repositorio contiene la biblioteca y todos los juegos nombrados en la introducción de este manual, incluyendo las implementaciones de los algoritmos correspondientes con cada uno de ellos.
+
+## Contacto
+
+En caso de tener alguna duda, idea o aportación sobre la biblioteca por favor contactar al siguiente correo: [pepoluis712@gmail.com](mailto:pepoluis712@gmail.com)
+
+## Referencias
+
+<a id="MCTS"></a>
+[1] Cameron B. Browne, Edward Powley, Daniel Whitehouse, Simon M. Lucas, Peter I.Cowling, Philipp Rohlfshagen, Stephen Tavener, Diego Perez, Spyridon Samoth-rakis, and Simon Colton. A survey of monte carlo tree search methods. IEEETransactions on Computational Intelligence and AI in Games, 4(1):1–43, 2012. doi:10.1109/TCIAIG.2012.2186810. URL https://ieeexplore.ieee.org/document/6145622.
+
+<a id="Minimax"></a>
+[2] Patricio Mendoza. Alpha-beta pruning algorithm: The intelligence behind strategygames. page 9, 2022. URL https://www.researchgate.net/publication/360872512.
+
+<a id="UltimateTicTacToe"></a>
+[3] Eytan Lifshitz and David Tsurel. Ai approaches to ultimate tic-tac-toe. page 5, 2013. URL https://www.cs.huji.ac.il/w~ai/projects/2013/UlitmateTic-Tac-Toe/files/report.pdf.
+
+<a id="ISMCTS"></a>
+[4] Peter I. Cowling, Edward J. Powley, and Daniel Whitehouse. Information setmonte carlo tree search. IEEE Transactions on Computational Intelligence and AIin Games, 4(2):120–143, 2012. doi: 10.1109/TCIAIG.2012.2200894. URL https://ieeexplore.ieee.org/document/6203567.
```

### Comparing `pyplAI-1.0.2/pyplAI/Algoritmos.py` & `pyplAI-1.0.3/pyplAI/Algoritmos.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from copy import deepcopy
 import time
 import math
 
 class MCTS:
     k = 1/math.sqrt(2) #Coeficiente de exploracion
 
-    def __init__(self, aplicar_movimiento, obtener_movimientos, es_estado_final, gana_jugador, numeroJugadores, tiempoEjecucion, estadisticas=True):
+    def __init__(self, aplicar_movimiento, obtener_movimientos, es_estado_final, gana_jugador, numeroJugadores, tiempoEjecucion, estadisticas=False):
         self.aplicar_movimiento = staticmethod(aplicar_movimiento)
         self.obtener_movimientos = staticmethod(obtener_movimientos)
         self.es_estado_final = staticmethod(es_estado_final)
         self.gana_jugador = staticmethod(gana_jugador)
         self.jugadores = [i+1 for i in range(numeroJugadores)]
         self.tiempoEjecucion = tiempoEjecucion
         self.estadisticas = estadisticas
@@ -132,15 +132,15 @@
             v.n = v.n+1
             #Incrementa la recompensa del nodo para cada jugador
             for jugador in jugadores:
                 v.q[jugadores.index(jugador)]+=delta[jugadores.index(jugador)]
             v = v.padre
 
 class Minimax:
-    def __init__(self, aplicar_movimiento, obtener_movimientos, es_estado_final, gana_jugador, heuristica, numeroJugadores, profundidadBusqueda, estadisticas=True):
+    def __init__(self, aplicar_movimiento, obtener_movimientos, es_estado_final, gana_jugador, heuristica, numeroJugadores, profundidadBusqueda, estadisticas=False):
         self.aplicar_movimiento = staticmethod(aplicar_movimiento)
         self.obtener_movimientos = staticmethod(obtener_movimientos)
         self.es_estado_final = staticmethod(es_estado_final)
         self.gana_jugador = staticmethod(gana_jugador)
         self.heuristica = staticmethod(heuristica)
         self.jugadores = [i+1 for i in range(numeroJugadores)]
         self.profundidadBusqueda = profundidadBusqueda
@@ -216,15 +216,15 @@
             print("\nTiempo de ejecución: ", time.time()-t0)
             print("Número de estados evaluados: ", estadosEvaluados)
         return mov
 
 class SOISMCTS:
     k = 1/math.sqrt(2) #Coeficiente de exploracion
 
-    def __init__(self, aplicar_movimiento, obtener_movimientos, es_estado_final, gana_jugador, determinization, numeroJugadores, tiempoEjecucion, estadisticas=True):
+    def __init__(self, aplicar_movimiento, obtener_movimientos, es_estado_final, gana_jugador, determinization, numeroJugadores, tiempoEjecucion, estadisticas=False):
         self.aplicar_movimiento = staticmethod(aplicar_movimiento)
         self.obtener_movimientos = staticmethod(obtener_movimientos)
         self.es_estado_final = staticmethod(es_estado_final)
         self.gana_jugador = staticmethod(gana_jugador)
         self.determinization = staticmethod(determinization)
         self.jugadores = [i+1 for i in range(numeroJugadores)]
         self.tiempoEjecucion = tiempoEjecucion
@@ -349,15 +349,15 @@
                 indiceJugador=jugadores.index(jugador)
                 v1.r[indiceJugador]+=r[indiceJugador]
             v1=v1.padre #El nodo actual es el nodo padre del nodo actual
 
 class MOISMCTS:
     k=1/math.sqrt(2)
 
-    def __init__(self, aplicar_movimiento, obtener_movimientos, es_estado_final, gana_jugador, determinization, accion_visible, numeroJugadores, tiempoEjecucion, estadisticas=True):
+    def __init__(self, aplicar_movimiento, obtener_movimientos, es_estado_final, gana_jugador, determinization, accion_visible, numeroJugadores, tiempoEjecucion, estadisticas=False):
         self.aplicar_movimiento = staticmethod(aplicar_movimiento)
         self.obtener_movimientos = staticmethod(obtener_movimientos)
         self.es_estado_final = staticmethod(es_estado_final)
         self.gana_jugador = staticmethod(gana_jugador)
         self.determinization = staticmethod(determinization)
         self.accion_visible = staticmethod(accion_visible)
         self.jugadores = [i+1 for i in range(numeroJugadores)]
```

### Comparing `pyplAI-1.0.2/pyplAI.egg-info/PKG-INFO` & `pyplAI-1.0.3/pyplAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplAI
-Version: 1.0.2
+Version: 1.0.3
 Summary: Biblioteca para Python con algoritmos de resolución de juegos de mesa (minimax, MCTS, SO-ISMCTS y MO-ISMCTS)
 Home-page: https://github.com/plss12/pyplAI
 Author: Pedro Luis Soto Santos
 Author-email: pepoluis712@gmail.com
 License: MIT
 Keywords: python,articial intelligence,AI,games,board games,minimax,alpha-beta,monte carlo,monte carlo tree search,UCT,game theory,information set,perfect information,imperfect information
 Classifier: Development Status :: 4 - Beta
@@ -22,36 +22,36 @@
 Classifier: Typing :: Typed
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # pyplAI
 
 ## Introducción
-Esta biblioteca para Python es el resultado final de un Trabajo de Fin de Grado centrado en la implementación de algoritmos de *Monte Carlo Tree Search* (MCTS) y *minimax* para diferentes tipos de juegos de mesa, entre ellos, según clasifica la teoría de juegos, los juegos de información perfecta, como lo son *el ajedrez* o *las damas*, en los que en todo momento cualquier jugador puede ver toda la información del juego, como los posibles movimientos del rival, y juegos de información imperfecta, como lo son la mayoría de juegos de cartas como por ejemplo *el Uno* o *la brisca*, en el que los jugadores solo conocen información propia, como sus cartas, o información general del juego, como el estado de la mesa, pero desconocen la información del rival, como las cartas de los demás jugadores.
+Esta biblioteca para *Python* es el resultado final de un Trabajo de Fin de Grado centrado en la implementación de algoritmos de *Monte Carlo Tree Search (MCTS)* y *minimax* para diferentes tipos de juegos de mesa, entre ellos, según clasifica la teoría de juegos, los juegos de información perfecta, como lo son el *ajedrez* o las *damas*, en los que en todo momento cualquier jugador puede ver toda la información del juego, como los posibles movimientos del rival, y juegos de información imperfecta, como lo son la mayoría de juegos de cartas como por ejemplo el *Uno* o la *brisca*, en el que los jugadores solo conocen información propia, como sus cartas, o información general del juego, como el estado de la mesa, pero desconocen la información del rival, como las cartas de los demás jugadores.
 
 ### Juegos de Información Perfecta
 
-Para este tipo de juegos se han implementado los algoritmos de MCTS con UCT [[1]](#MCTS) y minimax con la técnica de poda de alfa-beta [[2]](#Minimax). Además, como ejemplos para ver el correcto uso de la biblioteca, se han creado diferentes juegos de mesa, entre ellos, *TicTacToe* (3 en raya), *Ultimate TicTacToe* [[3]](#UltimateTicTacToe) y *las damas*.
+Para este tipo de juegos se han implementado los algoritmos de *MCTS con UCT* [[1]](#MCTS) y *minimax* con la técnica de *poda de alfa-beta* [[2]](#Minimax). Además, como ejemplos para ver el correcto uso de la biblioteca, se han creado diferentes juegos de mesa, entre ellos, el *Tic-Tac-Toe* (3 en raya), el *Ultimate Tic-Tac-Toe* [[3]](#UltimateTicTacToe) y las *damas*.
 
 ### Juegos de Información Imperfecta
 
-Para este segundo tipo de juegos se han implementado dos algoritmos, el *Single Observer Information Set Monte Carlo Tree Search* [[4]](#ISMCTS) (SO-ISMCTS) y el *Multiple Observer Information Set Monte Carlo Tree Search* [[4]](#ISMCTS) (MO-ISMCTS). El primero de estos algoritmos genera un único árbol desde el punto de vista del jugador al que le toca jugar. Por otro lado, el segundo algoritmo crea un árbol para cada uno de los jugadores y agrupa las acciones que son indiferenciables desde el punto de vista de este jugador, es decir, si un jugador puede realizar varios movimientos que no aportarían información a los rivales, agrupa estos movimientos como si fuesen uno solo, creando un único nodo en el árbol de los jugadores rivales.
+Para este segundo tipo de juegos se han implementado dos algoritmos, el *Single Observer Information Set Monte Carlo Tree Search (SO-ISMCTS)* [[4]](#ISMCTS) y el *Multiple Observer Information Set Monte Carlo Tree Search (MO-ISMCTS)* [[4]](#ISMCTS). El primero de estos algoritmos genera un único árbol desde el punto de vista del jugador al que le toca jugar. Por otro lado, el segundo algoritmo crea un árbol para cada uno de los jugadores y agrupa las acciones que son indiferenciables desde el punto de vista de este jugador, es decir, si un jugador puede realizar varios movimientos que no aportarían información a los rivales, agrupa estos movimientos como si fuesen uno solo, creando un único nodo en el árbol de los jugadores rivales.
 
 Un ejemplo serían los juegos en los que un jugador intercambia una de las cartas de su mano con cualquier carta de la baraja, cuando el jugador efectúa este intercambio los demás jugadores no reciben ningún tipo de información sobre el intercambio de cartas, por lo que su conocimiento sobre el estado del juego no cambia. 
 
-Para estos algoritmos también se han desarrollado varios juegos como ejemplos de uso de la biblioteca, aunque ambos algoritmos se pueden usar en todos los juegos de información imperfecta, se ha diferenciado entre juegos para el SO-ISMCTS y el MO-ISMCTS. Para el primer algoritmo se ha creado *el juego de la escoba*, *el Stratego* y *el blackJack*, y para el segundo se ha desarrollado *el holjjak* (juego de adivinar las canicas del rival) y *el phantom* (variante del 4 en raya en el que no se ven los movimientos del rival).
+Para estos algoritmos también se han desarrollado varios juegos como ejemplos de uso de la biblioteca, aunque ambos algoritmos se pueden usar en todos los juegos de información imperfecta, se ha diferenciado entre juegos para el *SO-ISMCTS* y el *MO-ISMCTS*. Para el primer algoritmo se ha creado el juego de la *escoba*, el *Stratego* y el *blackJack*, y para el segundo se ha desarrollado el *holjjak* (juego de adivinar las canicas del rival) y el *phantom* (variante del 4 en raya en el que no se ven los movimientos del rival).
 
 ## Manual de Uso
 El primer paso necesario para poder usar esta biblioteca es descargarla. Se puede descargar la biblioteca desde la consola usando el comando: 
 
 ``` python
 pip install pyplAI
 ```
 
-Tras esto, ya se puede importar en el archivo de Python del juego al que queramos implementarla.
+Tras esto, ya se puede importar en el archivo de *Python* del juego al que queramos implementarla.
 
 ``` python
 import pyplAI
 ```
 
 ### Clase sobre el Estado del Juego
 Para poder usar esta biblioteca es imprescindible que haya una clase que guarde la información necesaria sobre el estado del juego. Aunque se puede dar a esta clase el nombre que se desee, en este manual se utilizará una clase llamada *Juego* a modo de ejemplo.
@@ -201,15 +201,15 @@
         def heuristica(self, jugador):
                     .
                     .
                     .
             return evaluacion
 ```
 
-Por ejemplo, para el juego de *las damas* una posible heurística sería contar el número de fichas del jugador y restarle el número de fichas del rival. Hay multitud de posibles heurísticas para cada uno de los juegos, y se debe tener un conocimiento sobre el juego para poder crear una buena heurística, ya que la heurística tendrá un gran peso a la hora de decidir cuál es el mejor movimiento.
+Por ejemplo, para el juego de las *damas* una posible heurística sería contar el número de fichas del jugador y restarle el número de fichas del rival. Hay multitud de posibles heurísticas para cada uno de los juegos, y se debe tener un conocimiento sobre el juego para poder crear una buena heurística, ya que la heurística tendrá un gran peso a la hora de decidir cuál es el mejor movimiento.
 
 Al igual que en el método *gana_jugador*, el argumento *jugador* debe ser un número entero positivo, desde el 1, para el primer jugador, hasta *n*, para el último jugador, siendo *n* el número total de jugadores.
 
 ### Constructor Algoritmo
 
 Una vez tengamos todos estos métodos solamente debemos llamar a la biblioteca y al constructor del algoritmo que se desee utilizar. A esta llamada le pasaremos como argumentos los métodos necesarios para el uso de este algoritmo junto con algunas otras variables que detallaremos a continuación:
 
@@ -271,30 +271,30 @@
               Juego.es_movimiento_visible,
               numeroJugadores, 
               tiempoEjecucion)
 ```
 
 **•	Modo *verbose*:**
 
-Si queremos ver algunos detalles cuando ejecutemos el algoritmo, se debe añadir un *True* como último argumento en la llamada al constructor. Este modo mostrará información útil del algoritmo por consola, como por ejemplo, tiempo de ejecución, número de nodos creados y visitados y demás características propias de cada uno de los algoritmos. Un ejemplo de como quedaría la creación del algoritmo de MCTS con este argumento extra sería el siguiente:
+Si queremos ver algunos detalles cuando ejecutemos el algoritmo, se debe añadir un *True* como último argumento en la llamada al constructor. Este modo mostrará información útil del algoritmo por consola, como por ejemplo, tiempo de ejecución, número de nodos creados y visitados y demás características propias de cada uno de los algoritmos. Un ejemplo de como quedaría la creación del algoritmo de *MCTS* con este argumento extra sería el siguiente:
 
 ``` python
   mcts = pyplAI.MCTS(
          Juego.aplica_movimiento,
          Juego.obtiene_movimientos, 
          Juego.es_estado_final, 
          Juego.gana_jugador, 
          numeroJugadores, 
          tiempoEjecucion,
          True)
 ```
 
 ### Ejecución Algoritmo
 
-Una vez tengamos el objeto del algoritmo que se quiere utilizar solamente se debe llamar a su método *ejecuta* y pasarle como argumento el objeto que contiene el estado actual del juego, esto devolverá el mejor movimiento encontrado durante el tiempo de computación dado, para los algoritmos de *Monte Carlo*, o la profundidad de búsqueda, en el caso del algoritmo *minimax*. A continuación, se mostrará el código de ejemplo en el que se usa el algoritmo de *MCTS* para obtener un movimiento y seguidamente aplicarlo al juego, obtiendo así un nuevo estado del juego:
+Una vez tengamos el objeto del algoritmo que se quiere utilizar solamente se debe llamar a su método *ejecuta* y pasarle como argumento el objeto que contiene el estado actual del juego, esto devolverá el mejor movimiento encontrado durante el tiempo de computación dado, para los algoritmos de *Monte Carlo*, o la profundidad de búsqueda, en el caso del algoritmo *minimax*. A continuación, se mostrará el código de ejemplo en el que se usa el algoritmo de *MCTS* para obtener un movimiento y seguidamente aplicarlo al juego, obteniendo así un nuevo estado del juego:
 
 ``` python
   def main():
       juego = Juego()
       movimiento = mcts.ejecuta(juego)
       juego = aplica_movimiento(movimiento)
 ```
```

### Comparing `pyplAI-1.0.2/setup.py` & `pyplAI-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = "1.0.2"
+VERSION = "1.0.3"
 NAME = "pyplAI"
 DESCRIPTION = "Biblioteca para Python con algoritmos de resolución de juegos de mesa (minimax, MCTS, SO-ISMCTS y MO-ISMCTS)"
 LONG_DESCRIPTION = (HERE / "README.md").read_text(encoding='utf-8')
 LONG_DESC_TYPE = "text/markdown"
 
 AUTHOR = "Pedro Luis Soto Santos"
 EMAIL = "pepoluis712@gmail.com"
```

