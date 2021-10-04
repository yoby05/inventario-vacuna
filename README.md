# Inventario Vacuna
Sistema informático que permite realizar la administración según el perfil asignado ya sea de un Administrador
o de un Empleado asi como el contro y registro del esquema de vacunación completo contra la COVID-19.

## Comenzando 🚀

El desarrollo del proyeto fue realizado bajo un ambiente de máquina local. Las descripciones para el levantamiento del mismo
serán bajo las misma descripciones.

El Proyecto está dividido por pequeños mini-proyecto
1-inventario-vacuna-bdd (Aqui se encuentran las clases que mapean todas las tablas de la base datos)
2-inventario-vacuna-dto (Aqui se encuentran las clases pojos utilizadas para transformar los objetos de la base y poder realizar todas las acciones que el proyecto requiera)
3-inventario-vacuna-utilitario (Aqui se encuentran metodos, enumeradores, constantes, casteo toda herramienta que puede utilizar en cualquier momento dentro del proyecto)
4-inventario-vacuna-token (Este es uno de los proyecto mas importantes, es el encargado de crear un token con Spring y JWT el cual es utilizado en cada petición realizada lo que brinda una capa de seguridad avanzada)
5- inventario-vacuna-login (Proyecto web de JSF que mediante el ingreso de un usuario y clave se valida la información ingresada y de ser correcto se realiar la petición de crear un token de autenticación)
6-inventario-vacuna-ws (Proyecto backend donde se encuentran todos los servicios REST que permitirán realizar una acción. Este proyecto tiene un interceptor que valida si el token es correcto para poder coontinuar con la petición)
7-inventario-vacuna-web (Por último tenemos el proyecyo web de interación con el usuario desrrollada bajo la tecnología de primefaces con Spring Boot)

### Pre-requisitos 📋

Para comenzar con el levantamiento del ambiente se necesitan tener instalado los siguientes programas:
1- El JDK de java en su versión 8.
2- Un servidor de base dato Postgresql-v12.
3- Como servidor de aplicaciones Wildfly19 aunque puede ser una superior.
4- Maven para la descarga de Jar necesarios.
5- Configurar variable de entorno de JAVA_HOME(para java) y de M2_HOME(para maven)

### Instalación 🔧

Se asume que el proceso lo realizará una persona con el nivel necesario para el levantamiento del proyecto.

Una vez se instale


## Despliegue 📦

_Agrega notas adicionales sobre como hacer deploy_

## Construido con 🛠️

Las tecnología utilizadas para el desarrollo, para el backend Java como leguaje de programación con la ayuda del framework de Spring Boot.
Para la capa del acceso a datos, se utilizó hibernate, jpql, repository y Postgresql como motor de base datos
Para la presentación se utilizó Jsf y Primefaces con la ayuda del modelo mvc del Spring Boot

## Versionado 📌

Versión 1.0.0 con fecha fin 03-10-2021

## Autores ✒️
Yoan Hernández Méndez
correo: yoanhmz@gmail.com
