# API - CRM

Sistema para gestionar ventas, inventario, empleados, tiendas.

## Desenvolvido com

* [Node](https://nodejs.org/en/)
* [Express](https://expressjs.com/)
* [Prisma](https://www.prisma.io/)
* [PostgreSQL](https://www.postgresql.org/)

Esto es solo el backend de la aplicación, para obtener referencias visuales y también obtener el frontend (creado en React), vaya a: [Xarerp - Client](https://github.com/DanielMafra/xarerp-client)

## Algunas características

* ✅ Persistencia de autenticación utilizando jsonwebtoken
* ✅ Rutas protegidas
* ✅ Rutas con permisos de acceso basados en el usuario que ha iniciado sesión
* ✅ CRUD para cada funcionalidad de registro
* ✅ Reglas para no permitir entradas duplicadas
* ✅ Filtros de búsqueda y paginación
* ✅ Métricas de los últimos 7, 15 y 30 días

## Ejecuta la API

Después de haber clonado el repositorio y accedido a su carpeta a través del terminal, ejecute el siguiente comando (recuerde tener instalado Node + NPM y PostgreSQL)

```bash
  npm install
```

* Cambie el nombre del archivo .env.example a solo .env y reemplace el valor de la información con su entorno de desarrollo.

* Asegúrese de activar su PostgreSQL y ejecute el siguiente comando para crear las tablas

```bash
  npx prisma migrate dev
```

* Después de crear las tablas en la base de datos, ejecute el siguiente comando para poblar las tablas con algunos datos iniciales (no omita este paso)

```bash
  npx prisma db seed
```

El comando anterior ha poblado algunos datos en la base de datos y, de manera predeterminada, puede utilizar las siguientes credenciales de acceso para iniciar sesión:

```bash
  e-mail: user@mail.com
  password: 1234
```

Si todo ha ido bien hasta ahora, la API estará lista para ejecutarse.

* Ejecute el siguiente comando para activar la API y probarla en Insomnia, Postman o su software favorito.

```bash
  npm start
```
