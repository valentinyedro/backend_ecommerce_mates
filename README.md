# Proyecto Software - Backend E-Commerce Mates Berazategui

Este repositorio contiene el backend de una plataforma de e-commerce especializada en la venta de mates, desarrollada como parte de la materia Proyecto de Software. El sistema fue construido en **C#** siguiendo una arquitectura hexagonal, y proporciona la lógica de negocio, APIs y acceso a datos necesarios para una experiencia completa de comercio electrónico (las compras son ficticias).

## Propósito y Alcance

El objetivo de este backend es brindar soporte funcional a la plataforma de Mates Berazategui, permitiendo:

- Consultar y gestionar productos.
- Manejar información clientes.
- Procesar pedidos.
- Gestionar inventario.

## ⚙️ Arquitectura del Sistema

El sistema sigue una arquitectura hexagonal, lo que permite separar responsabilidades y mantener el código organizado dividiendo la lógica en tres capas principales:

- **Application**: Orquesta la lógica de negocio e interacciones entre componentes.
- **Domain**: Contiene las entidades y reglas del negocio puro.
- **Infrastructure**: Maneja detalles técnicos como acceso a base de datos.

---

## API Endpoints

A continuación se enumeran los endpoints disponibles en el backend:

### 🛒 Carrito

- `PUT /api/carrito`  
  Agrega un producto al carrito.

- `PATCH /api/carrito`  
  Actualiza la cantidad de un producto en el carrito.

- `DELETE /api/carrito/{clientId}/{productId}`  
  Elimina un producto específico del carrito de un cliente.

### 👤 Clientes

- `POST /api/clientes`  
  Crea un nuevo cliente.

### 📦 Orden

- `POST /api/orden/{clientId}`  
  Genera una orden a partir del carrito de un cliente.

- `GET /api/orden`  
  Lista todas las órdenes.

### 🧉 Productos

- `GET /api/productos`  
  Obtiene la lista de productos disponibles.

- `GET /api/productos/{id}`  
  Obtiene los detalles de un producto específico.

## Contribuciones

Se agradece cualquier contribución o sugerencia. Si deseás colaborar, podés hacer un *fork* del repositorio y enviar un *pull request* con tus cambios.

## Contacto

Para cualquier consulta, no dudes en contactarte:

Valentin Yedro: vnyedro@gmail.com

¡Gracias por visitar el repositorio! Espero que disfrutes explorando el backend del e-commerce de Mates Berazategui.
