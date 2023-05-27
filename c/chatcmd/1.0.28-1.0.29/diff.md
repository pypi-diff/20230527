# Comparing `tmp/chatcmd-1.0.28.tar.gz` & `tmp/chatcmd-1.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatcmd-1.0.28.tar", last modified: Sat May 27 21:33:47 2023, max compression
+gzip compressed data, was "chatcmd-1.0.29.tar", last modified: Sat May 27 21:53:47 2023, max compression
```

## Comparing `chatcmd-1.0.28.tar` & `chatcmd-1.0.29.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:33:47.577826 chatcmd-1.0.28/
--rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.28/LICENSE
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 21:33:47.577469 chatcmd-1.0.28/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-27 21:33:26.000000 chatcmd-1.0.28/README.md
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:33:47.574748 chatcmd-1.0.28/chatcmd/
--rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.28/chatcmd/__init__.py
--rw-r--r--   0 user       (501) staff       (20)     1760 2023-05-27 20:45:29.000000 chatcmd-1.0.28/chatcmd/api.py
--rw-r--r--   0 user       (501) staff       (20)     3464 2023-05-27 21:33:26.000000 chatcmd-1.0.28/chatcmd/chatcmd.py
--rw-r--r--   0 user       (501) staff       (20)     3754 2023-05-27 21:02:39.000000 chatcmd-1.0.28/chatcmd/commands.py
--rw-r--r--   0 user       (501) staff       (20)     2373 2023-05-27 21:05:11.000000 chatcmd-1.0.28/chatcmd/helpers.py
--rw-r--r--   0 user       (501) staff       (20)     2608 2023-05-27 21:33:26.000000 chatcmd-1.0.28/chatcmd/lookup.py
-drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:33:47.577022 chatcmd-1.0.28/chatcmd.egg-info/
--rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 21:33:47.000000 chatcmd-1.0.28/chatcmd.egg-info/PKG-INFO
--rw-r--r--   0 user       (501) staff       (20)      340 2023-05-27 21:33:47.000000 chatcmd-1.0.28/chatcmd.egg-info/SOURCES.txt
--rw-r--r--   0 user       (501) staff       (20)        1 2023-05-27 21:33:47.000000 chatcmd-1.0.28/chatcmd.egg-info/dependency_links.txt
--rw-r--r--   0 user       (501) staff       (20)       49 2023-05-27 21:33:47.000000 chatcmd-1.0.28/chatcmd.egg-info/entry_points.txt
--rw-r--r--   0 user       (501) staff       (20)       44 2023-05-27 21:33:47.000000 chatcmd-1.0.28/chatcmd.egg-info/requires.txt
--rw-r--r--   0 user       (501) staff       (20)        8 2023-05-27 21:33:47.000000 chatcmd-1.0.28/chatcmd.egg-info/top_level.txt
--rw-r--r--   0 user       (501) staff       (20)     1795 2023-05-27 21:33:26.000000 chatcmd-1.0.28/pyproject.toml
--rw-r--r--   0 user       (501) staff       (20)       38 2023-05-27 21:33:47.577911 chatcmd-1.0.28/setup.cfg
--rw-r--r--   0 user       (501) staff       (20)      556 2023-05-27 21:33:26.000000 chatcmd-1.0.28/setup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:53:47.731732 chatcmd-1.0.29/
+-rw-r--r--   0 user       (501) staff       (20)     1069 2023-05-15 17:18:35.000000 chatcmd-1.0.29/LICENSE
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 21:53:47.731485 chatcmd-1.0.29/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)     3972 2023-05-27 21:53:24.000000 chatcmd-1.0.29/README.md
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:53:47.728931 chatcmd-1.0.29/chatcmd/
+-rw-r--r--   0 user       (501) staff       (20)        0 2023-04-26 12:02:06.000000 chatcmd-1.0.29/chatcmd/__init__.py
+-rw-r--r--   0 user       (501) staff       (20)     1678 2023-05-27 21:44:19.000000 chatcmd-1.0.29/chatcmd/api.py
+-rw-r--r--   0 user       (501) staff       (20)     3410 2023-05-27 21:53:24.000000 chatcmd-1.0.29/chatcmd/chatcmd.py
+-rw-r--r--   0 user       (501) staff       (20)     3507 2023-05-27 21:48:02.000000 chatcmd-1.0.29/chatcmd/commands.py
+-rw-r--r--   0 user       (501) staff       (20)     1831 2023-05-27 21:45:32.000000 chatcmd-1.0.29/chatcmd/helpers.py
+-rw-r--r--   0 user       (501) staff       (20)     2518 2023-05-27 21:45:32.000000 chatcmd-1.0.29/chatcmd/lookup.py
+drwxr-xr-x   0 user       (501) staff       (20)        0 2023-05-27 21:53:47.731121 chatcmd-1.0.29/chatcmd.egg-info/
+-rw-r--r--   0 user       (501) staff       (20)     5594 2023-05-27 21:53:47.000000 chatcmd-1.0.29/chatcmd.egg-info/PKG-INFO
+-rw-r--r--   0 user       (501) staff       (20)      340 2023-05-27 21:53:47.000000 chatcmd-1.0.29/chatcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (501) staff       (20)        1 2023-05-27 21:53:47.000000 chatcmd-1.0.29/chatcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (501) staff       (20)       49 2023-05-27 21:53:47.000000 chatcmd-1.0.29/chatcmd.egg-info/entry_points.txt
+-rw-r--r--   0 user       (501) staff       (20)       44 2023-05-27 21:53:47.000000 chatcmd-1.0.29/chatcmd.egg-info/requires.txt
+-rw-r--r--   0 user       (501) staff       (20)        8 2023-05-27 21:53:47.000000 chatcmd-1.0.29/chatcmd.egg-info/top_level.txt
+-rw-r--r--   0 user       (501) staff       (20)     1795 2023-05-27 21:53:24.000000 chatcmd-1.0.29/pyproject.toml
+-rw-r--r--   0 user       (501) staff       (20)       38 2023-05-27 21:53:47.731809 chatcmd-1.0.29/setup.cfg
+-rw-r--r--   0 user       (501) staff       (20)      556 2023-05-27 21:53:24.000000 chatcmd-1.0.29/setup.py
```

### Comparing `chatcmd-1.0.28/LICENSE` & `chatcmd-1.0.29/LICENSE`

 * *Files identical despite different names*

### Comparing `chatcmd-1.0.28/PKG-INFO` & `chatcmd-1.0.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.28
+Version: 1.0.29
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT License
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
@@ -65,17 +65,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.28-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.29-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.28
+    Successfully installed chatcmd-1.0.29
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.28/README.md` & `chatcmd-1.0.29/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.28-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.29-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.28
+    Successfully installed chatcmd-1.0.29
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.28/chatcmd/api.py` & `chatcmd-1.0.29/chatcmd/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,37 +12,37 @@
         cursor.execute("SELECT api_key FROM config WHERE id = 1")
         api_key = cursor.fetchone()
         if api_key[0] is not None:
             if (validate_api_key(api_key[0])):
                 return api_key[0]
         return None
     except sqlite3.Error as e:
