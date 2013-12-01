Usuarios
########

Agregando un Usuario
--------------------

Una vez terminada la instalación de Postgres debes poder conectarte con `psql -h localhost`. Esto te pondrá dentro de la consola de base de datos para empezar a trabajar. De seguro el siguiente paso antes de hacer algo es crear una cuenta de usuario.


.. code-block:: sql

    craig=# CREATE USER craig WITH PASSWORD 'Password';
    CREATE ROLE

Nuevo usuario `craig` es creado con el password `Password`.

Siguiente paso es crear una base de datos y generar los accesos para el usuario `craig`

.. code-block:: sql

    craig=# CREATE DATABASE pgguide;
    CREATE DATABASE

Ahora la base de datos `pgguide` es creada. Ahora damos permisos al usuario `craig`.

.. code-block:: sql

    craig=# GRANT ALL PRIVILEGES ON DATABASE pgguide to craig;
    GRANT

Ahora `craig` tiene todos los permisos en la base de datos `pgguide`. Hay varias formas de permisos: SELECT, INSERT, UPDATE, DELETE, RULE, REFERENCES, TRIGGER, CREATE, TEMPORARY, EXECUTE, y USAGE.

.. code-block:: sql

    craig=# GRANT SELECT ON DATABASE pgguide to craig;
    GRANT

`GRANT SELECT` allows `craig` ONLY to do `select` query on database `pgguide`

[TBD: Agregar detalles sobre revoke]
