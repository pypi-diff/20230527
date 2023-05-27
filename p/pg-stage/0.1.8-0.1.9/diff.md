# Comparing `tmp/pg_stage-0.1.8.tar.gz` & `tmp/pg_stage-0.1.9.tar.gz`

## Comparing `pg_stage-0.1.8.tar` & `pg_stage-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pg_stage-0.1.8/requirements.txt
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 pg_stage-0.1.8/setup.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pg_stage-0.1.8/.github/workflows/bandit.yml
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pg_stage-0.1.8/.github/workflows/black.yml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 pg_stage-0.1.8/.github/workflows/pytest.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pg_stage-0.1.8/.idea/.gitignore
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pg_stage-0.1.8/.idea/misc.xml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pg_stage-0.1.8/.idea/modules.xml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pg_stage-0.1.8/.idea/pg_stage.iml
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pg_stage-0.1.8/.idea/vcs.xml
--rw-r--r--   0        0        0    22083 2020-02-02 00:00:00.000000 pg_stage-0.1.8/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pg_stage-0.1.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pg_stage-0.1.8/src/pg_stage/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 pg_stage-0.1.8/src/pg_stage/mutator.py
--rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 pg_stage-0.1.8/src/pg_stage/obfuscator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pg_stage-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pg_stage-0.1.8/tests/conftest.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 pg_stage-0.1.8/tests/test_parse_comment_column.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 pg_stage-0.1.8/tests/test_parse_comment_table.py
--rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 pg_stage-0.1.8/tests/test_parse_copy_values.py
--rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 pg_stage-0.1.8/tests/test_prepared_data.py
--rw-r--r--   0        0        0    13862 2020-02-02 00:00:00.000000 pg_stage-0.1.8/tests/sql/example_dump.sql
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 pg_stage-0.1.8/tests/sql/test_parse_copy_values_with_delete_tables.sql
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 pg_stage-0.1.8/tests/sql/test_parse_copy_values_with_mutation.sql
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pg_stage-0.1.8/tests/sql/test_parse_copy_values_with_relations.sql
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 pg_stage-0.1.8/tests/sql/test_parse_copy_values_with_self_relation.sql
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pg_stage-0.1.8/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pg_stage-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 pg_stage-0.1.8/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pg_stage-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 pg_stage-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 pg_stage-0.1.9/requirements.txt
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 pg_stage-0.1.9/setup.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pg_stage-0.1.9/.github/workflows/bandit.yml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pg_stage-0.1.9/.github/workflows/black.yml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 pg_stage-0.1.9/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pg_stage-0.1.9/.idea/.gitignore
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 pg_stage-0.1.9/.idea/misc.xml
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 pg_stage-0.1.9/.idea/modules.xml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 pg_stage-0.1.9/.idea/pg_stage.iml
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 pg_stage-0.1.9/.idea/vcs.xml
+-rw-r--r--   0        0        0    23729 2020-02-02 00:00:00.000000 pg_stage-0.1.9/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pg_stage-0.1.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pg_stage-0.1.9/src/pg_stage/__init__.py
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 pg_stage-0.1.9/src/pg_stage/mutator.py
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 pg_stage-0.1.9/src/pg_stage/obfuscator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pg_stage-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 pg_stage-0.1.9/tests/conftest.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 pg_stage-0.1.9/tests/test_parse_comment_column.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 pg_stage-0.1.9/tests/test_parse_comment_table.py
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 pg_stage-0.1.9/tests/test_parse_copy_values.py
+-rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 pg_stage-0.1.9/tests/test_prepared_data.py
+-rw-r--r--   0        0        0    13862 2020-02-02 00:00:00.000000 pg_stage-0.1.9/tests/sql/example_dump.sql
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 pg_stage-0.1.9/tests/sql/test_parse_copy_values_with_delete_tables.sql
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 pg_stage-0.1.9/tests/sql/test_parse_copy_values_with_mutation.sql
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pg_stage-0.1.9/tests/sql/test_parse_copy_values_with_relations.sql
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 pg_stage-0.1.9/tests/sql/test_parse_copy_values_with_self_relation.sql
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 pg_stage-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pg_stage-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 pg_stage-0.1.9/README.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 pg_stage-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 pg_stage-0.1.9/PKG-INFO
```

### Comparing `pg_stage-0.1.8/.idea/pg_stage.iml` & `pg_stage-0.1.9/.idea/pg_stage.iml`

 * *Files identical despite different names*

### Comparing `pg_stage-0.1.8/.idea/workspace.xml` & `pg_stage-0.1.9/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `pg_stage-0.1.8/.idea/workspace.xml` & `pg_stage-0.1.9/.idea/workspace.xml`

