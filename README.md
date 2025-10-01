
# Curso de PostgreSQL intensivo

## https://github.com/psigcat/curso_postgresql

## Tema 1 Introducción

#### Resumen del curso
Introducción a PostgreSQL y PostGIS, configuración y gestión básica

## Primero hay que descarregar los ficheros comprimidos en zip de este enlace, y descomprimirlos
Link material del curs([[https://drive.google.com/file/d/1-RnbCtC-7NPP-5YFcJ-6c1nRe4rVYa2W/view?usp=sharing](https://drive.google.com/file/d/1gnWKqoVd629DHXb93-j_OfwBF3RYIH-h/view?usp=sharing)]) (25 MB)

## Hay que tener instalado PostgreSQL, PostGIS, pgAdmin 4 y ...... otro cliente????

### Windows
Toturial como instalar postgreSQL y PostGIS en Windows
https://youtu.be/_EgtELrjLO4

### Linux
Protoclo de instalación y configuración en Linux
https://github.com/carlospsig/protocol_install_qgis_ubuntu/blob/master/install_postgis.sh

### PostgreSQL Service connection file
https://docs.qgis.org/3.10/en/docs/user_manual/managing_data_source/opening_data.html#pg-service-file

## Pasos a hacer
##### 1 Instalar PostgreSQL 17

##### 2 Instalar PostGIS 3, con Stackbuilder

##### 3 Instalar pgAdmin4 9

##### 4 Abrir pgAdmin con la configuración inicial
- host=localhost
- port=5432
- dbase=postgres
- user=postgres
- password=??

##### 5 Crear una nueva base de datos = **gis_curso**
Utilizar como plantilla (template) la base de datos "postgres", si se puede

##### 6 Activar la extensión de PostGIS
Ejecutar la sintaxi siguiente en una "Query Tool"
- create extension postgis;

##### 7 crear un nuevo usuario gisadmin
Ejecutar la sintaxi siguiente en una "Query Tool", antes de ejecutarlo reemplazar el texto 'your_password' por un password vuestro personal y guardarlo en agún sitio seguro como keepass
- CREATE ROLE **gisadmin** login PASSWORD **'your_password'** SUPERUSER CREATEDB CREATEROLE NOINHERIT;

##### 8 Abrir pgAdmin con el usuario gisadmin
Crear un nueva conexión con el usuario gisadmin y guardar la conexión

##### 9 Crear schemas de trabajo
Primero creamos nuevos esquemas 
  - limit_admin 
  - medi_ambient

##### 10 importar las tablas
Editamos los ficheros SQL que tenemos en la carpeta Datos
  - espais_pein.sql 
  - municipis_catalunya.sql

#### video 1- Instalar, configurar PostGIS e importar capas
https://youtu.be/_EgtELrjLO4

#### Otros vídeos tutoriales en este canal
http://www.youtube.com/c/CarlosLópezQuintanilla

### dudas y comentarios
carlos.lopez@psig.es

Colabora con QGIS, hazte socio!
www.qgis.es

## Fí
