# Comparing `tmp/Andreani_QA_Selenium-0.0.5.tar.gz` & `tmp/Andreani_QA_Selenium-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_Selenium-0.0.5.tar", last modified: Wed Jun 14 17:08:01 2023, max compression
+gzip compressed data, was "Andreani_QA_Selenium-0.0.6.tar", last modified: Wed Jun 14 17:58:09 2023, max compression
```

## Comparing `Andreani_QA_Selenium-0.0.5.tar` & `Andreani_QA_Selenium-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 17:08:01.956113 Andreani_QA_Selenium-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-06-14 17:08:01.940632 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium/
--rw-rw-rw-   0        0        0    97270 2023-06-14 16:48:55.000000 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium/Selenium.py
--rw-rw-rw-   0        0        0       32 2023-06-14 17:07:42.000000 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 17:08:01.951690 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium.egg-info/
--rw-rw-rw-   0        0        0      310 2023-06-14 17:08:01.000000 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-06-14 17:08:01.000000 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 17:08:01.000000 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      160 2023-06-14 17:08:01.000000 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-14 17:08:01.000000 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      310 2023-06-14 17:08:01.955104 Andreani_QA_Selenium-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Selenium-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 17:08:01.956113 Andreani_QA_Selenium-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1259 2023-06-14 17:07:42.000000 Andreani_QA_Selenium-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:58:09.471540 Andreani_QA_Selenium-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-06-14 17:58:09.445108 Andreani_QA_Selenium-0.0.6/Andreani_QA_Selenium/
+-rw-rw-rw-   0        0        0    97276 2023-06-14 17:46:32.000000 Andreani_QA_Selenium-0.0.6/Andreani_QA_Selenium/Selenium.py
+-rw-rw-rw-   0        0        0       32 2023-06-14 17:07:42.000000 Andreani_QA_Selenium-0.0.6/Andreani_QA_Selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:58:09.464926 Andreani_QA_Selenium-0.0.6/Andreani_QA_Selenium.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-06-14 17:58:09.000000 Andreani_QA_Selenium-0.0.6/Andreani_QA_Selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-14 17:58:09.000000 Andreani_QA_Selenium-0.0.6/Andreani_QA_Selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 17:58:09.000000 Andreani_QA_Selenium-0.0.6/Andreani_QA_Selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      160 2023-06-14 17:58:09.000000 Andreani_QA_Selenium-0.0.6/Andreani_QA_Selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-14 17:58:09.000000 Andreani_QA_Selenium-0.0.6/Andreani_QA_Selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      310 2023-06-14 17:58:09.468842 Andreani_QA_Selenium-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Selenium-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 17:58:09.471540 Andreani_QA_Selenium-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1259 2023-06-14 17:58:04.000000 Andreani_QA_Selenium-0.0.6/setup.py
```

### Comparing `Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium/Selenium.py` & `Andreani_QA_Selenium-0.0.6/Andreani_QA_Selenium/Selenium.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
                   f" {type_locator} apuntando a '{indentify}'")
             Selenium.message_error = f"Se agoto el tiempo de busqueda intentando encontrar el elemento web '{entity}'" \
                                  f" utilizando el identificador " \
                                  f"{type_locator} apuntando a '{indentify}'"
         except Exception as e:
             Functions.exception_logger(e)
             print(f"Ha ocurrido un error inesperado en tiempo de ejecución.")
-        self.lista_descripcion_pasos.append(indentify)
+        Selenium.lista_descripcion_pasos.append(indentify)
         return elements, find_element
 
     def highlight(self, element: WebElement):
 
         """
             Description:
                 Marca en pantalla el elemento pasado como parámetro.
@@ -710,14 +710,15 @@
             Args:
                 url (str): Dirección web que se debe cargar en la window
         """
 
         Selenium.driver.execute_script(f'''window.open("{url}","_blank");''')
         Selenium.page_has_loaded()
 
+
     @staticmethod
     def page_has_loaded():
 
         """
             Description:
                 Espera que la página sea cargada.
             Returns:
```

### Comparing `Andreani_QA_Selenium-0.0.5/setup.py` & `Andreani_QA_Selenium-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 PACKAGE_NAME = 'Andreani_QA_Selenium'  # Debe coincidir con el nombre de la carpeta
 AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'SeleniumFramework para ejecución de casos automatizados'  # Descripción corta
```

