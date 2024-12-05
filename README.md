# Examen de Bases de Datos (MySQL)

## 1. Creación de Tablas

Crea dos tablas con las siguientes características:

### Tabla `clientes`:
- `id_cliente` (clave primaria, tipo INT, autoincremental)
- `nombre` (tipo VARCHAR(100))
- `apellido` (tipo VARCHAR(100))
- `email` (tipo VARCHAR(100))

### Tabla `pedidos`:
- `id_pedido` (clave primaria, tipo INT, autoincremental)
- `id_cliente` (tipo INT, clave foránea que hace referencia a `id_cliente` en la tabla `clientes`)
- `fecha_pedido` (tipo DATE)
- `monto` (tipo DECIMAL(10, 2))

Asegúrate de que la tabla `pedidos` tenga una clave foránea que haga referencia a `clientes.id_cliente`.

---

## 2. Inserción de Registros

Inserta al menos 5 registros en la tabla `clientes` con valores ficticios (nombre, apellido, email).

Luego, inserta al menos 10 registros en la tabla `pedidos` relacionando los `id_cliente` de los clientes con algunos pedidos, asegurando que algunos pedidos sean del mismo cliente y otros de clientes diferentes.

---

## 3. Consulta con INNER JOIN

Realiza una consulta que devuelva los siguientes datos:
- Nombre del cliente
- Apellido del cliente
- Email del cliente
- Fecha del pedido
- Monto del pedido

Filtra los resultados para que solo se muestren los pedidos cuyo monto sea mayor a 100 y que correspondan a clientes cuyo apellido sea "González".

---


