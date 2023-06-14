# Comparing `tmp/Andreani_QA_Selenium-0.0.4.tar.gz` & `tmp/Andreani_QA_Selenium-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_Selenium-0.0.4.tar", last modified: Mon Jun 12 13:43:17 2023, max compression
+gzip compressed data, was "Andreani_QA_Selenium-0.0.5.tar", last modified: Wed Jun 14 17:08:01 2023, max compression
```

## Comparing `Andreani_QA_Selenium-0.0.4.tar` & `Andreani_QA_Selenium-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 13:43:17.676567 Andreani_QA_Selenium-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-06-12 13:43:17.660856 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium/
--rw-rw-rw-   0        0        0    96650 2023-06-09 20:57:03.000000 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium/Selenium.py
--rw-rw-rw-   0        0        0       33 2023-02-13 17:35:28.000000 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 13:43:17.673429 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium.egg-info/
--rw-rw-rw-   0        0        0      310 2023-06-12 13:43:17.000000 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-06-12 13:43:17.000000 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 13:43:17.000000 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      160 2023-06-12 13:43:17.000000 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-12 13:43:17.000000 Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      310 2023-06-12 13:43:17.675526 Andreani_QA_Selenium-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Selenium-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 13:43:17.676567 Andreani_QA_Selenium-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1259 2023-06-09 20:57:03.000000 Andreani_QA_Selenium-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:08:01.956113 Andreani_QA_Selenium-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-06-14 17:08:01.940632 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium/
+-rw-rw-rw-   0        0        0    97270 2023-06-14 16:48:55.000000 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium/Selenium.py
+-rw-rw-rw-   0        0        0       32 2023-06-14 17:07:42.000000 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-14 17:08:01.951690 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-06-14 17:08:01.000000 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-06-14 17:08:01.000000 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-14 17:08:01.000000 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      160 2023-06-14 17:08:01.000000 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-14 17:08:01.000000 Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      310 2023-06-14 17:08:01.955104 Andreani_QA_Selenium-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-26 19:44:24.000000 Andreani_QA_Selenium-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-14 17:08:01.956113 Andreani_QA_Selenium-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1259 2023-06-14 17:07:42.000000 Andreani_QA_Selenium-0.0.5/setup.py
```

### Comparing `Andreani_QA_Selenium-0.0.4/Andreani_QA_Selenium/Selenium.py` & `Andreani_QA_Selenium-0.0.5/Andreani_QA_Selenium/Selenium.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,48 +98,48 @@
         options.add_argument("--verbose")
         options.add_argument("--disable-popup-blocking")
         options.add_argument("--proxy-server='direct://'")
         options.add_argument("--proxy-bypass-list=*")
         options.add_argument("--disable-gpu") if os.name == "nt" else None
         if Parameters.environment == "Linux":
             options.add_argument("--headless")
-            self.set_exception_loggin(True)
-            self.set_mode_debug(False)
+            Selenium.set_exception_loggin(True)
+            Selenium.set_mode_debug(self, False)
             if browser == "CHROME":
                 services = Service(r'/usr/bin/chromedriver')
-                self.driver = webdriver.Chrome(service=services, options=options)
-                self.initialize_browser(url)
-                self.driver.maximize_window()
+                Selenium.driver = webdriver.Chrome(service=services, options=options)
+                Selenium.initialize_browser(self, url)
+                Selenium.driver.maximize_window()
 
         if Parameters.environment == "Windows":
             if options_headless or Parameters.enviroment_confguration == "Server":
                 options.add_argument("--headless")
                 Selenium.set_exception_loggin(True)
                 Selenium.select_browser(self, browser, options)
                 Selenium.initialize_browser(self, url)
                 Selenium.set_highlight(False)
             else:
-                options.add_argument(f"--remote-debugging-port={self.available_port()}")
-                self.set_mode_debug()
-                self.select_browser(browser, options)
-                self.initialize_browser(url)
-                self.driver.maximize_window()
-        return self.driver
+                options.add_argument(f"--remote-debugging-port={Selenium.available_port()}")
+                Selenium.set_mode_debug()
+                Selenium.select_browser(self, browser, options)
+                Selenium.initialize_browser(self, url)
+                Selenium.driver.maximize_window()
+        return Selenium.driver
 
     def initialize_browser(self, url):
         """
         Description:
             Inicia el navegador configurado y navega hacia la url.
         Args:
             url: Url destino.
         """
-        self.driver.implicitly_wait(10)
+        Selenium.driver.implicitly_wait(10)
         try:
-            self.driver.get(url)
-            self.windows = {'Principal': self.driver.window_handles[0]}
+            Selenium.driver.get(url)
+            Selenium.windows = {'Principal': Selenium.driver.window_handles[0]}
         except WebDriverException:
             Selenium.tear_down(self)
             unittest.TestCase().fail(f"--WebDriverException--No se ha podido establecer una "
                                      f"conexión con el ambiente de pruebas {url}.")
 
     def select_browser(self, browser, options):
         """
@@ -148,28 +148,28 @@
             Args:
                 browser: Nombre del navegador.
                 options: Argumentos opcionales del navegador.
         """
         driver_download_path = os.path.abspath(os.path.join(Parameters.current_path, "drivers"))
         try:
             if browser == "CHROME":
