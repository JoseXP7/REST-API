# restapi-express-mysql

REST API hecha con Express.js y MySQL para usarse con el proyecto de [CRUD REST API](https://github.com/JoseXP7/CRUD-Rest-API---Front)

## Variables de Entorno

Para iniciar el proyecto debes añadir estas variables de entorno a tu .env y configurar su valor a como lo requiere la base de datos MySQL

`HOST = localhost`
`DATABASE = `
`USER = root`
`PASSWORD  = `

## Correr localmente

Instalar dependencias

```bash
  npm install
```

Iniciar el servidor

```bash
  npm run dev
```

## Autor

- [@JoseXP7](https://www.github.com/JoseXP7)

## Referencias de la API

#### Obtener todos los lenguajes

```http
  GET /api/languages
```

#### Obtener un solo lenguaje

```http
  GET /api/languages/id
```

| Parameter | Type     | Description                    |
| :-------- | :------- | :----------------------------- |
| `id`      | `string` | **Requerido**. Id del lenguaje |

#### Añadir un lenguaje

```http
  POST /api/languages/
```

| Parameter     | Type     | Description                           |
| :------------ | :------- | :------------------------------------ |
| `name`        | `string` | **Requerido**. Nombre del lenguaje    |
| `programmers` | `number` | **Requerido**. Numero de programadore |

#### Actualizar un lenguaje

```http
  POST /api/languages/id
```

| Parameter     | Type     | Description                           |
| :------------ | :------- | :------------------------------------ |
| `name`        | `string` | **Requerido**. Nombre del lenguaje    |
| `programmers` | `number` | **Requerido**. Numero de programadore |

#### Eliminar un lenguaje

```http
  GET /api/languages/id
```

| Parameter | Type     | Description                    |
| :-------- | :------- | :----------------------------- |
| `id`      | `string` | **Requerido**. Id del lenguaje |
