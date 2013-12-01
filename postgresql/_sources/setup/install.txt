Instalando Postgres
===================

Para Mac
~~~~~~~~

`Postgres App <http://www.postgresapp.com>`_

Para Ubuntu
~~~~~~~~~~~

.. code-block:: sh

   sudo apt-get install postgresql

Para Windows
~~~~~~~~~~~~


`Instalador de Windows <http://www.enterprisedb.com/products-services-training/pgdownload#windows>`_

Para instalaciones YUM (Fedora / Red Hat / CentOS / Scientific Linux)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

(Ejemplo usado para PostgreSQL 9.2 en CentOS 6.4 x64)

1. Diríjase a `Repositorio Yum de PostgreSQL <http://yum.postgresql.org/>`_

2. Seleccione la versión de PostgreSQL que desea instalar y luego el SO, versión y arquitectura.

3. Descargar el RPM para tu plataforma (usando el link del paso 2)

.. code-block:: sh

   curl -O http://yum.postgresql.org/9.2/redhat/rhel-6-x86_64/pgdg-centos92-9.2-6.noarch.rpm

4. Instalar el RPM

.. code-block:: sh

   rpm -ivh pgdg-centos92-9.2-6.noarch.rpm

5. Con una busqueda rápida le mostrará los paquetes diposnibles para postgres

.. code-block:: sh
   
   yum list postgres*

Nota: Probablemente liste versiones anteriores también, asegúrese seleccionar la versión correcta que deseas instalar y todos los paquetes sean de la misma versión ejem: servidor, cliente, contrib (no siempre son necesarias pero es mejor, verdad?)

6. Instalar los paquetes descargados

.. code-block:: sh
   
   yum install postgresql92-server.x86_64 postgresql92-contrib.x86_64 postgresql92-devel.x86_64
   
