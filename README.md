# Curso SQL SERVER Básico 

CREATE DATABASE sql_productos;

USE sql_productos;

-- Crear nuestra primer tabla

CREATE TABLE productos(
	--atributos 
	producto_id INT IDENTITY(1,1), -- Para generar un ID auto incrementable INT son los numeros Enteros.
	descripcion VARCHAR(50), -- Varchar acepta cadenas de texto segun el limite que ingresemos en este caso 50.
	fecha_creacion datetime, -- datetime es tipo fecha y hora 2022-10-25 14:23:00
	precio FLOAT,    -- tipo coma flotante para poder utilizar decimales con mas precision.
	PRIMARY KEY (producto_id) -- Identificador unico para cada fila.
);

-- INSERT para generar datos en nuestra tabla productos.
-- En el primer parentesis van los atributos a completar y en el segundo los valores

INSERT INTO productos (descripcion,precio, fecha_creacion) VALUES ( 'Monitor 23 PUL', 15000.5 ,	'2022-05-17 15:45:00');
INSERT INTO productos (descripcion,precio, fecha_creacion) VALUES ( 'Teclado Gamer',8050.5,		'2022-05-17 16:25:00');
INSERT INTO productos (descripcion,precio,fecha_creacion) VALUES ( 'Mouse Logitech',2500.5,		'2022-05-17 16:35:00');
INSERT INTO productos (descripcion,precio, fecha_creacion) VALUES ( 'Pad Gamer',1500.4,			'2022-05-17 16:40:00');
INSERT INTO productos (descripcion,precio,fecha_creacion) VALUES ( 'Impresora Epson L355', 25144.25, '2022-05-17 17:14:00');
INSERT INTO productos (descripcion,precio, fecha_creacion) VALUES ( 'Parlante Sony',7500.5,			'2022-06-17 10:25:00');
INSERT INTO productos (descripcion,precio, fecha_creacion) VALUES ( 'Escritorio Ergonomico',19830.11, '2022-06-17 10:45:00');
INSERT INTO productos (descripcion,precio,fecha_creacion) VALUES ( 'Cargador usb', 900,				'2022-06-17 17:45:00');
INSERT INTO productos (descripcion,precio, fecha_creacion) VALUES ( 'Memoria Ram ddr4 8GB', 6500.5 , '2022-06-17 18:45:00');
INSERT INTO productos (descripcion,precio, fecha_creacion) VALUES ( 'Memoria Ram ddr4 16GB', 3000 , '2022-10-25 11:39:00');