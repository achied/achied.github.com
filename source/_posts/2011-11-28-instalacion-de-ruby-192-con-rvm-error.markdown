---
layout: post
title: "Instalación de ruby 1.9.2 con rvm: Error en yaml-0.1.4"
date: 2011-11-28
comments: true
categories:
- ruby
- yaml
- rvm
---
Enredando estos días con [cloudfoundry](https://github.com/achied/vcap) uno de los elementos que instala y configura es [rvm](https://rvm.beginrescueend.com/) un sistema de gestión de versiones de ruby y sus gemas. Muy útil a la hora de estar con desarrollos donde las dependencias y las versiones son dispares. Permite aislar los entornos y adaptarlos de forma personalizada, elegir la versión de ruby más adecuada, construir un grupo de gemas específico para cada entorno, ...

Después de haber instalado rvm la compilación de ruby nos da un error extraño

![error_yaml](http://2.bp.blogspot.com/-2dpmYu1N5FA/Tsue5q_IbvI/AAAAAAAAAUs/4EFll10IDKg/s1600/error_yaml.png "error de configuración y compilación de yaml-0.1.4")

Para solucionar este pequeño inconveniente realizamos los siguientes pasos:

<!-- more -->

Instalamos libtool, en el caso de no tenerlo instalado

```
apt-get install libtool
```

Entramos dentro del directorio donde están las fuentes de yaml

``` 
cd .rvm/src/yaml-0.1.4/
```

Eliminamos los ficheros generados de forma errónea

```
rm aclocal.m4
rm config/ltmain.sh
```
Volvemos a reconfigurar para generar los ficheros eliminados de forma adecuada
    
```
autoreconf
```

![autoreconf_yaml](http://1.bp.blogspot.com/-VSsXdSwzuEk/TsvBQdn9f-I/AAAAAAAAAU4/8ToPaH3mWkY/s1600/autoreconf_yaml.png "reconfiguración de yaml")

Y reinstalamos la versión de ruby

```
rvm install 1.9.2-p180
```

Al  final tenemos nuestra versión 1.9.2-p180 funcionando correctamente y sin problemas

![yaml_solucionado](http://3.bp.blogspot.com/-8r2q5_6j5cg/TsvBv9kzOQI/AAAAAAAAAVI/BysWMW2ek_A/s1600/yaml_solucionado.png "Instalación correcta")
