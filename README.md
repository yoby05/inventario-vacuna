# Inventario Vacuna
Sistema informático que permite realizar la administración según el perfil asignado ya sea de un Administrador o de un Empleado así como el control y registro del esquema de vacunación completo contra la COVID-19.

## Comenzando 🚀

El desarrollo del proyecto fue realizado bajo un ambiente de máquina local. Las descripciones para el levantamiento del mismo
serán bajo las mismas descripciones.

El Proyecto está dividido por pequeños mini-proyecto
+ inventario-vacuna-bdd (Aquí se encuentran las clases que mapean todas las tablas de la base datos)
+ inventario-vacuna-dto (Aquí se encuentran las clases pojos utilizadas para transformar los objetos de la base y poder realizar todas las acciones que el proyecto requiera)
+ inventario-vacuna-utilitario (Aquí se encuentran métodos, enumeradores, constantes, casteo toda herramienta que puede utilizar en cualquier momento dentro del proyecto)
+ inventario-vacuna-token (Este es uno de los proyecto mas importantes, es el encargado de crear un token con Spring y JWT el cual es utilizado en cada petición realizada lo que brinda una capa de seguridad avanzada)
+ inventario-vacuna-login (Proyecto web de JSF que mediante el ingreso de un usuario y clave se valida la información ingresada y de ser correcto se realizar la petición de crear un token de autenticación)
+ inventario-vacuna-ws (Proyecto backend donde se encuentran todos los servicios REST que permitirán realizar una acción. Este proyecto tiene un interceptor que valida si el token es correcto para poder continuar con la petición)
+ inventario-vacuna-web (Por último tenemos el proyecto web de interacción con el usuario desarrollada bajo la tecnología de primefaces con Spring Boot)

Otra característica principal es que en el caso del proyecto inventario-vacuna-ws y inventario-vacuna-web está configurado para tener su archivo de propiedades fuera de la compilación del proyecto. Los mismos que tienen configurado la conexión a la base y ciertos textos cifrados. En caso de la base para este caso las credenciales son en texto plano, pero como se usa JASYPT se puede cifrar esta información y quedar oculta.


### Pre-requisitos 📋

Para comenzar con el levantamiento del ambiente se necesitan tener instalado los siguientes programas:
+  El JDK de java en su versión 8.
+  Un servidor de base dato Postgresql-v12.
+  Como servidor de aplicaciones Wildfly19 aunque puede ser una superior.
+  Maven para la descarga de Jar necesarios.
+  Configurar variable de entorno de JAVA_HOME(para java) y de M2_HOME(para maven)

### Instalación 🔧

Se asume que el proceso lo realizará una persona con el nivel necesario para el levantamiento del mismo.

Una vez se instale


## Despliegue 📦
+ Desplegar en el servidor de aplicaciones inventario-vacuna-login.war que se encuentra dentro del archivo War Login o mediante el maven o cualquier herramienta exportarlo como .war
+ ubicarse en la carpeta raíz de cada proyecto y ejecutar el comando maven (mvn clean install) pero antes revisar el archivo de propiedad ahi se les actualiza las dependencias de cada proyecto y se les genera un war dentro de la carpeta target siguiendo el orden iventario-vacuna-bdd,iventario-vacuna-dto,iventario-vacuna-utilitario,iventario-vacuna-ws,iventario-vacuna-web


## Construido con 🛠️

Las tecnologías utilizadas para el desarrollo, para el backend Java como leguaje de programación con la ayuda del framework de Spring Boot.
Para la capa del acceso a datos, se utilizó hibernate, jpql, repository y Postgresql como motor de base datos
Para la presentación se utilizó Jsf y Primefaces con la ayuda del modelo mvc del Spring Boot

## Versionado 📌

Versión 1.0.0 con fecha fin 03-10-2021

## Autores ✒️
Yoan Hernández Méndez
correo: yoanhmz@gmail.com