-                version = self.get_version_driver_for_browser(browser)
+                version = Selenium.get_version_driver_for_browser(browser)
                 services = Service(ChromeDriverManager(path=driver_download_path, version=version).install())
-                self.driver = webdriver.Chrome(service=services, options=options)
+                Selenium.driver = webdriver.Chrome(service=services, options=options)
             elif browser == "FIREFOX":
                 services = Service(executable_path=GeckoDriverManager(path=driver_download_path).install(),
                                    log_path=None)
-                self.driver = webdriver.Firefox(service=services, options=options)
+                Selenium.driver = webdriver.Firefox(service=services, options=options)
             elif browser == "IE":
                 services = IEDriverManager(path=driver_download_path).install()
-                self.driver = webdriver.Ie(services)
+                Selenium.driver = webdriver.Ie(services)
 
         except WebDriverException as e:
             Functions.exception_logger(e)
-            self.tear_down()
+            Selenium.tear_down(self)
             unittest.TestCase().skipTest(f"El web driver no esta disponible para esta prueba. {e}")
 
     @staticmethod
     def get_version_driver_for_browser(browser):
 
         """
             Description:
@@ -212,28 +212,28 @@
 
     def tear_down(self):
 
         """
             Descripcion:
                 Finaliza la ejecución cerrando el Web Driver.
         """
-        Selenium.create_grid_by_sources(self.data_cache, "Datos del cache")
+        Functions.create_grid_by_sources(self.data_cache, "Datos del cache")
         try:
-            if self.data_cache not in ([], {}):
+            if Selenium.data_cache not in ([], {}):
                 print("====================Inicio Cache===================")
-                pprint.pprint(self.data_cache)
+                pprint.pprint(Selenium.data_cache)
                 print("=====================Fin Cache=====================")
-            print(f"{Functions.color_message('YELLOW', 'AGUARDANDO:')} Se cerrará el web driver.")
-            self.driver.quit()
+            print(f"{Selenium.color_message('YELLOW', 'AGUARDANDO:')} Se cerrará el web driver.")
+            Selenium.driver.quit()
 
         except Exception as e:
             Functions.exception_logger(e)
 
         finally:
-            print(f"{Functions.color_message('GREEN', 'REALIZADO:')} Finaliza la ejecución.")
+            print(f"{Selenium.color_message('GREEN', 'REALIZADO:')} Finaliza la ejecución.")
 
     @staticmethod
     def create_grid_by_sources(resource: dict, message):
 
         body = """
                 <!DOCTYPE html>
                 <html>
@@ -299,16 +299,16 @@
     def refresh(self):
 
         """
             Description:
                 Actualiza la página web.
         """
 
-        self.driver.refresh()
-        self.page_has_loaded()
+        Selenium.driver.refresh()
+        Selenium.page_has_loaded()
 
     def get_proyect_name(self):
 
         """
             Description:
                 Obtiene el nombre del proyecto en contexto.
             Returns:
@@ -324,15 +324,15 @@
         """
             Description:
                 Obtiene la url actual de la pestaña activa.
             Returns:
                 Url (str): La url de la pestaña activa.
         """
 
-        return self.driver.current_url
+        return Selenium.driver.current_url
 
     def locator_element(self, type_locator, indentify, entity=None):
 
         """
             Description:
                 Localiza un elemento utilizando el tipo de identificador indicado como parámetro.
             Args:
@@ -343,34 +343,34 @@
                 Si el elemento fue encontrado imprime "Esperar_Elemento: Se visualizó el elemento " + XPATH",
                 en caso contrario imprime "No se pudo interactuar con el elemento", XPATH".
         """
 
         find_element = False
         elements = None
         try:
-            elements = self.driver.find_element(type_locator, indentify)
+            elements = Selenium.driver.find_element(type_locator, indentify)
             print(f"Se interactuo con el elemento {indentify}")
-            print(f"{self.color_message('GREEN', 'REALIZADO:')} Se detecto el elemento web "
-                  f"'{self.color_message('BLUE', entity)}' utilizando el "
+            print(f"{Selenium.color_message('GREEN', 'REALIZADO:')} Se detecto el elemento web "
+                  f"'{Selenium.color_message('BLUE', entity)}' utilizando el "
                   f"identificador {type_locator} apuntando a '{indentify}'")
             find_element = True
 
         except NoSuchElementException:
-            self.exception = "NoSuchElementException"
-            print(f"No se pudo encontrar el elemento web '{self.color_message('BLUE', entity)}'"
+            Selenium.exception = "NoSuchElementException"
+            print(f"No se pudo encontrar el elemento web '{Selenium.color_message('BLUE', entity)}'"
                   f" utilizando el identificador {type_locator} apuntando a '{indentify}'")
-            self.message_error = f"No se pudo encontrar el elemento web '{entity}' utilizando el identificador " \
+            Selenium.message_error = f"No se pudo encontrar el elemento web '{entity}' utilizando el identificador " \
                                  f"{type_locator} apuntando a '{indentify}'"
 
         except TimeoutException:
-            self.exception = "TimeoutException"
+            Selenium.exception = "TimeoutException"
             print(f"Se agoto el tiempo de busqueda intentando encontrar el elemento web "
-                  f"'{self.color_message('BLUE', entity)}' utilizando el identificador"
+                  f"'{Selenium.color_message('BLUE', entity)}' utilizando el identificador"
                   f" {type_locator} apuntando a '{indentify}'")
-            self.message_error = f"Se agoto el tiempo de busqueda intentando encontrar el elemento web '{entity}'" \
+            Selenium.message_error = f"Se agoto el tiempo de busqueda intentando encontrar el elemento web '{entity}'" \
                                  f" utilizando el identificador " \
                                  f"{type_locator} apuntando a '{indentify}'"
         except Exception as e:
             Functions.exception_logger(e)
             print(f"Ha ocurrido un error inesperado en tiempo de ejecución.")
         self.lista_descripcion_pasos.append(indentify)
         return elements, find_element
@@ -380,24 +380,24 @@
         """
             Description:
                 Marca en pantalla el elemento pasado como parámetro.
             Args:
                 element: Elemento al que se le hace foco.
         """
 
-        Functions.wait(self, 1)
+        Functions.wait(1)
         try:
             original_style = element.get_attribute('style')
             highlight_style = "border: 3px solid green;"
             for x in range(2):
                 try:
-                    self.driver.execute_script("arguments[0].setAttribute('style', arguments[1]);",
+                    Selenium.driver.execute_script("arguments[0].setAttribute('style', arguments[1]);",
                                                element, highlight_style)
                     time.sleep(0.1)
-                    self.driver.execute_script("arguments[0].setAttribute('style', arguments[1]);",
+                    Selenium.driver.execute_script("arguments[0].setAttribute('style', arguments[1]);",
                                                element, original_style)
                     time.sleep(0.1)
 
                 except Exception as e:
                     Functions.exception_logger(e)
                     print(f"Se encontro el elemento pero no puede ser señalado.")
 
@@ -416,58 +416,58 @@
                 variable_y: Variable y para parametrizar un elemento JSON.
             Returns:
                 Si la entidad se encuentra correctamente se devuelve el elemento y se imprime "Última screenshot
                 antes de finalizar la ejecución", caso contrario lanza la excepción.
         """
 
         element = None
-        self.page_has_loaded()
-        get_entity = self.get_entity(entity)
+        Selenium.page_has_loaded()
+        get_entity = Selenium.get_entity(self, entity)
         if get_entity is None:
             print("No se encontro el value en el Json definido.")
         else:
             if variable_x is not None:
-                self.value_to_find = self.value_to_find.replace("IndiceX", variable_x)
+                Selenium.value_to_find = Selenium.value_to_find.replace("IndiceX", variable_x)
             if variable_y is not None:
-                self.value_to_find = self.value_to_find.replace("IndiceY", variable_y)
+                Selenium.value_to_find = Selenium.value_to_find.replace("IndiceY", variable_y)
 
         find_element = False
         for intentos in range(Parameters.number_retries):
-            if self.get_locator_type.lower() == "xpath":
-                element, find_element = self.locator_element(By.XPATH, self.value_to_find)
+            if Selenium.get_locator_type.lower() == "xpath":
+                element, find_element = Selenium.locator_element(self, By.XPATH, Selenium.value_to_find, entity=entity)
 
-            elif self.get_locator_type.lower() == "id":
-                element, find_element = self.locator_element(By.ID, self.value_to_find)
+            elif Selenium.get_locator_type.lower() == "id":
+                element, find_element = Selenium.locator_element(self, By.ID, Selenium.value_to_find, entity=entity)
 
-            elif self.get_locator_type.lower() == "name":
-                element, find_element = self.locator_element(By.NAME, self.value_to_find)
+            elif Selenium.get_locator_type.lower() == "name":
+                element, find_element = Selenium.locator_element(self, By.NAME, Selenium.value_to_find, entity=entity)
             else:
                 print("El tipo de entidad del objeto no es valido para Selenium Framework.")
                 unittest.TestCase().fail(f"--JsonErrorIdentity-- El tipo de entidad del objeto {entity} no es valido.")
 
             if find_element:
                 unittest.TestCase().assertTrue(find_element, f"El elemento {entity} se visualiza en pantalla.")
                 if Parameters.highlight:
-                    self.highlight(element)
+                    Selenium.highlight(self, element)
                 else:
-                    self.wait(self, Parameters.time_between_retries)
+                    Selenium.wait(Parameters.time_between_retries)
                 break
-            self.wait(self, Parameters.time_between_retries)
+            Selenium.wait(Parameters.time_between_retries)
 
         if not find_element:
             self.image_for_debugger_report()
             self.steps_case = ""
             for i in range(len(self.lista_pasos)):
                 self.steps_case += f"* {self.lista_pasos[i]}: {self.lista_descripcion_pasos[i]}\n"
-            status_code_returned = self.debugger(entity)
+            status_code_returned = Selenium.debugger(entity)
             if status_code_returned == 1:  # retry / refab
-                self.set_retry(3)
+                Selenium.set_retry(3)
                 return Selenium.capture_element(self, entity)