-        error_msg(f"Error 1003: Failed to get API key from database: {e}")
+        print(f"Error 1003: Failed to get API key from database: {e}")
         return None
 
 def output_api_key(conn, cursor):
     try:
         api_key = get_api_key(conn, cursor)
-        print("\n ChatGPT API key: "+color_text(api_key,'green')+"\n")
+        print("\n ChatGPT API key: "+api_key+"\n")
     except Exception as e:
-        error_msg(f"Error 1004: Failed to output API key: {e}")
+        print(f"Error 1004: Failed to output API key: {e}")
         return None
 
 def save_api_key(conn, cursor, api_key):
     try:
         cursor.execute("UPDATE config SET api_key = ? WHERE id = ?", (api_key,1))
         conn.commit()
         return True
     except sqlite3.Error as e:
-        error_msg(f"Error 1005: Failed to save API key to database: {e}")
+        print(f"Error 1005: Failed to save API key to database: {e}")
 
 def ask_for_api_key(conn, cursor):
     try:
         while True:
-            api_key = input(color_text("\nEnter a valid ChatGPT API key: ", 'green'))
+            api_key = input("\nEnter a valid ChatGPT API key: ")
             if (validate_api_key(api_key)):
                 if save_api_key(conn, cursor, api_key):
-                    print(color_text(f"\nChatGPT API Key updated successfully.\n",'green'))
+                    print("\nChatGPT API Key updated successfully.\n")
                     return api_key
-            error_msg('Error 1006: Invalid ChatGPT API key!')
+            print('Error 1006: Invalid ChatGPT API key!')
     except Exception as e:
