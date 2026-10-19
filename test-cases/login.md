# Login - Test Cases

### Información general

Funcionalidad: Inicio de sesión  
Requisito: REQ-001  
Tipo de prueba: Pruebas funcionales  
Estado: Completado


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

# TC-006 — Inicio de sesión con contraseña vacía

Requisito: REQ-001
Prioridad: Alta
Precondiciones: El usuario debe estar registrado.
Datos de prueba: Usuario registrado; contraseña vacía.

### Pasos:
  -Acceder al formulario de inicio de sesión.
  -Ingresar un usuario registrado.
  -Dejar vacío el campo de contraseña.
  -Presionar el botón de inicio de sesión.

### Resultados:
Resultado esperado: El sistema debe impedir el inicio de sesión e informar que falta completar la contraseña.
Resultado real: El sistema rechazó el inicio de sesión y mostró el mensaje: "Epic sadface: Password is required".
Estado: PASS (Aprobado).  
Observaciones: Se mostraron indicadores de error en los campos de usuario y contraseña, junto con un mensaje indicando que la contraseña es obligatoria. No se permitió el acceso al catálogo de productos.

# TC-007 — Inicio de sesión con usuario y contraseña vacíos

Requisito: REQ-001
Prioridad: Alta
Precondiciones: Acceder al formulario de inicio de sesión.
Datos de prueba: Usuario vacío; contraseña vacía.

### Pasos:
  -Acceder al formulario de inicio de sesión.
  -Dejar vacío el campo de usuario.
  -Dejar vacío el campo de contraseña.
  -Presionar el botón de inicio de sesión.

### Resultados:
Resultado esperado: El sistema debe impedir el inicio de sesión y mostrar un mensaje de validación que indique que deben completarse los campos obligatorios.
Resultado real: El sistema rechazó el inicio de sesión y mostró el mensaje: "Epic sadface: Username is required".
Estado: PASS (Aprobado).  
Observaciones: Se mostraron indicadores de error en los campos de usuario y contraseña, junto con un mensaje indicando el nombre de usuario es obligatorio. No se permitió el acceso al catálogo de productos.

# TC-008 — Inicio de sesión con usuario bloqueado

Requisito: REQ-001
Prioridad: Alta
Precondiciones: Acceder al formulario de inicio de sesión.
Datos de prueba: Usuario: locked_out_user; Contraseña: secret_sauce.

### Pasos:
  -Acceder al formulario de inicio de sesión.
  -Ingresar el usuario bloqueado "locked_out_user".
  -Ingresar la contraseña "secret_sauce".
  -Presionar el botón de inicio de sesión.

### Resultados:
Resultado esperado: el sistema debe impedir el acceso y mostrar un mensaje que indique que el usuario está bloqueado.
Resultado real: El sistema rechazó el inicio de sesión y mostró el mensaje: "Epic sadface: Sorry, this user has been locked out.".
Estado: PASS (Aprobado).  
Observaciones: Se mostraron indicadores de error en los campos de usuario y contraseña, junto con un mensaje indicando el usuario se encuentra bloqueado. No se permitió el acceso al catálogo de productos.

# TC-009 — Inicio de sesión con usuario compuesto por espacios
Requisito: REQ-001
Prioridad: Media
Precondiciones: Acceder al formulario de inicio de sesión.
Datos de prueba: Usuario: tres espacios (   ); Contraseña: secret_sauce.

### Pasos:
  -Acceder al formulario de inicio de sesión.
  -Ingresar tres espacios en el campo Username.
  -Ingresar la contraseña "secret_sauce".
  -Presionar el botón de inicio de sesión.

### Resultados:
Resultado esperado: El sistema debe impedir el inicio de sesión y mostrar un mensaje de validación o de credenciales incorrectas.
Resultado real: El sistema impidió el inicio de sesión y mostró el mensaje "Epic sadface: Username and password do not match any user in this service".
Estado: PASS (Aprobado).
Observaciones: El sistema mostró un error de credenciales no coincidentes en lugar de un mensaje específico para campos vacíos o compuestos únicamente por espacios.




## Resumen de ejecución

| ID     | Caso de prueba                   | Resultado |
| ------ | -------------------------------- | --------- |
| TC-001 | Inicio de sesión exitoso         | PASS      |
| TC-002 | Contraseña incorrecta            | PASS      |
| TC-003 | Usuario incorrecto               | PASS      |
| TC-004 | Usuario y contraseña incorrectos | PASS      |
| TC-005 | Usuario vacío                    | PASS      |
| TC-006 | Contraseña vacía                 | PASS      |
| TC-007 | Usuario y contraseña vacíos      | PASS      |
| TC-008 | Usuario bloqueado                | PASS      |
| TC-009 | Usuario compuesto por espacios   | PASS      |
