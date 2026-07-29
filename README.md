README - Normalización de Base de Datos para una Tienda de Libros

Descripción del Proyecto

Este proyecto tiene como objetivo diseñar y normalizar una base de datospara una tienda de libros, aplicando las tres primeras Formas Normales(1FN, 2FN y 3FN). El propósito principal es organizar la información demanera eficiente, evitando la redundancia de datos y garantizando laintegridad y consistencia de la información almacenada.

La base de datos permite gestionar la información relacionada con loslibros, sus autores, editoriales y categorías, así como los datos de losclientes, las ventas realizadas y los pagos asociados a cadatransacción.

Objetivos

Aplicar correctamente las reglas de normalización hasta la TerceraForma Normal (3FN).

Eliminar la duplicidad de datos y las dependencias innecesarias.

Diseñar un modelo Entidad-Relación claro y estructurado.

Garantizar la integridad referencial entre las entidades de la basede datos.

Facilitar el mantenimiento y la escalabilidad del sistema.

Primera Forma Normal (1FN)

La 1FN garantiza que cada atributo almacene un único valor, eliminandogrupos repetitivos y asegurando que cada registro pueda identificarsecorrectamente mediante una clave primaria.

Segunda Forma Normal (2FN)

La 2FN permite eliminar las dependencias parciales separando lainformación relacionada con los libros, los clientes y las ventas,logrando que cada atributo dependa completamente de su clave principal.

Tercera Forma Normal (3FN)

La 3FN elimina las dependencias transitivas creando entidadesindependientes que almacenan información única y reutilizable.

Entidades del Modelo

AUTOR

LIBRO

EDITORIAL

CATEGORIA

CLIENTE

VENTA

PAGO

Relaciones del Modelo

AUTOR escribe LIBRO (1).

EDITORIAL publica LIBRO (1).

CATEGORIA clasifica LIBRO (1).

CLIENTE realiza VENTA (1).

LIBRO participa en VENTA (1).

VENTA genera PAGO (1:1).

Estructura de las Entidades

AUTOR

Nombre Autor (PK)

Apellido Autor

LIBRO

ISBN (PK)

Título

Fecha Publicación

Precio

Stock

Nombre Autor (FK)

Editorial (FK)

Categoría (FK)

EDITORIAL

Editorial (PK)

CATEGORIA

Categoría (PK)

CLIENTE

Correo Cliente (PK)

Nombre Cliente

Apellido Cliente

Dirección Cliente

Teléfono Cliente

VENTA

ISBN (FK)

Correo Cliente (FK)

PAGO

Método Pago

Monto

Tecnologías Utilizadas

Draw.io.

Modelo Entidad-Relación.

Normalización de Bases de Datos (1FN, 2FN y 3FN).

Claves Primarias (PK) y Claves Foráneas (FK).

Beneficios del Diseño

Reducción de la redundancia de datos.

Mayor integridad de la información.

Mejor organización del modelo de datos.

Mayor facilidad para el mantenimiento y futuras ampliaciones.

Conclusión

La aplicación de las formas normales permitió construir un modelo dedatos eficiente, organizado y escalable para la gestión de una tienda delibros, garantizando la correcta relación entre sus entidades y evitandoinconsistencias en la información.

Autor

Yeimer Andrés Torres Manrique
