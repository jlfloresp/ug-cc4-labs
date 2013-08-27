---
layout: post
title:  "Laboratorio #6"
subtitle:  "JSON parser"
date:   2013-08-27 21:28:27
categories: labs
published: true
due_date: 2013-08-12
excerpt: Parser para JSON.
tags: antlr parser java json
---

Objetivos
---------
Para este laboratorio trabajaremos con un estandar de intercambio de datos llamado JSON (JavaScript Object Notation).  
Este esta basado en Javascript y es uno de los estandares mas utilizados por ser "open" y human-readable. Puede revisar más información sobre JSON [aquí](http://tools.ietf.org/html/rfc4627).

Los objetivos de la práctica son:
     
- Poner en práctica lo visto en clase acerca de analizadores sintácticos.
- Escribir un parser de ANTLR para JSON.
- Que practiquen un poco y se diviertan con Java, JSON y ANTLR ;)

---
Descripción
-----------
     
Usted debe hacer un análisis sintáctico sobre un archivo de input (por la linea de comandos) con extencion .json y desplegar en pantalla l que su programa reconoció.  
Utilice ANTLR para definir su parser (puede utilizar su lexer del laboratorio anterior). Incluya además un `Makefile` y siga la estructura de laboratorios que hemos estado utilizando (su paquete para este ejercicio seria `laboratorios.lab06[.paquetes_adicionales]`).  

A continuacion damos un ejemplo del parseo de un archivo JSON válido:

{%highlight json %}
{
	"nombre": "Homero J",
	"apellido": "Simpson",
	"age": 37,
	"direccion": {
		"calle": "Avenida siempre viva 17-42",
		"ciudad": "Springfield",
		"pais": "Estados Unidos de Norte America",
		"codigoPostal": "1513"
	},
	"numeroTelefonico": [
		{
			"tipo": "casa",
			"numero": "0555-1234"
		},
		{
			"tipo": "fax",
			"numero": "0555-4567"
		}
	]
}
{% endhighlight %}


---
Entrega
-------     

La entrega se realizará a través del `GES` antes de las 23:55:00 del día Lunes 2 de Septiembre de 2013, debe enviar un archivo llamado `carnet.zip` conteniendo el directorio lab06 que debe llevar todos sus archivos.

---