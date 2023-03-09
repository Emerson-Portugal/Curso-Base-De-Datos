# Curso de SQL

En este repositorio estara los comandos basicos de SQL, que necesitas saber para empezar en el mundo de las bases de datos

El nombre que se le esta asignado es un ejemplo, ya que cada nombre puede variar segun sus preferencias del programador

> "nombreBase" -> Prueba
> "nombreTabla" -> Persona

- Crear una base de datos

```
CREATE DATABASE "nombreBase";
```

- Listar toda las Base de datos Existentes

```
SHOW DATABASES;
```

- Indicar que base de datos vas a usar 

```
USE "nombreBase";
```

- Creamos las tablas para la base de datos

```
CREARTE TABLE "nombreTabla"(
    id int not null auto_increment,
    name varchar(50) not null,
    age int not null,
    email varchar(100) not null,
    primary key (id)
);
```

- Insertamos valores a la tabla

```
INSERT INTO "nombreTabla" (name, age, email) VALUES ('Emer', 20, 'emer@gmail.com');
```

- Listar el contenido de las tablas

```
SELECT * FROM "nombreTabla";
```

- Listar solo en contenido que nosotros indicamos

```
SELECT * FROM "nombreTabla" WHERE 'id' = 'posicion';
```

- Nodificar el valor de un elemento de una Tabla

```
UPDATE "nombreTabla" SET "atributoTabla" = "valorCambio" WHERE "id" = "posicion"
```


- Eliminar el contenido de la Tabla

```
DELETE FROM 'nombreTabla' WHERE 'id' = 'posicion';
```