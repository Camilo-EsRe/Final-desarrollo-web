# Aplicación de Gestión de Contactos (Full-Stack)

Este es un proyecto de aplicación full-stack diseñado para gestionar contactos, permitiendo a los usuarios registrarse, iniciar sesión y realizar operaciones CRUD (Crear, Leer, Actualizar, Eliminar) sobre sus contactos personales.

---

## 🚀 Características Principales

* **Autenticación de Usuarios:**
    * Registro de nuevos usuarios.
    * Inicio de sesión seguro para usuarios existentes.
    * Generación y gestión de tokens JWT para la autenticación de sesiones.
* **Gestión de Contactos (CRUD):**
    * Listado de contactos asociados al usuario logueado.
    * Creación de nuevos contactos (Nombre, Apellidos, Teléfono Fijo, Celular, Email).
    * Actualización de los datos de contactos existentes.
    * Eliminación de contactos.
* **Seguridad:**
    * Contraseñas hasheadas con `bcryptjs`.
    * Rutas protegidas por token JWT en el backend.
    * Protección de rutas en el frontend basada en la autenticación del usuario.

---

## 🛠️ Tecnologías Utilizadas

### Frontend
* **Angular**: Framework para la construcción de interfaces de usuario dinámicas.
* **TypeScript**: Lenguaje de programación que añade tipado estático a JavaScript.
* **HTML5 / CSS3**: Para la estructura y estilos de la interfaz.
* **HttpClientModule**: Módulo de Angular para realizar peticiones HTTP al backend.
* **FormsModule**: Módulo de Angular para manejar formularios basados en plantillas (`ngModel`).
* **CommonModule**: Módulo de Angular que provee directivas estructurales (`*ngIf`, `*ngFor`).
* **Session Storage**: Para el almacenamiento del token de sesión del usuario.

### Backend
* **Node.js**: Entorno de ejecución de JavaScript en el lado del servidor.
* **Express.js**: Framework web para Node.js, utilizado para construir la API REST.
* **`jsonwebtoken`**: Para implementar JSON Web Tokens (JWT) para la autenticación.
* **`bcryptjs`**: Para el hashing seguro de contraseñas.
* **`cors`**: Middleware para habilitar Cross-Origin Resource Sharing.
* **`dotenv`**: Para la gestión de variables de entorno (ej. secretos JWT, URLs de bases de datos).

### Base de Datos
* **MongoDB (Opción Principal)**: Base de datos NoSQL basada en documentos.
    * **Mongoose**: ODM (Object Data Modeling) para Node.js que simplifica la interacción con MongoDB.
* **MySQL (Opción Alternativa)**: Base de datos relacional.
    * **`mysql2`**: Driver para Node.js para interactuar con bases de datos MySQL.

---

## 📂 Estructura del Proyecto

El proyecto está dividido en dos directorios principales: `frontend` y `backend`.