-            self.screenshot("Ultima screenshot antes de finalizar la ejecución")
-            unittest.TestCase().fail(f"--{self.exception}-- El objeto {entity} no se visualiza en pantalla.")
+            Selenium.screenshot("Ultima screenshot antes de finalizar la ejecución")
+            unittest.TestCase().fail(f"--{Selenium.exception}-- El objeto {entity} no se visualiza en pantalla.")
 
         return element
 
     def get_element(self, entity: object, variable_y: object = None, variable_x: object = None):
 
         """
             Description:
@@ -477,17 +477,17 @@
                 variable_y: Variable x para parametrizar un elemento JSON.
                 variable_x: Variable y para parametrizar un elemento JSON.
             Returns:
                 Si la entidad fue encontrada retorna el elemento, en caso contrario imprime
                 "No se encontro el value en el Json definido".
         """
 
-        element = self.capture_element(entity, variable_y=variable_y, variable_x=variable_x)
-        Selenium.page_has_loaded(self)
-        return ElementUI(element, self.driver, self.value_to_find, self.get_locator_type, entity)
+        element = Selenium.capture_element(self, entity, variable_y=variable_y, variable_x=variable_x)
+        Selenium.page_has_loaded()
+        return ElementUI(element, Selenium.driver, Selenium.value_to_find, Selenium.get_locator_type, entity)
 
     def debugger(self, debug_this_entity):
 
         """
             Description:
                 Permite visualizar los defectos antes de finalizar la ejecución, la corrección de los mismos y
                 luego cierra el navegador.
@@ -524,29 +524,27 @@
                 Lee un archivo json.
             Args:
                 file (file): Archivo json.
             Returns:
                 Si el archivo fue encontrado imprime "get_json_file: " + json_path",
                 en caso contrario imprime "get_json_file: No se encontro el Archivo " + file".
         """
-        self.json_on_loaded = file
-        json_path = os.path.abspath(
-            os.path.join(__file__, f"../../../../../projects/{self.project_name}/src/pages/{file}.json"))
-        self.complete_json_path = json_path
+        Selenium.json_on_loaded = file
+        json_path = os.path.join(self.path_json, f"{file}.json")
+        Selenium.complete_json_path = json_path
         try:
             with open(json_path, "r", encoding='utf8') as read_file:
                 Selenium.json_strings = json.loads(read_file.read())
