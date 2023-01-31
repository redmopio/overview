# Proyecto REDMOP

## Resumen
El proyecto REDMOP es un sistema de monitoreo climático distribuido que utiliza una red de voluntarios para recopilar datos sobre las condiciones meteorológicas en una zona geográfica específica. Los voluntarios comparten sus mediciones locales de lluvia a través de un sistema colaborativo, lo que resulta en una base de datos climática colectiva y distribuida. Este sistema puede ser utilizado para tomar decisiones y crear aplicaciones para diferentes usuarios interesados en la información climática en tiempo real.

## Estado actual
Actualmente, el proyecto REDMOP cuenta con un proceso de adquision de datos a traves de WhatsApp. Dicho proceso requiere de intervencion humana en dos etapas del proceso principal: Recoleccion de datos e interaccion con la red de voluntarios.

### Recoleccion de datos
La recoleccion de datos es el proceso por el cual un voluntario de la red comunica los resultados de su medicion en una ventana de tiempo.

### Interaccion con la red de voluntarios
La interaccion con la red de voluntarios hace referencia a los procesos por el cual, el sistema interactua con cada uno de los participantes de la red buscando perdurar la colaboracion activa de dicho voluntario en el proyecto REDMOP.

## Primera Propuesta Tecnica
La propuesta técnica del proyecto REDMOP consiste en utilizar la plataforma de WhatsApp como canal principal de interacción con los participantes de la red. Se busca construir un sistema que automatice los procesos de recolección y consumo de datos climáticos, asegurando la compatibilidad con el ecosistema SQL y la posibilidad de usar diferentes herramientas de Data Analytics.

Para lograr este objetivo, se construirá un programa que pueda recolectar los datos climáticos de manera conversacional a través de WhatsApp. Este programa tendrá una conversación con los voluntarios de la red para recopilar sus datos climáticos y almacenarlos en una base de datos.

En cuanto a la arquitectura de software, el sistema REDMOP estaría compuesto por los siguientes componentes:

1. Una interfaz de usuario conversacional que permita la recolección de datos climáticos a través de WhatsApp.

2. Un motor de procesamiento de datos que permita el tratamiento y análisis de los datos recopilados.

3. Una base de datos que almacene los datos climáticos y permita su acceso y análisis por parte de los interesados.

4. Un sistema de seguimiento y gestión de los voluntarios de la red, que permita conocer su actividad y garantizar la calidad de los datos recopilados.

Esta arquitectura de software permitiría construir un sistema eficiente y escalable que permita la recolección, procesamiento y análisis de datos climáticos de manera automatizada y distribuida.

### Arquitectura propuesta
El sistema completo para el proyecto REDMOP se ha disenado con la premisa de conseguir escalabilidad en cada una de sus componentes, a continuacion se muestra un grafico que ilustra los diferentes componentes del sistema.

<p align="center">
  <img width="640" src="/architecture.png">
</p>

#### Conversational Service
El servicio conversacional es el encargado de generar la interaccion en lenguaje natural con los voluntarios de la red. Este servicio se encarga de recibir los mensajes de los voluntarios y procesarlos para generar una respuesta, tambien en lenguaje natural, que permita al voluntario continuar con el proceso de recoleccion de datos.

#### RedMop System
El sistema REDMOP es el encargado de procesar los datos climaticos recopilados por los voluntarios de la red. Este sistema se encarga de almacenar los datos en una base de datos y de generar reportes de los datos recopilados.

#### WhatsApp Client
El cliente de WhatsApp es el encargado de interactuar con la plataforma de WhatsApp para enviar y recibir mensajes de los voluntarios de la red.

#### Telegram Client
El cliente de Telegram es el encargado de interactuar con la plataforma de Telegram para enviar y recibir mensajes de los voluntarios de la red.

#### Web Client
El cliente web permitira a los usuarios acceder a la informacion climatica recopilada por el sistema REDMOP a traves de una interfaz web.