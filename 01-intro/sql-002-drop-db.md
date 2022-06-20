# Sentencia SQL DROP DATABASE

La declaración DROP DATABASE se usa para descartar una base de datos SQL existente.

## Sintaxis

```sql
DROP DATABASE databasename;
```

Nota: tenga cuidado antes de descartar una base de datos. ¡Eliminar una base de datos resultará en la pérdida de la información completa almacenada en la base de datos!

## DROP DATABASE Ejemplo

La siguiente instrucción SQL descarta la base de datos existente "testDB":

```sql
DROP DATABASE testDB;
```

Sugerencia: asegúrese de tener privilegios de administrador antes de descartar cualquier base de datos. Una vez que se elimina una base de datos, puede verificarla en la lista de bases de datos con el siguiente comando SQL: SHOW DATABASES;