-        error_msg(f"Error 1007: Failed asking for API key: {e}")
+        print(f"Error 1007: Failed asking for API key: {e}")
```

### Comparing `chatcmd-1.0.28/chatcmd/chatcmd.py` & `chatcmd-1.0.29/chatcmd/chatcmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,35 +42,35 @@
         args = docopt(__doc__)
         try:
             BASE_DIR = os.path.dirname(os.path.dirname(__file__))
             db_path = os.path.join(BASE_DIR, "chatcmd/db.sqlite")
             conn = sqlite3.connect(db_path)
             cursor = conn.cursor()
         except sqlite3.Error as e:
-            error_msg(f"Error 1002: Failed to connect to database: {e}")
+            print(f"Error 1002: Failed to connect to database: {e}")
 
         api_key = get_api_key(conn, cursor)
 
         if api_key is None:
             api_key = ask_for_api_key(conn, cursor)
 
         openai.api_key = api_key
 
         if args['--version']:
-            print(color_text('ChatCMD','green')+' 1.0.28')
+            print('ChatCMD'+' 1.0.29')
         elif args['--set-key']:
             ask_for_api_key(conn, cursor)
         elif args['--get-key']:
             output_api_key(conn, cursor)
         elif args['--get-cmd']:
             get_cmd(conn, cursor)
         elif args['--get-last']:
             get_last_num_cmd(conn, cursor, args['--get-last'])
         elif args['--cmd-total']:
-            print('\nTotal of ' + color_text(get_commands_count(conn, cursor), 'green') + ' commands\n')
+            print(f'\nTotal of {get_commands_count(conn, cursor)} commands\n')
         elif args['--delete-cmd']:
             delete_cmd(conn, cursor)
         elif args['--delete-last-cmd']:
             delete_last_num_cmd(conn, cursor, args['--delete-last-cmd'])
         elif args['--clear-history']:
             clear_history(conn, cursor)
         elif args['--db-size']:
@@ -79,12 +79,12 @@
             library_info()
         else:
             prompt(conn, cursor, api_key)
 
         cursor.close()
         conn.close()
     except Exception as e:
-        error_msg(f"Error 1001: {e}")
+        print(f"Error 1001: {e}")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `chatcmd-1.0.28/chatcmd/commands.py` & `chatcmd-1.0.29/chatcmd/commands.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,87 +9,87 @@
         conn.commit()
 
         cursor.execute("INSERT INTO history (prompt,command,created_at) VALUES(?,?,?)", (prompt, command, datetime.datetime.now()))
         conn.commit()
 
         return True
     except sqlite3.Error as e:
-        error_msg(f"Error 1012: Failed to add command to history: {e}")
+        print(f"Error 1012: Failed to add command to history: {e}")
     return False
 
 def get_cmd(conn, cursor):
     try:
         cursor.execute("SELECT prompt, command, created_at FROM history ORDER BY id DESC LIMIT 1")
         command = cursor.fetchone()
 
         if command is not None:
-            print("Latest Command:\n\n "+color_text(command[0],'white')+": "+color_text(command[1],'green')+"\n")
+            print("Latest Command:\n\n "+command[0]+": "+command[1]+"\n")
         else:
-            warning_msg("History is empty.")
+            print("History is empty.")
 
     except sqlite3.Error as e:
-        error_msg(f"Error 1013: Failed to get last command from history: {e}")
+        print(f"Error 1013: Failed to get last command from history: {e}")
 
 def get_last_num_cmd(conn, cursor, number):
     try:
         number = int(number)
         if number < 1:
-            warning_msg('History is empty.')
+            print('History is empty.')
         cursor.execute("SELECT prompt, command, created_at FROM history ORDER BY id DESC LIMIT ?", (number,))
         commands = cursor.fetchall()
         if len(commands) > 0:
             number = min(number, len(commands))
-            print(color_text('Latest Command:\n','white') if number == 1 else color_text(f'Last {number} Commands:\n','white'))
+            print('Latest Command:\n')
 
             for command in commands:
-                print(f'  - {color_text(command[1], "green")}')
+                print(f'  - {command[1]}')
         else:
-            warning_msg("History is empty.")
+            print("History is empty.")
         return True
     except ValueError as ve:
-        warning_msg(str(ve))
+        print(str(ve))
     except sqlite3.Error as e:
-        error_msg(f"Error 1014: Failed to get last command from history: {e}")
+        print(f"Error 1014: Failed to get last command from history: {e}")
     return False
 
 def delete_cmd(conn, cursor):
     try:
        cursor.execute("DELETE FROM history ORDER BY id DESC LIMIT 1")
        conn.commit()
-       success_msg("Command deleted successfully.")
+       print("Command deleted successfully.")
     except sqlite3.Error as e:
-        error_msg(f"Error 1015: Failed deleting last command: {e}")
+        print(f"Error 1015: Failed deleting last command: {e}")
     return False
 
 def delete_last_num_cmd(conn, cursor, number):
     try:
         if get_commands_count(conn,cursor) == 0:
-            warning_msg('History is empty.')
+            print('History is empty.')
         else:
             number = int(number)
             if number < 1:
-                error_msg('Please enter a correct number.')
+                print('Please enter a correct number.')
             else:
                 cursor.execute("DELETE FROM history ORDER BY id DESC LIMIT "+str(number))
                 delete = conn.commit()
                 if number > 1:
-                    success_msg("All "+str(number)+" commands deleted successfully")
+                    print("All "+str(number)+" commands deleted successfully")
                 else:
-                    success_msg("Command deleted successfully")
+                    print("Command deleted successfully")
     except sqlite3.Error as e:
-        error_msg(f"Error 1016: Failed to get last command from history: {e}")
+        print(f"Error 1016: Failed to get last command from history: {e}")
 
 def clear_history(conn, cursor):
     try:
         cursor.execute('DELETE FROM history')
         conn.commit()
-        print(color_text(f"\nAll command lookup has been cleared.",'green'))
+        print("\nAll command lookup has been cleared.")
         return True
     except sqlite3.Error as e:
-        error_msg(f"Error 1017: Failed clearing history: {e}")
+        print(f"Error 1017: Failed clearing history: {e}")
     return False
 
 def get_db_size(db_path):
     file_size_bytes = os.path.getsize(db_path)
     units = ['bytes', 'KB', 'MB', 'GB']
     size = file_size_bytes
     unit_index = 0
```

