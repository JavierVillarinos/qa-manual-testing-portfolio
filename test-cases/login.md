Login - Test Cases

Información general

Funcionalidad: Inicio de sesión
Requisito: REQ-001
Tipo de prueba: Pruebas funcionales
Estado: En preparación


TC-001 - Inicio de sesión con credenciales válidas

Requisito: REQ-001
Prioridad: Alta
Precondiciones: El usuario debe estar registrado.
Datos de prueba: Email y contraseña correctos.

Pasos:
  -Acceder al formulario de inicio de sesión.
  -Ingresar un email registrado.
  -Ingresar la contraseña correspondiente.
  -Presionar el botón de inicio de sesión.

Resultado esperado: El sistema permite iniciar sesión y muestra la página correspondiente al usuario autenticado.
Resultado obtenido: Pendiente de ejecución.
Estado: No ejecutado.



TC-002 - Inicio de sesión con contraseña incorrecta

Requisito: REQ-001
Prioridad: Alta
Precondiciones: El usuario debe estar registrado.
Datos de prueba: Email correcto y contraseña incorrecta.

Pasos:
  -Acceder al formulario de inicio de sesión.
  -Ingresar un email registrado.
  -Ingresar una contraseña incorrecta.
  -Presionar el botón de inicio de sesión.

Resultado esperado: El sistema rechaza el inicio de sesión y muestra un mensaje de error.
Resultado obtenido: Pendiente de ejecución.
Estado: No ejecutado.



TC-003 - Inicio de sesión con email incorrecto y contraseña correcta

Requisito: REQ-001
Prioridad: Alta
Precondiciones: Debe existir un usuario registrado cuya contraseña sea conocida para la prueba.
Datos de prueba: Email no registrado y contraseña correcta del usuario de prueba.

Pasos:
  -Acceder al formulario de inicio de sesión.
  -Ingresar un email no registrado.
  -Ingresar la contraseña correcta del usuario de prueba.
  -Presionar el botón de inicio de sesión.

Resultado esperado: El sistema rechaza el inicio de sesión y muestra un mensaje de error.
Resultado obtenido: Pendiente de ejecución.
Estado: No ejecutado.


TC-004 - Inicio de sesión con email y contraseña incorrectos
Requisito: REQ-001
Prioridad: Alta
Precondiciones: Ninguna adicional.
Datos de prueba: Email no registrado y contraseña incorrecta.

Pasos:
  -Acceder al formulario de inicio de sesión.
  -Ingresar un email no registrado.
  -Ingresar una contraseña incorrecta.
  -Presionar el botón de inicio de sesión.

Resultado esperado: El sistema rechaza el inicio de sesión y muestra un mensaje de error.
Resultado obtenido: Pendiente de ejecución.
Estado: No ejecutado.



TC-005 - Inicio de sesión con email vacío y contraseña correcta

Requisito: REQ-001
Prioridad: Alta
Precondiciones: El usuario debe estar registrado.
Datos de prueba: Email vacío y contraseña correcta.

Pasos:
  -Acceder al formulario de inicio de sesión.
  -Dejar el campo de email vacío.
  -Ingresar la contraseña correcta.
  -Presionar el botón de inicio de sesión.

Resultado esperado: El sistema impide el inicio de sesión e informa que el campo de email es obligatorio.
Resultado obtenido: Pendiente de ejecución.
Estado: No ejecutado.
