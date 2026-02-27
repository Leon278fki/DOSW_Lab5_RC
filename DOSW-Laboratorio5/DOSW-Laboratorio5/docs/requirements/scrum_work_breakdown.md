
# 📄 Planeación del Sistema

## Desglose de trabajo: Épicas, Historias de Usuario y Tareas

La implementación de los requerimientos identificados de Bankify se desglosa de la siguiente manera:

---

### 1. Épica: Desarrollo de login y registro de usuarios dentro de la aplicación Bankify

| Campo | Descripción |
|------|-------------|
| **ID** | EP-01 |
| **Título** | Desarrollo de login y registro de usuarios |
| **Descripción** | Implementar autenticación y gestión básica de usuarios para acceso seguro a la aplicación |
| **Stakeholder** | Usuarios finales, Departamento de Seguridad |

### 2. Historias de usuario:

| Campo | Descripción |
|------|-------------|
| **ID** | HU-01 |
| **Título** | Desarrollo de login de usuarios |
| **Descripción** | Como usuario quiero ingresar a la aplicación para realizar transacciones |
| **Prioridad** | *[Alta] [Media] [Baja]* |
| **Estimación** | *Puntos de historia* |

| Campo | Descripción |
|------|-------------|
| **ID** | HU-02 |
| **Título** | Registro de nuevos usuarios |
| **Descripción** | Como nuevo usuario quiero registrarme ingresando mis datos personales para crear una cuenta |
| **Prioridad** | *[Alta] [Media] [Baja]* |
| **Estimación** | *Puntos de historia* |

| Campo | Descripción |
|------|-------------|
| **ID** | HU-03 |
| **Título** | Recuperación de contraseña |
| **Descripción** | Como usuario quiero recuperar mi contraseña en caso de olvido para volver a acceder a mi cuenta |
| **Prioridad** | *[Alta] [Media] [Baja]* |
| **Estimación** | *Puntos de historia* |

| Campo | Descripción |
|------|-------------|
| **ID** | HU-04 |
| **Título** | Autenticación multifactor (2FA) |
| **Descripción** | Como usuario, quiero una segunda capa de verificación (por SMS o correo) para aumentar la seguridad al iniciar sesión |
| **Prioridad** | *[Alta] [Media] [Baja]* |
| **Estimación** | *Puntos de historia* |

### 3. Tareas:

| Campo | Descripción |
|------|-------------|
| **ID** | TR-01 |
| **Título** | Implementar login |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Desarrollar la funcionalidad de autenticación con usuario y contraseña |
| **Tareas requisito** | Ninguna |

| Campo | Descripción |
|------|-------------|
| **ID** | TR-02 |
| **Título** | Verificar datos del login |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Validar credenciales contra la base de datos |
| **Tareas requisito** | TR-01 |

| Campo | Descripción |
|------|-------------|
| **ID** | TR-03 |
| **Título** | Mostrar mensaje de error en login inválido |
| **ID de la Historia de Uso asociada** | HU-01 |
| **Descripción** | Mostrar mensajes de error claros cuando las credenciales sean inválidas |
| **Tareas requisito** | TR-02 |

| Campo | Descripción |
|------|-------------|
| **ID** | TR-04 |
| **Título** | Diseño del formulario de registro |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Diseñar un formulario claro e intuitivo para el registro de usuarios |
| **Tareas requisito** | Ninguna |

| Campo | Descripción |
|------|-------------|
| **ID** | TR-05 |
| **Título** | Implementación reglas de contraseña |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Validar la complejidad de contraseñas (mayúsculas, minúsculas, números, símbolos) |
| **Tareas requisito** | TR-04 |

| Campo | Descripción |
|------|-------------|
| **ID** | TR-06 |
| **Título** | Guardar usuario en base de datos |
| **ID de la Historia de Uso asociada** | HU-02 |
| **Descripción** | Crear proceso para insertar nuevos usuarios en la base de datos de forma segura |
| **Tareas requisito** | TR-05 |

| Campo | Descripción |
|------|-------------|
| **ID** | TR-07 |
| **Título** | Diseñar interfaz de recuperación de contraseña |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Crear un formulario amigable para la recuperación de contraseña |
| **Tareas requisito** | Ninguna |

| Campo | Descripción |
|------|-------------|
| **ID** | TR-08 |
| **Título** | Implementar seguridad para recuperación |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Agregar verificaciones (código, preguntas de seguridad) para asegurar la recuperación |
| **Tareas requisito** | TR-07 |

| Campo | Descripción |
|------|-------------|
| **ID** | TR-09 |
| **Título** | Actualizar base de datos (recuperación) |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Implementar proceso seguro para actualizar la contraseña en la base de datos |
| **Tareas requisito** | TR-08 |

| Campo | Descripción |
|------|-------------|
| **ID** | TR-10 |
| **Título** | Integrar envío de códigos (SMS/Email) |
| **ID de la Historia de Uso asociada** | HU-05 |
| **Descripción** | Implementar servicio para enviar códigos temporales vía SMS o correo electrónico |
| **Tareas requisito** | Ninguna |

| Campo | Descripción |
|------|-------------|
| **ID** | TR-11 |
| **Título** | Interfaz para ingreso de código 2FA |
| **ID de la Historia de Uso asociada** | HU-05 |
| **Descripción** | Diseñar y desarrollar la pantalla/modal para ingresar el código de verificación |
| **Tareas requisito** | TR-10 |

| Campo | Descripción |
|------|-------------|
| **ID** | TR-12 |
| **Título** | Validación y persistencia de preferencias 2FA |
| **ID de la Historia de Uso asociada** | HU-05 |
| **Descripción** | Validar el código 2FA, permitir activar/desactivar 2FA y guardar la preferencia de usuario de forma segura |
| **Tareas requisito** | TR-11 |

