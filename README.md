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
Debido a las caracteristicas particulares del proyecto y su ejecucion, se mantendra WhatsApp como canal principal para la interaccion con el sistema principal. Se construira un sistema agnostico que sea el encargado del procesamiento y consumo de datos compatible con el ecosistema SQL, asegurando la posibilidad de uso de diferentes herramientas de Data Analytics.

El primer objetivo es automatizar los procesos de recoleccion de datos e interaccion con los participantes de la red. Como objetivo mas inmediato se encuentra automatizar la recoleccion de datos.

El primer paso para conseguir dicho objetivo es construir un sistema que permita la automatizacion de respuestas a traves de la plataforma de WhatsApp, para eso se construira un programa que, de manera conversacional pueda recolectar los datos de cada voluntario y almacenarlo en una base de datos.

### Arquitectura propuesta
El sistema completo para el proyecto REDMOP se ha disenado con la premisa de conseguir escalabilidad en cada una de sus componentes, a continuacion se muestra un grafico que ilustra los diferentes componentes del sistema.

<p align="center">
  <img width="640" src="/architecture.png">
</p>