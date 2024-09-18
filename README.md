La base de datos no cuenta con migraciones asi que se tiene que conectar al servidor donde se este ejecutando la prueba 

Create Database Num 

CREATE TABLE personas (
    id INT IDENTITY(1,1) PRIMARY KEY, -- Llave primaria autoincrementable
    numero_cedula VARCHAR(20) NOT NULL, -- Número de cédula obligatorio
    primer_nombre VARCHAR(50) NOT NULL, -- Primer nombre obligatorio
    segundo_nombre VARCHAR(50), -- Segundo nombre opcional
    primer_apellido VARCHAR(50) NOT NULL, -- Primer apellido obligatorio
    segundo_apellido VARCHAR(50), -- Segundo apellido opcional
    telefono VARCHAR(15), -- Teléfono opcional
    correo VARCHAR(100), -- Correo opcional
    direccion VARCHAR(150) NOT NULL, -- Dirección obligatoria
    edad INT NOT NULL, -- Edad obligatoria
    genero CHAR(1) NOT NULL -- Género obligatorio, asumido como una sola letra (M/F/O)
);

INSERT INTO personas (numero_cedula, primer_nombre, segundo_nombre, primer_apellido, segundo_apellido, telefono, correo, direccion, edad, genero)
VALUES
('1234567890', 'Juan', 'Pablo', 'Gómez', 'Hernández', '1234567890', 'juan.gomez@example.com', 'Calle 1 #23-45', 30, 'M'),
('0987654321', 'Ana', 'María', 'López', 'Castro', '0987654321', 'ana.lopez@example.com', 'Avenida 5 #67-89', 25, 'F'),
('1122334455', 'Carlos', 'Andrés', 'Martínez', 'Ríos', '1122334455', 'carlos.martinez@example.com', 'Carrera 10 #12-34', 40, 'M'),
('2233445566', 'Laura', 'Fernanda', 'Rojas', 'Mendoza', '2233445566', 'laura.rojas@example.com', 'Calle 3 #45-67', 35, 'F'),
('3344556677', 'Jorge', 'Luis', 'Pérez', 'García', '3344556677', 'jorge.perez@example.com', 'Calle 4 #56-78', 28, 'M'),
('4455667788', 'Valeria', 'Sánchez', 'Vargas', 'Serrano', '4455667788', 'valeria.sanchez@example.com', 'Avenida 6 #78-90', 32, 'F'),
('5566778899', 'Santiago', 'Alejandro', 'Mendoza', 'García', '5566778899', 'santiago.mendoza@example.com', 'Calle 7 #89-01', 27, 'M'),
('6677889900', 'Camila', 'Andrea', 'Torres', 'Morales', '6677889900', 'camila.torres@example.com', 'Calle 8 #90-12', 29, 'F'),
('7788990011', 'Felipe', 'Eduardo', 'García', 'Paredes', '7788990011', 'felipe.garcia@example.com', 'Carrera 9 #01-23', 33, 'M'),
('8899001122', 'Isabella', 'Méndez', 'Jaramillo', 'Salazar', '8899001122', 'isabella.mendez@example.com', 'Calle 10 #23-45', 26, 'F'),
('9900112233', 'Andrés', 'Felipe', 'Gutiérrez', 'Córdoba', '9900112233', 'andres.gutierrez@example.com', 'Avenida 11 #34-56', 31, 'M'),
('0011223344', 'Paola', 'Juliana', 'Gómez', 'Herrera', '0011223344', 'paola.gomez@example.com', 'Calle 12 #45-67', 34, 'F'),
('1122334456', 'Alejandro', 'Santos', 'Castillo', 'Rentería', '1122334456', 'alejandro.santos@example.com', 'Carrera 13 #56-78', 38, 'M'),
('2233445567', 'Natalia', 'Mora', 'Salazar', 'Hurtado', '2233445567', 'natalia.mora@example.com', 'Avenida 14 #67-89', 30, 'F'),
('3344556678', 'Daniel', 'Riviera', 'Jiménez', 'Velásquez', '3344556678', 'daniel.riviera@example.com', 'Calle 15 #78-90', 26, 'M');

