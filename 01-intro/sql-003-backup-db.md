# Crear respaldo de SQL Server

## La instrucción SQL BACKUP DATABASE

La instrucción BACKUP DATABASE se usa en SQL Server para crear una copia de seguridad completa de una base de datos SQL existente.

## Sintaxis

```sql
BACKUP DATABASE databasename
TO DISK = 'filepath';
```

## La sentencia SQL BACKUP CON DIFERENCIAL

Una copia de seguridad diferencial solo realiza una copia de seguridad de las partes de la base de datos que han cambiado desde la última copia de seguridad completa de la base de datos.

## Sintaxis

```sql
BACKUP DATABASE databasename
TO DISK = 'filepath'
WITH DIFFERENTIAL;
```

## Ejemplo de BACKUP

La siguiente instrucción SQL crea una copia de seguridad completa de la base de datos existente "testDB" en el disco D:

```sql
BACKUP DATABASE testDB
TO DISK = 'D:\backups\testDB.bak';
```

## Ejemplo BACKUP WITH DIFFERENTIAL

La siguiente instrucción SQL crea una copia de seguridad diferencial de la base de datos "testDB":

```sql
BACKUP DATABASE testDB
TO DISK = 'D:\backups\testDB.bak'
WITH DIFFERENTIAL;
```

Sugerencia: una copia de seguridad diferencial reduce el tiempo de copia de seguridad (ya que solo se realiza una copia de seguridad de los cambios).