### Comparing `chatcmd-1.0.28/chatcmd/helpers.py` & `chatcmd-1.0.29/chatcmd/helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,37 +18,14 @@
     "  License: MIT\n"
     "  Author: Naif Alshaye\n"
     "  Author Email: naif@naif.io\n"
     "  Author Website: https://naif.io\n"
     "----------------------------------------------------------------"
     )
 
-def color_text(text, color):
-    colors = {
-        'red': Fore.RED,
-        'green': Fore.GREEN,
-        'yellow': Fore.YELLOW,
-        'blue': Fore.BLUE,
-        'magenta':Fore.MAGENTA,
-        'cyan': Fore.CYAN,
-        'white':Fore.WHITE,
-        'black':Fore.BLACK,
-    }
-
-    return f"{colors[color]}{text}" + Style.RESET_ALL
-
-def success_msg(text):
-    print("\n"+color_text(text, 'green'))
-
-def error_msg(text):
-    print("\n"+color_text(text, 'red'))
-    exit()
-
-def warning_msg(text):
-    print("\n"+color_text(text, 'yellow'))
 
 def clear_input(input):
     input = re.sub('[^a-zA-Z0-9 -_=]', '', input.strip())
     return input
 
 def validateInput(prompt):
     if len(prompt.split()) <= 2:
@@ -70,12 +47,12 @@
         if system == 'Darwin':  # macOS
             subprocess.run(['pbcopy'], input=text, encoding='utf-8')
         elif system == 'Linux':  # Linux
             subprocess.run(['xclip', '-selection', 'clipboard'], input=text, encoding='utf-8')
         elif system == 'Windows':  # Windows
             subprocess.run(['clip'], input=text, encoding='utf-8', shell=True)
     except Exception as e:
-        error_msg("Error 1018: Failed to copy command. "+str(e))
+        print("Error 1018: Failed to copy command. "+str(e))
 
 def get_line_number():
     frame = inspect.currentframe().f_back
     return frame.f_lineno
