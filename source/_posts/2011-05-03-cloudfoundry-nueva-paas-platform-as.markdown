---
layout: post
title: "CloudFoundry: Nueva PaaS (Platform as a Service)"
date: 2011-05-03
comments: true
categories:
- cloud
- cloudfoundry
---
En el pasado mes de Abril, de la mano de [vmware](http://blogs.vmware.com/console/2011/04/cloud-foundry-delivering-on-vmwares-open-paas-strategy.html) y [springsource](http://blog.springsource.com/2011/04/12/launching-cloud-foundry/) nace una nueva solución en el mundo de la nube. Una solución [PaaS](http://en.wikipedia.org/wiki/Platform_as_a_service) que permite el despliegue de aplicaciones evitando la complejidad de las configuraciones hardware, software y servicios subyacentes necesarios para el correcto ciclo de vida de cualquier aplicación, desde su desarrollo hasta su puesta en marcha.

Pero... ¿qué es esto de la nube? Ciertamente el número de definiciones y conceptos es dispar. En muchos casos no se termina de tener una idea clara de ¿qué es la nube? Quizá por eso se denomine de forma tan difusa ;-).

En algunos casos ([Grid and Cloud Computing: A Business Perspective on Technology an Applications](http://books.google.es/books?id=TxOJI24idPYC&amp;pg=PA45&amp;lpg=PA45&amp;dq=grid+evolution+to+cloud&amp;source=bl&amp;ots=XVY-Q1c4Ef&amp;sig=h3HE7zT5mrnYt313_W7LvjmonJc&amp;hl=es&amp;ei=z4O-TdnYOYi38QOVpsW_BQ&amp;sa=X&amp;oi=book_result&amp;ct=result&amp;resnum=7&amp;ved=0CGIQ6AEwBg#v=onepage&amp;q=grid%20evolution%20to%20cloud&amp;f=false), por ejemplo) se ve el [Cloud Computing](http://en.wikipedia.org/wiki/Cloud_computing) como una evolución del [Grid Computing](http://en.wikipedia.org/wiki/Grid_computing") Y creo que no les falta razón. De hecho comparten muchos puntos en común en la orientación de su paradigma y con unas virtudes muy similares.

No prentendo hacer una comparativa en toda regla, ni mucho menos. No creo que tenga los conocimientos adecuados para hacer algo de semejante calado medianamente bien, prefiero traeros un artículo muy interesante donde realizan este análisis desde los distintos ángulos entre el Cloud Computing, Grid Computing y Distributed Systems: [Cloud Computing and Grid Computing 360-Degree Compared](http://arxiv.org/pdf/0901.0131)

En esta evolución, no son pocos los movimientos que se vienen desarrollando en este tipo de plataformas. Véase como ejemplo:
- [Amazon Web Services](http://aws.amazon.com/es/)
- [Google App Engine](http://code.google.com/appengine/)
- [Azure](http://www.microsoft.com/windowsazure/)
- [Heroku](http://www.heroku.com/)
- [IBM SmartCloud](http://www.ibm.com/cloud-computing/us/en/#%21paas)
- [CloudControl](http://cloudcontrol.com/php-cloud-platform-as-a-service-en/)

Pero hay algo que, a mi parecer, hace a [CloudFoundry](http://www.cloudfoundry.com/) algo diferente.

1. *Proyecto Open Source*: [www.cloudfoundry.org](http://www.cloudfoundry.org/"). El código está disponible en [https://github.com/cloudfoundry](https://github.com/cloudfoundry) Y esto hace que sea muy muy interesante.
2. Sin restricciones en los frameworks soportados.
3. Cloud Foundry Micro Cloud. Previo registro nos pueden habilitar una micro nube descargable de forma que podamos hacer nuestras pruebas en nuestros propios entornos. Nos da la capacidad de tener PaaS en una de nuestras máquinas.

Definitivamente creo que springsource y vmware han hecho un movimiento muy inteligente a la hora de proporcionar una plataforma tan abierta. En su  [FAQ](http://www.cloudfoundry.com/faq) justifican y detallan esta elección.

Esto es lo que se puede ver a simple vista. Espero poder entrar en mayor detalle según me acerque a las plataformas con ejemplos sencillos que nos permitan conocer mejor sus características y modos de uso.
