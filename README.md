CREATE TABLE Categorias (
    id_categoria INT PRIMARY KEY,
    nombre_categoria VARCHAR(100)
);
CREATE TABLE Productos (
    id_producto INT PRIMARY KEY,
    nombre_producto VARCHAR(100),
    precio DECIMAL(10,2),
    id_categoria INT,
    FOREIGN KEY (id_categoria) REFERENCES Categorias(id_categoria)
);