```diff
@@ -1,24 +1,32 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
-    <list default="true" id="48822be1-252d-44d5-bbe2-003f83f80c12" name="Default Changelist" comment="Change method"/>
+    <list default="true" id="48822be1-252d-44d5-bbe2-003f83f80c12" name="Default Changelist" comment="Fix bandit">
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/setup.py" beforeDir="false" afterPath="$PROJECT_DIR$/setup.py" afterDir="false"/>
+    </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
     <option name="RECENT_TEMPLATES">
       <list>
         <option value="Python Script"/>
       </list>
     </option>
   </component>
   <component name="Git.Settings">
+    <option name="RECENT_BRANCH_BY_REPOSITORY">
+      <map>
+        <entry key="$PROJECT_DIR$" value="main"/>
+      </map>
+    </option>
     <option name="RECENT_GIT_ROOT_PATH" value="$PROJECT_DIR$"/>
   </component>
   <component name="GitSEFilterConfiguration">
     <file-type-list>
       <filtered-out-file-type name="LOCAL_BRANCH"/>
       <filtered-out-file-type name="REMOTE_BRANCH"/>
       <filtered-out-file-type name="TAG"/>
@@ -101,14 +109,15 @@
       <workItem from="1675061024756" duration="7075000"/>
       <workItem from="1675083920542" duration="1029000"/>
       <workItem from="1675086408073" duration="7403000"/>
       <workItem from="1675137158346" duration="9511000"/>
       <workItem from="1675173014453" duration="839000"/>
       <workItem from="1675223118425" duration="18325000"/>
       <workItem from="1675356667998" duration="2703000"/>
+      <workItem from="1675428237860" duration="3900000"/>
     </task>
     <task id="LOCAL-00001" summary="Init repo">
       <created>1675061774071</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1675061774072</updated>
@@ -417,15 +426,43 @@
     <task id="LOCAL-00045" summary="Change method">
       <created>1675358711006</created>
       <option name="number" value="00045"/>
       <option name="presentableId" value="LOCAL-00045"/>
       <option name="project" value="LOCAL"/>
       <updated>1675358711006</updated>
     </task>
-    <option name="localTasksCounter" value="46"/>
+    <task id="LOCAL-00046" summary="Update version on 0.1.8">
+      <created>1675428411286</created>
+      <option name="number" value="00046"/>
+      <option name="presentableId" value="LOCAL-00046"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1675428411286</updated>
+    </task>
+    <task id="LOCAL-00047" summary="Added new mutation">
+      <created>1675442645327</created>
+      <option name="number" value="00047"/>
+      <option name="presentableId" value="LOCAL-00047"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1675442645327</updated>
+    </task>
+    <task id="LOCAL-00048" summary="Fix tests">
+      <created>1675443185217</created>
+      <option name="number" value="00048"/>
+      <option name="presentableId" value="LOCAL-00048"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1675443185217</updated>
+    </task>
+    <task id="LOCAL-00049" summary="Fix bandit">
+      <created>1675443228980</created>
+      <option name="number" value="00049"/>
+      <option name="presentableId" value="LOCAL-00049"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1675443228980</updated>
+    </task>
+    <option name="localTasksCounter" value="50"/>
     <servers/>
   </component>
   <component name="TypeScriptGeneratedFilesManager">
     <option name="version" value="3"/>
   </component>
   <component name="Vcs.Log.Tabs.Properties">
     <option name="TAB_STATES">
@@ -436,40 +473,40 @@
           </value>
         </entry>
       </map>
     </option>
     <option name="oldMeFiltersMigrated" value="true"/>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="Change image"/>
-    <MESSAGE value="Change command"/>
     <MESSAGE value="Added black in action"/>
     <MESSAGE value="Added pyproject toml"/>
     <MESSAGE value="Refactoring code by black"/>
     <MESSAGE value="Added bandit action"/>
     <MESSAGE value="Mock bandit"/>
     <MESSAGE value="Added new test for relations"/>
     <MESSAGE value="Added new mutator for uri"/>
     <MESSAGE value="Added info for pypi"/>
     <MESSAGE value="Added setup.py"/>
     <MESSAGE value="Fix action tests"/>
     <MESSAGE value="Fix setup.py"/>
     <MESSAGE value="Exclude tests from packages"/>
-    <MESSAGE value="Fix tests"/>
     <MESSAGE value="Change version and dependencies"/>
     <MESSAGE value="Fix missing in mutator"/>
     <MESSAGE value="Update version"/>
     <MESSAGE value="Added new test and mutations"/>
-    <MESSAGE value="Fix bandit"/>
     <MESSAGE value="Added readme and update version"/>
     <MESSAGE value="Added delete_tables_by_pattern"/>
     <MESSAGE value="Fix black"/>
     <MESSAGE value="Added new test"/>
     <MESSAGE value="Change method"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Change method"/>
+    <MESSAGE value="Update version on 0.1.8"/>
+    <MESSAGE value="Added new mutation"/>
+    <MESSAGE value="Fix tests"/>
+    <MESSAGE value="Fix bandit"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Fix bandit"/>
   </component>
   <component name="XDebuggerManager">
     <watches-manager>
       <configuration name="tests">
         <watch expression="f'COMMENT ON COLUMN {table_name}.{column_name} IS \'anon: {&quot;mutation_name&quot;: &quot;null&quot;}\''" language="Python"/>
         <watch expression="f'COMMENT ON COLUMN {table_name}.{column_name}' + ' IS \'anon: {&quot;mutation_name&quot;: &quot;null&quot;}\''" language="Python"/>
         <watch expression="result.group(2)" language="Python"/>
@@ -481,10 +518,10 @@
         <watch expression="result" language="Python"/>
         <watch expression="{line for line in result if '20f654fe-b27d-4051-9fd4-000000000001' in line and '111n' not in line}" language="Python"/>
       </configuration>
     </watches-manager>
   </component>
   <component name="com.intellij.coverage.CoverageDataManagerImpl">
     <SUITE FILE_PATH="coverage/pg_stage$main.coverage" NAME="main Coverage Results" MODIFIED="1675238408472" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$"/>
-    <SUITE FILE_PATH="coverage/pg_stage$pytest.coverage" NAME="pytest Coverage Results" MODIFIED="1675357843349" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/"/>
+    <SUITE FILE_PATH="coverage/pg_stage$pytest.coverage" NAME="pytest Coverage Results" MODIFIED="1675443172902" SOURCE_PROVIDER="com.intellij.coverage.DefaultCoverageFileProvider" RUNNER="coverage.py" COVERAGE_BY_TEST_ENABLED="true" COVERAGE_TRACING_ENABLED="false" WORKING_DIRECTORY="$PROJECT_DIR$/"/>
   </component>
 </project>
```