-                print("get_json_file: " + json_path)
-                print(f"{self.color_message('GREEN', 'REALIZADO:')} Se a cargado el respositorio de objetos "
-                      f"'{self.color_message('BLUE', f'{file}.json')}' encontrado en el directorio "
+                print(f"{Selenium.color_message('GREEN', 'REALIZADO:')} Se a cargado el respositorio de objetos "
+                      f"'{Selenium.color_message('BLUE', f'{file}.json')}' encontrado en el directorio "
                       f"'{json_path}'.")
         except FileNotFoundError:
             Selenium.json_strings = False
-            print(f"{self.color_message('RED', 'ERROR:')} No se encontro "
-                  f"'{self.color_message('BLUE', f'{file}.json')}' en el directorio '{json_path}'.")
+            print(f"{Selenium.color_message('RED', 'ERROR:')} No se encontro "
+                  f"'{Selenium.color_message('BLUE', f'{file}.json')}' en el directorio '{json_path}'.")
             unittest.TestCase().skipTest(f"get_json_file: No se encontro el Archivo {file}")
             Selenium.tear_down(self)
 
     def get_entity(self, entity):
 
         """
             Description:
@@ -558,22 +556,22 @@
                 "get_entity: No se encontró la key a la cual se hace referencia: " + entity".
         """
 
         if not Selenium.json_strings:
             print("Define el DOM para esta prueba")
         else:
             try:
-                self.value_to_find = Selenium.json_strings[entity]["ValueToFind"]
-                self.get_locator_type = Selenium.json_strings[entity]["GetFieldBy"]
+                Selenium.value_to_find = Selenium.json_strings[entity]["ValueToFind"]
+                Selenium.get_locator_type = Selenium.json_strings[entity]["GetFieldBy"]
 
             except KeyError as e:
-                self.exception_logger(e)
+                Functions.exception_logger(e)
                 unittest.TestCase().skipTest(f"get_entity: No se encontro la key a la cual se hace referencia:"
                                              f"{entity}.")
-                self.tear_down()
+                Selenium.tear_down()
 
             return True
 
     # TEXTBOX & COMBO HANDLE ###########################################################################################
     def send_especific_keys(self, element, key):
 
         """
@@ -581,164 +579,163 @@
                 Simula el envío de una tecla del teclado.
             Args:
                 element (str): Entidad del objeto que se quiere obtener.
                 key (str): Tecla seleccionada.
         """
 
         if key == 'Enter':
-            self.get_element(self, element).send_keys(Keys.ENTER)
+            Selenium.get_element(self, element).send_keys(Keys.ENTER)
         if key == 'Tab':
-            self.get_element(self, element).send_keys(Keys.TAB)
+            Selenium.get_element(self, element).send_keys(Keys.TAB)
         if key == 'Space':
-            self.get_element(self, element).send_keys(Keys.SPACE)
+            Selenium.get_element(self, element).send_keys(Keys.SPACE)
         if key == 'Esc':
-            self.get_element(self, element).send_keys(Keys.ESCAPE)
+            Selenium.get_element(self, element).send_keys(Keys.ESCAPE)
         if key == 'Retroceso':
-            self.get_element(self, element).send_keys(Keys.BACKSPACE)
+            Selenium.get_element(self, element).send_keys(Keys.BACKSPACE)
         if key == 'Suprimir':
-            self.get_element(self, element).send_keys(Keys.DELETE)
+            Selenium.get_element(self, element).send_keys(Keys.DELETE)
         if key == "Abajo":
-            self.get_element(self, element).send_keys(Keys.ARROW_DOWN)
+            Selenium.get_element(self, element).send_keys(Keys.ARROW_DOWN)
         time.sleep(3)
 
     def get_id_window(self):
 
         """
             Description:
                 Obtiene el id de una window.
             Returns:
                 Devuelve el id de la window obtenida.
         """
 
-        print(self.driver.window_handles[0])
-        return self.driver.window_handles[0]
+        print(Selenium.driver.window_handles[0])
+        return Selenium.driver.window_handles[0]
 
     def switch_to_windows_handles(self, number_window):
 
         """
             Description:
                 Cambia entre ventanas del navegador.
             Args:
                 number_window (int): Número de window seleccionada.
         """
 
-        self.driver.switch_to.window(self.driver.window_handles[number_window])
-        self.driver.maximize_window()
+        Selenium.driver.switch_to.window(Selenium.driver.window_handles[number_window])
+        Selenium.driver.maximize_window()
 
     def switch_to_iframe(self, locator):
 
         """
             Description:
                 Cambia entre iframes en la WebApp.
             Args:
                 locator (str): Nombre del objeto que se quiere obtener.
             Returns:
                 Imprime "Se realizó el switch a (Locator)".
         """
 
-        iframe = self.capture_element(self, locator)
-        self.driver.switch_to.frame(iframe)
+        iframe = Selenium.capture_element(self, locator)
+        Selenium.driver.switch_to.frame(iframe)
         print(f"Se realizó el switch a {locator}")
 
     def switch_to_parent_frame(self):
 
         """
             Description:
                 Cambia al iframes padre.
         """
 
-        self.driver.switch_to.parent_frame()
+        Selenium.driver.switch_to.parent_frame()
         print(f"Se realizó el switch al parent frame.")
 
     def switch_to_default_frame(self):
 
         """
             Description:
                 Cambia al iframe principal.
         """
 
-        self.driver.switch_to.default_content()
+        Selenium.driver.switch_to.default_content()
         print(f"Se realizó el switch al frame principal.")
 
     def switch_to_windows_name(self, window):
 
         """
             Description:
                 Cambia entre ventanas del navegador a través de su nombre.
             Args:
                 window (str): Nombre de ventana seleccionada.
             Returns:
                 Si la ventana es encontrada imprime "volviendo a (ventana)",
                 en caso contrario imprime "Estas en (ventana)".
         """
 
-        if window in self.windows:
-            self.driver.switch_to.window(self.windows[window])
-            self.page_has_loaded()
-            print("volviendo a " + window + " : " + self.windows[window])
+        if window in Selenium.windows:
+            Selenium.driver.switch_to.window(Selenium.windows[window])
+            Selenium.page_has_loaded(self)
+            print("volviendo a " + window + " : " + Selenium.windows[window])
         else:
-            self.number_windows = len(self.driver.window_handles) - 1
-            self.windows[window] = self.driver.window_handles[int(self.number_windows)]
-            self.driver.switch_to.window(self.windows[window])
-            self.driver.maximize_window()
-            print(self.windows)
-            print("Estas en " + window + " : " + self.windows[window])
-            self.page_has_loaded()
+            Selenium.number_windows = len(Selenium.driver.window_handles) - 1
+            Selenium.windows[window] = Selenium.driver.window_handles[int(Selenium.number_windows)]
+            Selenium.driver.switch_to.window(Selenium.windows[window])
+            Selenium.driver.maximize_window()
+            print("Estas en " + window + " : " + Selenium.windows[window])
+            Selenium.page_has_loaded()
 
     def close_page(self):
 
         """
             Description:
                 Cierra la instancia del explorador.
         """
 
-        self.driver.close()
+        Selenium.driver.close()
 
     # FUNCIONES DE JAVASCRIPT ##########################################################################################
     def get_page_dom(self):
 
         """
             Description:
                 Obtiene el DOM de una WebApp.
             Returns:
                 El DOM de una WebApp.
         """
 
-        return self.driver.execute_script("return document.documentElement.outerHTML")
+        return Selenium.driver.execute_script("return document.documentElement.outerHTML")
 
     def new_window(self, url):
 
         """
             Description:
                 Abre una nueva window con el navegador.
             Args:
                 url (str): Dirección web que se debe cargar en la window
         """
 
-        self.driver.execute_script(f'''window.open("{url}","_blank");''')
-        self.page_has_loaded()
-
+        Selenium.driver.execute_script(f'''window.open("{url}","_blank");''')
+        Selenium.page_has_loaded()
 
-    def page_has_loaded(self):
+    @staticmethod
+    def page_has_loaded():
 
         """
             Description:
                 Espera que la página sea cargada.
             Returns:
                 Si la página se cargó imprime "complete", en caso contrario imprime "No se completó la carga".
         """
 
         try:
-            WebDriverWait(self.driver, 60).until(
-                lambda target: self.driver.execute_script('return document.readyState;') == 'complete')
+            WebDriverWait(Selenium.driver, 60).until(
+                lambda target: Selenium.driver.execute_script('return document.readyState;') == 'complete')
 
 
         except TimeoutException:
             try:
-                allure.attach(self.driver.get_screenshot_as_png(),
+                allure.attach(Selenium.driver.get_screenshot_as_png(),
                               "Ultima screenshot antes de finalizar la ejecución.",
                               attachment_type=allure.attachment_type.PNG)
             except Exception as e:
                 Functions.exception_logger(e)
                 print(f"No se pudo realizar la screenshot de pantalla.")
             unittest.TestCase().fail("--TimeoutException-- No se ha podido realizar la carga de la página.")
 
@@ -749,51 +746,52 @@
                 Hace scroll en la página hacia el elemento que se pasa como parámetro.
             Args:
                 y: Variable y para parametrizar un elemento JSON.
                 x: Variable x para parametrizar un elemento JSON.
                 locator (str): Nombre del elemento al cual se quiere scrollear.
         """
 
-        element = self.capture_element(locator, variable_y=y, variable_x=x)
-        self.driver.execute_script("arguments[0].scrollIntoView();", element)
+        element = Selenium.capture_element(self, locator, variable_y=y, variable_x=x)
+        Selenium.driver.execute_script("arguments[0].scrollIntoView();", element)
         print(f"Scroleando la pagina hacia el objeto: {locator}")
 
     # FUNCIONES DE ESPERA ##############################################################################################
-    def wait(self, time_load, logger=Parameters.loggin_time, reason=None):
+    @staticmethod
+    def wait(time_load, logger=Parameters.loggin_time, reason=None):
 
         """
             Description:
                 Espera un elemento, el tiempo es dado en segundos.
             Args:
                 time_load: Tiempo en segundos.
                 logger:
                 reason: Razón por la que se quiere esperar un elemento.
             Returns:
                 Cuando termina el tiempo de espera imprime "Esperar: Carga Finalizada ... "
         """
 
-        return self.wait(time_load, logger=logger, reason=reason)
+        return Functions.wait(time_load, logger=logger, reason=reason)
 
     def alert_windows(self, accept="accept"):
 
         """
             Description:
                 Espera un alert(window pop up) y hace click en accept.
             Args:
                 accept (str): Opción aceptar.
             Returns:
                 Al hacer click en accept imprime "Click in Accept", de lo contrario
                 imprime "Alerta no presente".
         """
 
         try:
-            wait = WebDriverWait(self.driver, 30)
+            wait = WebDriverWait(Selenium.driver, 30)
             wait.until(ec.alert_is_present(), print("Esperando alerta..."))
 
-            alert = self.driver.switch_to.alert
+            alert = Selenium.driver.switch_to.alert
 
             if accept.lower() == "accept":
                 alert.accept()
                 print("Click in Accept")
             elif accept.lower() == "text":
                 print("Get alert text")
                 return alert.text
@@ -806,15 +804,15 @@
         except NoSuchWindowException:
             print('Alerta no presente.')
         except TimeoutException:
             print('Alerta no presente.')
         except UnexpectedAlertPresentException:
             print('Alerta inesperada.')
         except Exception as e:
-            self.exception_logger(e)
+            Functions.exception_logger(e)
             print(f"Ocurrio un error inesperado.")
 
     # ACCION CHAINS ####################################################################################################
     def mouse_over(self, locator):
 
         """
             Description:
@@ -822,101 +820,101 @@
             Args:
                 locator (str): Locator del objeto que se quiere obtener.
             Returns:
                 Retorna "True" si existe el objeto dentro del json, de lo contrario
                 imprime "No se encontró el value en el Json definido".
         """
 
-        get_entity = self.get_entity(locator)
+        get_entity = Selenium.get_entity(self, locator)
         if get_entity is None:
             return print("No se encontro el value en el Json definido.")
         else:
             try:
-                if self.get_locator_type.lower() == "id":
-                    localizador = self.driver.find_element(By.ID, self.value_to_find)
-                    action = ActionChains(self.driver)
+                if Selenium.get_locator_type.lower() == "id":
+                    localizador = Selenium.driver.find_element(By.ID, Selenium.value_to_find)
+                    action = ActionChains(Selenium.driver)
                     action.move_to_element(localizador)
                     action.click(localizador)
                     action.perform()
                     print(u"mouse_over: " + locator)
                     return True
 
-                if self.get_locator_type.lower() == "xpath":
-                    localizador = self.driver.find_element(By.XPATH, self.value_to_find)
-                    action = ActionChains(self.driver)
+                if Selenium.get_locator_type.lower() == "xpath":
+                    localizador = Selenium.driver.find_element(By.XPATH, Selenium.value_to_find)
+                    action = ActionChains(Selenium.driver)
                     action.move_to_element(localizador)
                     action.click(localizador)
                     action.perform()
                     print(u"mouse_over: " + locator)
                     return True
 
-                if self.get_locator_type.lower() == "link":
-                    localizador = self.driver.find_element(By.PARTIAL_LINK_TEXT, self.value_to_find)
-                    action = ActionChains(self.driver)
+                if Selenium.get_locator_type.lower() == "link":
+                    localizador = Selenium.driver.find_element(By.PARTIAL_LINK_TEXT, Selenium.value_to_find)
+                    action = ActionChains(Selenium.driver)
                     action.move_to_element(localizador)
                     action.click(localizador)
                     action.perform()
                     print(u"mouse_over: " + locator)
                     return True
 
-                if self.get_locator_type.lower() == "name":
-                    localizador = self.driver.find_element(By.NAME, self.value_to_find)
-                    action = ActionChains(self.driver)
+                if Selenium.get_locator_type.lower() == "name":
+                    localizador = Selenium.driver.find_element(By.NAME, Selenium.value_to_find)
+                    action = ActionChains(Selenium.driver)
                     action.move_to_element(localizador)
                     action.click(localizador)
                     action.perform()
                     print(u"mouse_over: " + locator)
                     return True
 
             except TimeoutException:
                 print(u"mouse_over: No presente " + locator)
-                self.tear_down()
+                Selenium.tear_down(self)
                 return None
 
             except StaleElementReferenceException:
                 print(u"element " + locator + " is not attached to the DOM")
-                self.tear_down()
+                Selenium.tear_down(self)
                 return None
 
     def double_click_element(self, element: WebElement):
 
         """
             Description:
                 Hace doble click con el mouse sobre un elemento.
             Args:
                 element: Nombre del elemento que se quiere obtener.
         """
 
-        mouse_action = ActionChains(self.driver)
+        mouse_action = ActionChains(Selenium.driver)
         mouse_action.double_click(element)
         mouse_action.perform()
 
     def drag_and_drop(self, origin_object, target_object):
 
         """
             Description:
                 Arrastra y suelta un elemento con el mouse.
             Args:
                 origin_object (str): Origen del elemento.
                 target_object (str): Destino del elemento.
         """
 
-        ActionChains(self.driver).drag_and_drop(origin_object, target_object).perform()
+        ActionChains(Selenium.driver).drag_and_drop(origin_object, target_object).perform()
 
     def click_and_hold(self, origin_object, target_object):
 
         """
             Description:
                 Mantiene un elemento clickeado.
             Args:
                 origin_object (str): Origen del elemento.
                 target_object (str): Destino del elemento.
         """
 
-        mouse_action = ActionChains(self.driver)
+        mouse_action = ActionChains(Selenium.driver)
         mouse_action.click_and_hold(origin_object).move_to_element(target_object).release(target_object)
         mouse_action.perform()
 
     # VALIDADORES ######################################################################################################
     def check_element(self, locator):  # devuelve true o false
 
         """
@@ -925,59 +923,58 @@
             Args:
                 locator (str): Nombre del objeto que se quiere verificar.
             Returns:
                 Retorna "True" si existe el objeto dentro del json, de lo contrario
                 imprime "No se encontro el value en el Json definido".
         """
 
-        get_entity = self.get_entity(locator)
+        get_entity = Selenium.get_entity(self, locator)
 
         if get_entity is None:
             print("No se encontro el value en el Json definido")
         else:
             try:
-                if self.get_locator_type.lower() == "id":
-                    wait = WebDriverWait(self.driver, 20)
-                    wait.until(ec.visibility_of_element_located((By.ID, self.value_to_find)))
+                if Selenium.get_locator_type.lower() == "id":
+                    wait = WebDriverWait(Selenium.driver, 20)
+                    wait.until(ec.visibility_of_element_located((By.ID, Selenium.value_to_find)))
                     print(u"check_element: Se visualizo el elemento " + locator)
                     return True
 
-                if self.get_locator_type.lower() == "name":
-                    wait = WebDriverWait(self.driver, 20)
-                    wait.until(ec.visibility_of_element_located((By.NAME, self.value_to_find)))
+                if Selenium.get_locator_type.lower() == "name":
+                    wait = WebDriverWait(Selenium.driver, 20)
+                    wait.until(ec.visibility_of_element_located((By.NAME, Selenium.value_to_find)))
                     print(u"check_element: Se visualizo el elemento " + locator)
                     return True
 
-                if self.get_locator_type.lower() == "xpath":
-                    wait = WebDriverWait(self.driver, 20)
-                    wait.until(ec.visibility_of_element_located((By.XPATH, self.value_to_find)))
+                if Selenium.get_locator_type.lower() == "xpath":
+                    wait = WebDriverWait(Selenium.driver, 20)
+                    wait.until(ec.visibility_of_element_located((By.XPATH, Selenium.value_to_find)))
                     print(u"check_element: Se visualizo el elemento " + locator)
                     return True
 
-                if self.get_locator_type.lower() == "link":
-                    wait = WebDriverWait(self.driver, 20)
-                    wait.until(ec.visibility_of_element_located((By.LINK_TEXT, self.value_to_find)))
+                if Selenium.get_locator_type.lower() == "link":
+                    wait = WebDriverWait(Selenium.driver, 20)
+                    wait.until(ec.visibility_of_element_located((By.LINK_TEXT, Selenium.value_to_find)))
                     print(u"check_element: Se visualizo el elemento " + locator)
                     return True
 
-                if self.get_locator_type.lower() == "css":
-                    wait = WebDriverWait(self.driver, 20)
-                    wait.until(ec.visibility_of_element_located((By.CSS_SELECTOR, self.value_to_find)))
+                if Selenium.get_locator_type.lower() == "css":
+                    wait = WebDriverWait(Selenium.driver, 20)
+                    wait.until(ec.visibility_of_element_located((By.CSS_SELECTOR, Selenium.value_to_find)))
                     print(u"check_element: Se visualizo el elemento " + locator)
                     return True
 
             except NoSuchElementException:
-                print("get_text: No se encontró el elemento: " + self.value_to_find)
+                print("get_text: No se encontró el elemento: " + Selenium.value_to_find)
                 return False
             except TimeoutException:
-                print("get_text: No se encontró el elemento: " + self.value_to_find)
+                print("get_text: No se encontró el elemento: " + Selenium.value_to_find)
                 return False
 
     # FUNCIONES DE CONFIGURACIÓN #######################################################################################
-
     def set_proyect(self, project_name=None):
 
         """
             Description:
                 Setea variables de ambiente y rutas del proyecto.
             Args:
                 project_name: Nombre del proyecto.
@@ -1145,15 +1142,16 @@
         """
             Description:
                 Devuelve el environment (Sistema operativo) en el que se está corriendo la prueba.
         """
 
         return Parameters.environment
 
-    def get_mode_execution(self):
+    @staticmethod
+    def get_mode_execution():
 
         """
             Description:
                 Indica si el caso requiere ser debugeado.
             Returns:
                 Devuelve valor de la variable de Parameters.debug (True o False)
                 que indica si el caso requiere ser debugeado.
@@ -1218,17 +1216,17 @@
             Description:
                 Saca screenshot de pantalla para los reportes de allure y se agrega la descripción de la misma.
             Args:
                 description: Descripción de la screenshot de pantalla.
             Returns:
                 Retorna la imágen y descripción de la screenshot de pantalla.
         """
-        Selenium.page_has_loaded(self)
+        Selenium.page_has_loaded()
         try:
-            allure.attach(self.driver.get_screenshot_as_png(), description, attachment_type=allure.attachment_type.PNG)
+            allure.attach(Selenium.driver.get_screenshot_as_png(), description, attachment_type=allure.attachment_type.PNG)
         except Exception as e:
             Functions.exception_logger(e)
             print(f"No se pudo realizar la screenshot de pantalla.")
 
     def image_for_debugger_report(self):
 
         """
@@ -1236,15 +1234,15 @@
                 Saca screenshot de pantalla para los reportes de allure y se agrega la descripción de la misma.
             Returns:
                 Retorna la imágen y descripción de la screenshot de pantalla.
         """
         try:
             base_folder = f"C:\\testing-Automation\\projects\\{str(self.project_name)}\\src\\outputs\\"
             if "jira_report.png" not in base_folder:
-                self.memory_image = self.driver.get_screenshot_as_png()
+                self.memory_image = Selenium.driver.get_screenshot_as_png()
         except Exception as e:
             print(f"Hubo inconvenientes al intentar crear la carpeta contenedora de las 'report image'")
 
     # SERVICIOS WEB ####################################################################################################
     def send_service(self, data):
 
         """
@@ -1288,15 +1286,15 @@
             else:
                 try:
                     response = requests.request(data['tipoPeticion'], data['endPoint'], timeout=data['time'])
                     print(f"El servicio '{data['endPoint']}' respondio con status code {response.status_code}")
                     break
                 except requests.exceptions.Timeout:
                     print("Hubo un error por timeout al enviar el servicio")
-            Functions.wait(self, 1)
+            Selenium.wait(1)
 
         # Se valida es status code del request.
         try:
             unittest.TestCase().assertNotEqual(str(type(response)), "<class 'str'>",
                                                "Error Status Code: No se obtuvo response valido. Response de tipo String (TimeOut)")
             validation_status_code = self.validate_status_code(data['statusCodeEsperado'], response.status_code)
             statuscode = response.status_code
@@ -1565,15 +1563,15 @@
                 name_template (str): Nombre del template a utilizar.
             Return:
                 Retorna la ruta del archivo html creado.
         """
 
         from datetime import datetime
         replacement = ""
-        path = self.path_output
+        path = Selenium.path_output
 
         date_time = datetime.now().strftime("%d-%m-%y_%H-%M-%S-%f")
         file_name = f"{date_time}.html"
 
         path_file = os.path.join(path, file_name)
 
         with open(path_file, 'a', encoding="utf-8") as f:
@@ -2197,15 +2195,15 @@
         Selenium.driver.execute_script("window.open('about:blank', 'secondtab');")
         # Cambio de prioridad a la segunda ventana
         Selenium.driver.switch_to.window("secondtab")
         # ingresar a la web deseada en la nueva tab
         Selenium.driver.get(f'{web_url}')
 
 
-class ElementUI(Functions):
+class ElementUI(Selenium):
 
     def __init__(self, context_element, driver, json_value, json_get_indicator, entity):
         self.retry = 0
         self.element = context_element
         self.driver = driver
         self.json_ValueToFind = json_value
         self.json_GetFieldBy = json_get_indicator
```

### Comparing `Andreani_QA_Selenium-0.0.4/setup.py` & `Andreani_QA_Selenium-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 PACKAGE_NAME = 'Andreani_QA_Selenium'  # Debe coincidir con el nombre de la carpeta
 AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'SeleniumFramework para ejecución de casos automatizados'  # Descripción corta
```

