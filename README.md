# 🚀 CRUD API con Express y Sequelize

[![Node.js](https://img.shields.io/badge/Node.js-22-green.svg)](https://nodejs.org/)
[![Express](https://img.shields.io/badge/Express-4.18.2-blue.svg)](https://expressjs.com/)
[![Sequelize](https://img.shields.io/badge/Sequelize-6.35.2-orange.svg)](https://sequelize.org/)
[![SQLite](https://img.shields.io/badge/SQLite-3-lightgrey.svg)](https://www.sqlite.org/)
[![ES Modules](https://img.shields.io/badge/ES%20Modules-Enabled-brightgreen.svg)](https://nodejs.org/api/esm.html)

API RESTful simple para gestión de productos, construida con Express.js y Sequelize ORM, utilizando SQLite como base de datos.

## 📋 Características

- CRUD completo para productos
- Base de datos SQLite para desarrollo
- API RESTful siguiendo las mejores prácticas
- Manejo de errores robusto
- Validación de datos
- Documentación de API incluida

## 🛠️ Requisitos Previos

- Node.js v22 o superior
- npm (incluido con Node.js)

## 🚀 Instalación

1. Clona el repositorio:
```bash
git clone <tu-repositorio>
cd <nombre-del-repositorio>
```

2. Instala las dependencias:
```bash
npm install
```

3. Inicia el servidor de desarrollo:
```bash
npm run dev
```

El servidor se iniciará en `http://localhost:3000`

## 📚 Documentación de la API

### Endpoints

#### Productos

| Método | Endpoint | Descripción |
|--------|----------|-------------|
| GET    | /api/products | Obtener todos los productos |
| GET    | /api/products/:id | Obtener un producto específico |
| POST   | /api/products | Crear un nuevo producto |
| PUT    | /api/products/:id | Actualizar un producto existente |
| DELETE | /api/products/:id | Eliminar un producto |

### Ejemplos de Uso

#### Crear un Producto
```http
POST /api/products
Content-Type: application/json

{
    "name": "Laptop Gaming",
    "price": 1299.99,
    "description": "Laptop gaming de alta gama"
}
```

#### Obtener Todos los Productos
```http
GET /api/products
```

#### Obtener un Producto Específico
```http
GET /api/products/1
```

#### Actualizar un Producto
```http
PUT /api/products/1
Content-Type: application/json

{
    "name": "Laptop Gaming Pro",
    "price": 1499.99,
    "description": "Laptop gaming actualizada"
}
```

#### Eliminar un Producto
```http
DELETE /api/products/1
```

## 🧪 Testing

El proyecto incluye un archivo `requests.http` que contiene ejemplos de todas las peticiones posibles. Para usarlo:

1. Instala la extensión "REST Client" en VS Code
2. Abre el archivo `requests.http`
3. Haz clic en "Send Request" sobre cada petición para probarla

## 📁 Estructura del Proyecto

```
src/
├── config/
│   └── database.js
├── controllers/
│   └── productController.js
├── models/
│   └── Product.js
├── routes/
│   └── productRoutes.js
└── app.js
```

## 🤝 Contribuir

Las contribuciones son bienvenidas. Por favor, abre un issue para discutir los cambios que te gustaría hacer.

## 📄 Licencia

Permission to use, copy, modify, and/or distribute this software for any
purpose with or without fee is hereby granted, provided that the above
copyright notice and this permission notice appear in all copies.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.