### Comparing `pg_stage-0.1.8/src/pg_stage/mutator.py` & `pg_stage-0.1.9/src/pg_stage/mutator.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,22 @@
     def mutation_empty_string(**_) -> str:
         """
         Метод для создания пустой строки
         :return: пустая строка
         """
         return ''
 
+    @staticmethod
+    def mutation_fixed_value(**kwargs) -> str:
+        """
+        Метод для вставки значения из параметров
+        :return: строка со значением
+        """
+        return str(kwargs.get('value', ''))
+
     def mutation_first_name(self, **_) -> str:
         """
         Метод для формирования фамилии
         :return:
         """
         return self._faker.first_name()
```

### Comparing `pg_stage-0.1.8/src/pg_stage/obfuscator.py` & `pg_stage-0.1.9/src/pg_stage/obfuscator.py`

 * *Files identical despite different names*

### Comparing `pg_stage-0.1.8/tests/test_parse_comment_column.py` & `pg_stage-0.1.9/tests/test_parse_comment_column.py`

 * *Files identical despite different names*

### Comparing `pg_stage-0.1.8/tests/test_parse_comment_table.py` & `pg_stage-0.1.9/tests/test_parse_comment_table.py`

 * *Files identical despite different names*

### Comparing `pg_stage-0.1.8/tests/test_parse_copy_values.py` & `pg_stage-0.1.9/tests/test_parse_copy_values.py`

 * *Files identical despite different names*

### Comparing `pg_stage-0.1.8/tests/test_prepared_data.py` & `pg_stage-0.1.9/tests/test_prepared_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,29 +47,33 @@
         '06fa5d0f3a4d62ff60717ff3315301129a5bcd152f63f073b67d2e6a835b098524b1d097367283c97ca75db9154cf61d6a918248e'
         'b68eaf8cd83d1a87cdd92dc',
         '02cbd8d1e9690c7786375f9f6ec4da6fa3c2ead70d41a7aa1d7fe631477b42635210f0e8fa7579f6f4b5afdb364d9465623a2861e'
         'cff75fa3a052c9b2a9fc2dd',
         'b09909b6e83938dd41ffb5e931eeb3d646b1856dfb74a81acb1697b6d8466468047fe92286e011a4634c71b8d8775c7d5a31e19ce'
         '111bd31d0a61a4faf93d6af',
     }
