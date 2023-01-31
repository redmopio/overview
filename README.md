# Proyecto REDMOP

## Definiciones
A continuacion se describen los conceptos mas importantes del proyecto REDMOP.

### Red de Monitoreo Participativo (REDMOP)
La red de monitoreo participativo es una red de personas voluntarias, distribuidas a lo largo de un determinado espacio geografico, y que comparten los resultados de sus mediciones de lluvia locales a traves de un sistema de agregacion colaborativa.

Al tener esta red distribuida de voluntarios que recolectan datos fluviales, contamos con una base de datos colaborativa que se puede usar para toma de decisiones y la creacion de aplicaciones paa diferentes usuarios interesados en la informacion en tiempo real de las condiciones fluviales de dicho espacio geografico.

## Estado inicial
Actualmente, el proyecto REDMOP cuenta con un proceso de adquision de datos a traves de WhatsApp. Dicho proceso requiere de intervencion humana en dos etapas del proceso principal: Recoleccion de datos e interaccion con la red de voluntarios.

### Recoleccion de datos
La recoleccion de datos es el proceso por el cual un voluntario de la red comunica los resultados de su medicion en una ventana de tiempo.

### Interaccion con la red de voluntarios
La interaccion con la red de voluntarios hace referencia a los procesos por el cual, el sistema interactua con cada uno de los participantes de la red buscando perdurar la colaboracion activa de dicho voluntario en el proyecto REDMOP.

## Primera Propuesta Tecnica
Debido a las caracteristicas particulares del proyecto y su ejecucion, se mantendra WhatsApp como canal principal para la interaccion con el sistema principal. Se construira un sistema agnostico que sea el encargado del procesamiento y consumo de datos compatible con el ecosistema SQL, asegurando la posibilidad de uso de diferentes herramientas de Data Analytics.

El primer objetivo es automatizar los procesos de recoleccion de datos e interaccion con los participantes de la red. Como objetivo mas inmediato se encuentra automatizar la recoleccion de datos.

El primer paso para conseguir dicho objetivo es construir un sistema que permita la automatizacion de respuestas a traves de la plataforma de WhatsApp, para eso se construira un programa que, de manera conversacional pueda recolectar los datos de cada voluntario y almacenarlo en una base de datos.

