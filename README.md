![Logo de GammaTech SChool](./assets/Logo_Yellow.png)

# Challenge: Authentication
En este pequeño reto, vamos a poner en práctica todo lo que hemos aprendido de peticiones `HTTP` con `fetch` para programar un flujo de autenticación típico de muchas aplicaciones.

### Introducción
La escuela necesita construir un `back office` que le presente la información de todos los alumnos que están actualmente matriculados en sus cursos. Sin embargo, sólo los usuarios con permisos (los trabajadores), pueden acceder al `endpoint` de la API que devuelve el registro de usuarios. Por ello, existe otro `endpoint` que gestiona la autenticación con usuario (email) y contraseña.

Además, para diseñar el frontend, te proporcionan el [este Figma](https://www.figma.com/file/oV5b9JjO2WNm5dTzVRhSsk/Auth-Challenge?node-id=0-1&t=AMfzBMTiz1THXQyg-0).

### Requisitos
- Ningún usuario no autorizado puede tener acceso a la página donde se visualiza el registro de alumnos. Debe redirigirse a los usuarios desconocidos a la página de login.
- Si los credenciales introducidos en el formulario de login son incorrectos, debe informarse al usuario de que dicho usuario no está registrado.
- Si, por el contrario, el proceso de logado es correcto, debe redirigirse a la página donde se listan los usuarios.

### Recursos
- Los `endpoints` de la API son:
    - **GET** `https://token-api-wine.vercel.app`: devuelve el listado de alumnos a los usuarios autenticados. EL tipo de autenticación es `bearer token`.
    - **POST** `https://token-api-wine.vercel.app/auth`: recibe los credenciales de usuario (`email` y `password`) y devuelve el token de autenticación.

- Puedes encontrar el Figma del proyecto [aquí](https://www.figma.com/file/oV5b9JjO2WNm5dTzVRhSsk/Auth-Challenge?node-id=0-1&t=AMfzBMTiz1THXQyg-0).
- El usuario y contraseña del proyecto es el siguiente:
    - email: gammatech@gmail.com
    - password: gamma23