+    crypted_password = (  # nosec
+        '400$8$4c$c11df6facaefc6bc$93a657fb3c6e4cd1fd3125d3bd1ett18ffc4a8092e2616b9e5ca7954b2c52504'
+    )
     password_salts = {
         'v8BMktHnOeokEBTy6As',
         'c5d6v3NS97D3wYkUltFQ',
         '2IcBeSh6IVVCJyZpqBt',
         'QOqWQ24CMiRNuPUz8f5',
         'uMYA6c3A7uGoI0aEbJ8R',
     }
 
     for line in dump_sql.splitlines():
         new_line = obfuscator_object._parse_line(line=line)
-        if new_line is not None:
+        if new_line and 'COPY' not in new_line and 'COMMENT' not in new_line and '\\.' not in line:
             assert not any([email in new_line for email in emails])  # nosec
             assert not any([birthday in new_line for birthday in birthdays])  # nosec
             assert not any([token in new_line for token in tokens])  # nosec
             assert not any([password_salt in new_line for password_salt in password_salts])  # nosec
+            assert crypted_password in new_line  # nosec
 
 
 def test_parse_copy_values_with_relations(obfuscator_object: Obfuscator):
     """
     Arrange: Дамп таблиц, в которых необходимо мутировать одно связанное поле
     Act: Вызов функции `_parse_line` класса Obfuscator
     Assert: В stdout данные поле мутировано во всех таблицах одинаково и не задета таблица с похожими данными
```

### Comparing `pg_stage-0.1.8/tests/sql/example_dump.sql` & `pg_stage-0.1.9/tests/sql/example_dump.sql`

 * *Files identical despite different names*

### Comparing `pg_stage-0.1.8/tests/sql/test_parse_copy_values_with_delete_tables.sql` & `pg_stage-0.1.9/tests/sql/test_parse_copy_values_with_delete_tables.sql`

 * *Files identical despite different names*

### Comparing `pg_stage-0.1.8/tests/sql/test_parse_copy_values_with_mutation.sql` & `pg_stage-0.1.9/tests/sql/test_parse_copy_values_with_mutation.sql`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 COMMENT ON COLUMN table_1.persistence_token IS 'anon: {"mutation_name": "empty_string"}';
+COMMENT ON COLUMN table_1.crypted_password IS 'anon: {"mutation_name": "fixed_value", "mutation_kwargs": {"value": "400$8$4c$c11df6facaefc6bc$93a657fb3c6e4cd1fd3125d3bd1ett18ffc4a8092e2616b9e5ca7954b2c52504"}}';
 
 COPY table_1 (id, crypted_password, persistence_token, created_at, updated_at, active, first_name, last_name, agency_id, phone, perishable_token, extension, commissioned, region, division, location, last_request_at) FROM stdin;
 07750c56-fb37-46e1-b7b6-da530704c056	400$8$4c$c11df6facaefc6bc$93a657fb3c6e4cd1fd3255d3bd1edd18ffc4a8092e2616b9e5ca7954b2c52504	86a97ff982e87ed5af7d90ab2ce31d4e89a3af3e6a0490b067bb8213aea7a4ee0eeafae1d8fe3c6f990aead095092fcf852004b18e484ef22569aebf64c3747f	2016-06-03 18:23:06.25685	2016-06-03 18:23:06.25685	t	C.J.	Cregg	\N	1231231234	hw1rFSX7yJBz65lDVzYi	\N	f	\N	\N	\N	\N
 d489bda7-3212-4026-aef9-879d3242ad0c	400$8$50$5555852e67bf920f$161b41afd99159609151f22fbc4efdccb925244606a87fc635954a71e8f7606f	630aaf10f3edcb396181535476bccfd369e1ee9281cbc218d0861e6117b9839219cb403abed3b59468b2564c229d78b0cb610d0e16fa4a03dc4d93ed3d55deb3	2016-06-03 18:23:06.417694	2016-06-03 18:23:06.417694	t	Leo	McGarry	\N	1231231234	ojbfkdLiQOOHvqxuTsg	\N	f	\N	\N	\N	\N
 ab344f75-d78a-47ba-a4f7-121275b3b241	400$8$4a$fb1a833f95079502$8b6ddd327381860e18bce53ee1a3249d5237de4f4344c06ad940ba8cfc6a2259	06fa5d0f3a4d62ff60717ff3315301129a5bcd152f63f073b67d2e6a835b098524b1d097367283c97ca75db9154cf61d6a918248eb68eaf8cd83d1a87cdd92dc	2016-06-03 18:23:06.563866	2016-06-03 18:23:06.563866	t	Donna	Moss	\N	1231231234	p8MikeuBbbbFZ2i7V1gT	\N	f	\N	\N	\N	\N
 f7bd4a7f-b63f-41c3-83bd-9683f33bb4b3	400$8$50$8368e20d878ef1b1$b271e3af024b424b7256592439a35d6eb224b4dc769ac9f2fa564b282efb8a47	02cbd8d1e9690c7786375f9f6ec4da6fa3c2ead70d41a7aa1d7fe631477b42635210f0e8fa7579f6f4b5afdb364d9465623a2861ecff75fa3a052c9b2a9fc2dd	2016-06-03 18:23:06.739671	2016-06-03 18:23:06.739671	t	Charlie	Young	\N	1231231234	rkU7yVplV5FMsoJFDkaM	\N	f	\N	\N	\N	\N
 abe9fd39-f0b3-4ec6-9006-9783fbdade07	400$8$50$ef1eb813f8d8b99d$2932a9dc75d10f13525e43c29726061d99b4ebdff2e9f9951eb6e2393f36d221	b09909b6e83938dd41ffb5e931eeb3d646b1856dfb74a81acb1697b6d8466468047fe92286e011a4634c71b8d8775c7d5a31e19ce111bd31d0a61a4faf93d6af	2016-06-03 18:23:05.797143	2016-06-07 21:53:45.149755	t	Fun	Buyer	5030cc27-e7a8-4768-b355-20cdcf9efc53	1112223333	8npwjv7m8NmCTT9eZdIK	\N	f	\N	\N	\N	2016-06-07 21:53:45.148823
 \.
 
 COMMENT ON COLUMN schema.table_1.email IS 'anon: {"mutation_name": "email"}';
 COMMENT ON COLUMN schema.table_1.password_salt IS 'anon: {"mutation_name": "null"}';
 COMMENT ON COLUMN schema.table_1.dt_birthday IS 'anon: {"mutation_name": "past_date"}';
+COMMENT ON COLUMN schema.table_1.crypted_password IS 'anon: {"mutation_name": "fixed_value", "mutation_kwargs": {"value": "400$8$4c$c11df6facaefc6bc$93a657fb3c6e4cd1fd3125d3bd1ett18ffc4a8092e2616b9e5ca7954b2c52504"}}';
 
 COPY schema.table_1 (id, email, crypted_password, password_salt, created_at, updated_at, active, first_name, last_name, dt_birthday, agency_id, phone, perishable_token, extension, commissioned, region, division, location, last_request_at) FROM stdin;
 07750c56-fb37-46e1-b7b6-da530704c056	cj@example.com	400$8$4c$c11df6facaefc6bc$93a657fb3c6e4cd1fd3255d3bd1edd18ffc4a8092e2616b9e5ca7954b2c52504	v8BMktHnOeokEBTy6As	2016-06-03 18:23:06.25685	2016-06-03 18:23:06.25685	t	C.J.	Cregg	1996-10-02	\N	1231231234	hw1rFSX7yJBz65lDVzYi	\N	f	\N	\N	\N	\N
 d489bda7-3212-4026-aef9-879d3242ad0c	leo@example.com	400$8$50$5555852e67bf920f$161b41afd99159609151f22fbc4efdccb925244606a87fc635954a71e8f7606f	c5d6v3NS97D3wYkUltFQ	2016-06-03 18:23:06.417694	2016-06-03 18:23:06.417694	t	Leo	McGarry	1996-10-03	\N	1231231234	ojbfkdLiQOOHvqxuTsg	\N	f	\N	\N	\N	\N
 ab344f75-d78a-47ba-a4f7-121275b3b241	donna@example.com	400$8$4a$fb1a833f95079502$8b6ddd327381860e18bce53ee1a3249d5237de4f4344c06ad940ba8cfc6a2259	2IcBeSh6IVVCJyZpqBt	2016-06-03 18:23:06.563866	2016-06-03 18:23:06.563866	t	Donna	Moss	2005-01-02	\N	1231231234	p8MikeuBbbbFZ2i7V1gT	\N	f	\N	\N	\N	\N
 f7bd4a7f-b63f-41c3-83bd-9683f33bb4b3	charlie@example.com	400$8$50$8368e20d878ef1b1$b271e3af024b424b7256592439a35d6eb224b4dc769ac9f2fa564b282efb8a47	QOqWQ24CMiRNuPUz8f5	2016-06-03 18:23:06.739671	2016-06-03 18:23:06.739671	t	Charlie	Young	2005-10-02	\N	1231231234	rkU7yVplV5FMsoJFDkaM	\N	f	\N	\N	\N	\N
 abe9fd39-f0b3-4ec6-9006-9783fbdade07	fun@example.com	400$8$50$ef1eb813f8d8b99d$2932a9dc75d10f13525e43c29726061d99b4ebdff2e9f9951eb6e2393f36d221	uMYA6c3A7uGoI0aEbJ8R	2016-06-03 18:23:05.797143	2016-06-07 21:53:45.149755	t	Fun	Buyer	2022-12-31	5030cc27-e7a8-4768-b355-20cdcf9efc53	1112223333	8npwjv7m8NmCTT9eZdIK	\N	f	\N	\N	\N	2016-06-07 21:53:45.148823
```

### Comparing `pg_stage-0.1.8/tests/sql/test_parse_copy_values_with_relations.sql` & `pg_stage-0.1.9/tests/sql/test_parse_copy_values_with_relations.sql`

 * *Files identical despite different names*

### Comparing `pg_stage-0.1.8/tests/sql/test_parse_copy_values_with_self_relation.sql` & `pg_stage-0.1.9/tests/sql/test_parse_copy_values_with_self_relation.sql`

 * *Files identical despite different names*

### Comparing `pg_stage-0.1.8/.gitignore` & `pg_stage-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pg_stage-0.1.8/LICENSE.txt` & `pg_stage-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pg_stage-0.1.8/README.md` & `pg_stage-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pg_stage-0.1.8/pyproject.toml` & `pg_stage-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pg_stage"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="froOzzy", email="ieme5gll6u78@mail.ru" },
 ]
 description = "Anonymization of data in pg_dump"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `pg_stage-0.1.8/PKG-INFO` & `pg_stage-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg_stage
-Version: 0.1.8
+Version: 0.1.9
 Summary: Anonymization of data in pg_dump
 Project-URL: Homepage, https://github.com/froOzzy/pg_stage
 Author-email: froOzzy <ieme5gll6u78@mail.ru>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