```

### Comparing `chatcmd-1.0.28/chatcmd/lookup.py` & `chatcmd-1.0.29/chatcmd/lookup.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,44 +10,44 @@
     ##       ######### ##     ##    ##    ##       ## ### ## ##     ##
     ##       ##     ## #########    ##    ##       ##     ## ##     ##
     ##    ## ##     ## ##     ##    ##    ##    ## ##     ## ##     ##
      ######  ##     ## ##     ##    ##     ######  ##     ## ########
 
     """)
     if validate_api_key(api_key) is False:
-        error_msg("Error 1009: API key is invalid or missing")
+        print("Error 1009: API key is invalid or missing")
     prompt = clear_input(input("Prompt: "))
 
     if prompt == '':
         prompt(conn, cursor, api_key)
     if prompt == 'exit':
-        print(color_text('bye...', 'green'))
+        print('bye...')
         exit()
     elif validateInput(prompt):
         command = lookup(prompt, api_key)
         if command is not None:
             copy_to_clipboard(command)
             command = clear_input(command)
 
             if command.find('there is no command') is True and command.find('There is no specific command') is True:
-                warning_msg('there is no command for this!')
+                print('there is no command for this!')
             else:
                 history = add_cmd(conn, cursor, prompt, command.strip())
                 if history is False:
-                    print(color_text("Error 1008 Failed to add command to history", 'cyan'))
-                print(color_text(" " + command.strip(), 'green'))
+                    print("Error 1008 Failed to add command to history")
+                print(" " + command.strip())
                 print('')
     else:
-        warning_msg("Please type in more than two words.\n")
+        print("Please type in more than two words.\n")
 
 
 def lookup(prompt, api_key):
     try:
         if validate_api_key(api_key) is False:
-            error_msg("Error 1009: API key is invalid or missing")
+            print("Error 1009: API key is invalid or missing")
             exit()
 
         prompt = prompt
         print("Looking up...\n")
 
         stop_keywords = ["###", "END", "stop", "Command:", "Syntax:", "Usage:","The command to install MySQL on Windows is:"]
         response = openai.Completion.create(
@@ -57,10 +57,10 @@
             n=1,
             stop=None,
             temperature=0.7)
         message = response.choices[0].text.strip()
         return message
 
     except openai.error.OpenAIError as e:
-        error_msg(f"Error 1010: OpenAI API error occurred: {e}")
+        print(f"Error 1010: OpenAI API error occurred: {e}")
     except Exception as e:
-        error_msg(f"Error 1011: Unhandled exception occurred: {e}")
+        print(f"Error 1011: Unhandled exception occurred: {e}")
```

### Comparing `chatcmd-1.0.28/chatcmd.egg-info/PKG-INFO` & `chatcmd-1.0.29/chatcmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatcmd
-Version: 1.0.28
+Version: 1.0.29
 Summary: ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.
 Home-page: https://github.com/naifalshaye/chatcmd
 Author: Naif Alshaye
 Author-email: Naif Alshaye <naif@naif.io>
 License: MIT License
 Project-URL: Homepage, https://github.com/naifalshaye/chatcmd
 Project-URL: Documentation, https://github.com/naifalshaye/chatcmd/blob/master/README.md
@@ -65,17 +65,17 @@
 If pip not installed:
 
     python3 -m pip install chatcmd
 
 Installation output should display:
 
     Collecting chatcmd
-    Using cached chatcmd-1.0.28-py3-none-any.whl (6.8 kB)
+    Using cached chatcmd-1.0.29-py3-none-any.whl (6.8 kB)
     Installing collected packages: chatcmd
-    Successfully installed chatcmd-1.0.28
+    Successfully installed chatcmd-1.0.29
 
 ### Uninstall ###
     pip3 uninstall chatcmd
 
 If pip not installed:
 
     python3 -m pip uninstall chatcmd
```

### Comparing `chatcmd-1.0.28/pyproject.toml` & `chatcmd-1.0.29/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel >= 0.38",
     "colorama >=0.4.6"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatcmd"
-version = "1.0.28"
+version = "1.0.29"
 description = "ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input."
 authors = [
     { name = "Naif Alshaye", email = "naif@naif.io" }
 ]
 license = {text = "MIT License"}
 readme = "README.md"
 requires-python = ">=3.7.1"
```

### Comparing `chatcmd-1.0.28/setup.py` & `chatcmd-1.0.29/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name="chatcmd",
-    version="1.0.28",
+    version="1.0.29",
     description="ChatCMD is an AI-driven CLI-based command lookup using ChatGPT to lookup relevant CLI commands based on user input.",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Naif Alshaye",
     author_email="naif@naif.io",
     url="https://github.com/naifalshaye/chatcmd",
     install_requires=[
```

