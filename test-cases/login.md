# Login - Test Cases

### Información general

Funcionalidad: Inicio de sesión  
Requisito: REQ-001  
Tipo de prueba: Pruebas funcionales  
Estado: En preparación  


# TC-001 - Inicio de sesión con credenciales válidas

Requisito: REQ-001  
Prioridad: Alta  
Precondiciones: El usuario debe estar registrado.  
Datos de prueba: Usuario y contraseña correctos.  

### Pasos:  
  -Acceder al formulario de inicio de sesión.  
  -Ingresar un usuario registrado.  
  -Ingresar la contraseña correspondiente.  
  -Presionar el botón de inicio de sesión.  

### Resultados:  
Resultado esperado: El sistema permite iniciar sesión y muestra la página correspondiente al usuario autenticado.  
Resultado obtenido: El inicio de sesión fue exitoso y se mostró la página de productos.  
Estado: PASS (Aprobado).  
Observaciones: Se ingresó con las credenciales válidas "standard_user" / "secret_sauce" y se accedió correctamente al catálogo de productos.  



# TC-002 - Inicio de sesión con contraseña incorrecta

Requisito: REQ-001  
Prioridad: Alta  
Precondiciones: El usuario debe estar registrado.  
Datos de prueba: Usuario correcto y contraseña incorrecta.  

### Pasos:  
  -Acceder al formulario de inicio de sesión.  
  -Ingresar un usuario registrado.  
  -Ingresar una contraseña incorrecta.  
  -Presionar el botón de inicio de sesión.  

### Resultados:  
Resultado esperado: El sistema rechaza el inicio de sesión y muestra un mensaje de error.  
Resultado obtenido: El sistema rechazó el inicio de sesión y mostró el mensaje: "Epic sadface: Username and password do not match any user in this service."  
Estado: PASS (Aprobado).  
Observaciones: Se mostraron indicadores de error en los campos de usuario y contraseña, junto con un mensaje de error general. No se permitió el acceso al catálogo de productos.  


# TC-003 - Inicio de sesión con usuario incorrecto y contraseña correcta

Requisito: REQ-001 
Prioridad: Alta  
Precondiciones: Debe existir un usuario registrado cuya contraseña sea conocida para la prueba.  
Datos de prueba: Usuario no registrado y contraseña correcta del usuario de prueba.  

### Pasos:  
  -Acceder al formulario de inicio de sesión.  
  -Ingresar un usuario no registrado.  
  -Ingresar la contraseña correcta del usuario de prueba.  
  -Presionar el botón de inicio de sesión.  

### Resultados:  
Resultado esperado: El sistema rechaza el inicio de sesión y muestra un mensaje de error.  
Resultado obtenido: El sistema rechazó el inicio de sesión y mostró el mensaje: "Epic sadface: Username and password do not match any user in this service."  
Estado: PASS (Aprobado).  
Observaciones: Se mostraron indicadores de error en los campos de usuario y contraseña, junto con un mensaje de error general. No se permitió el acceso al catálogo de productos.  


# TC-004 - Inicio de sesión con usuario y contraseña incorrectos

Requisito: REQ-001  
Prioridad: Alta  
Precondiciones: Ninguna adicional.  
Datos de prueba: Usuario no registrado y contraseña incorrecta.  

### Pasos:  
  -Acceder al formulario de inicio de sesión.  
  -Ingresar un usuario no registrado.  
  -Ingresar una contraseña incorrecta.  
  -Presionar el botón de inicio de sesión.  

### Resultados:  
Resultado esperado: El sistema rechaza el inicio de sesión y muestra un mensaje de error.  
Resultado obtenido: El sistema rechazó el inicio de sesión y mostró el mensaje: "Epic sadface: Username and password do not match any user in this service."  
Estado: PASS (Aprobado).  
Observaciones: Se mostraron indicadores de error en los campos de usuario y contraseña, junto con un mensaje de error general. No se permitió el acceso al catálogo de productos.  


# TC-005 - Inicio de sesión con usuario vacío y contraseña correcta

Requisito: REQ-001  
Prioridad: Alta  
Precondiciones: El usuario debe estar registrado.  
Datos de prueba: Usuario vacío y contraseña correcta.  

### Pasos:  
  -Acceder al formulario de inicio de sesión.  
  -Dejar el campo de Usuario vacío.  
  -Ingresar la contraseña correcta.  
  -Presionar el botón de inicio de sesión.  

### Resultados:  
Resultado esperado: El sistema impide el inicio de sesión e informa que el campo de Usuario es obligatorio.  
Resultado obtenido: El sistema rechazó el inicio de sesión y mostró el mensaje: "Epic sadface: Username is required".  
Estado: PASS (Aprobado).  
Observaciones: Se mostraron indicadores de error en los campos de usuario y contraseña, junto con un mensaje indicando que el nombre de usuario es obligatorio. No se permitió el acceso al catálogo de productos.

## Resumen de ejecución

| ID     | Caso de prueba                   | Resultado |
| ------ | -------------------------------- | --------- |
| TC-001 | Inicio de sesión exitoso         | PASS      |
| TC-002 | Contraseña incorrecta            | PASS      |
| TC-003 | Usuario incorrecto               | PASS      |
| TC-004 | Usuario y contraseña incorrectos | PASS      |
| TC-005 | Usuario vacío                    | PASS      |
