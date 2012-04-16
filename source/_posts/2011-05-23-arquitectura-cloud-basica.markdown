---
layout: post
title: "Arquitectura Cloud básica"
date: 2011-05-23
comments: true
categories:
- cloud
- paas
- iaas
- saas
---
Es irónico pero, despúes de empezar a hablar de las bondades del Cloud y definir los elementos de su arquitectura básica, [a blogger le dio por caerse](http://status.blogger.com/2011/03/postmortem-for-blogger-service.html "a blogger le dio por caerse") a blooger le dio por caerse. También se fastidió mi último post y algunos de mis borradores.

Eso me pasa por no tomar la medidas que hay que tomar en cualquier entorno:

- Copias de seguridad
- Plan de contingencia

Y es que en el Cloud no existe la magia y hay que tener en cuenta que las ventajas exponenciales que se pueden experimentar y pueden ofrecer a usuarios y desarrolladores crecen de igual forma en la complejidad de su gestión y mantenimiento.

Así que para enmendar mi torpeza haré un breve resumen de lo que presentaba en la última entrada.

##Arquitectura Cloud básica

Los elementos fundamentales de la arquitectura cloud no difieren mucho de aquellos que tradicionalmente conocemos. Antes de desplegar ningún tipo de servicio o desarrollo, es preciso disponer de una plataforma que nos ofrezca los recursos necesarios para el ciclo de vida completo de nuestra aplicación: Un contenedor de ejecución, una fuente de acceso a datos, ... Y esta plataforma, a su vez, ha de descansar en alguna infraestructura que le ofrezca los recursos de cómputo, memoria, red...

*Un ejemplo concreto tradicional*
Servicio: Una página web
Plataforma: Una base de datos
Infraestructura: Un PC o servidor

Evidentemente la evolución de la tecnología y de la mano de la [virtualización](http://es.wikipedia.org/wiki/Virtualizaci%C3%B3n) provocado la revolución de las arquitecturas tradicionales. Escalabilidad, Disponibilidad, Redundancia, Balanceo de Carga, ... vuelven a ser conceptos conocidos que están subiendo de escalafón constantemente.

![cloud stack](http://2.bp.blogspot.com/-zRyG1sLvAeA/TjujH40YG6I/AAAAAAAAAT8/4Cg4d9aygMI/s1600/cloud_stack.gif, "cloud stack")

###SaaS
Se trata de la capa más externa, destinada al usuario final, principalmente. Es el Software como Service (Software as a Service). En esta capa se dan servicios de lo más vario pinto. Desde servicios de correo electrónico, álbumes de fotos, gestión de contactos, gestión de proyectos... hasta servicios que nos ofrecen almacenamiento. En este plano nos encontramos con [gmail](http://www.gmail.com/), [flickr](http://www.flickr.com/), [salesforce](http://www.salesforce.com/),[teambox](http://teambox.com/) y [dropbox](http://www.dropbox.com/) por poner algunos ejemplos.

###PaaS
Se trata de la capa intermedia y que cada vez está adquiriendo más importancia. Fundamentalmente desde el punto de vista de los desarrolladores. Es la Plataforma como Service (Platform as a Service). En esta capa encontramos los recursos necesarios para poder desplegar nuestras aplicaciones (nuestros servicios). Algunas referencias tenemos en [Google App Engine](http://code.google.com/appengine/), [Azure](http://www.microsoft.com/windowsazure/), [Heroku](http://www.heroku.com/) ...

El pasado mes de Abril entró en juego una solución promovida por [VMWare](http://www.vmware.com/) de la que hablé en [CloudFoundry: Nueva PaaS (Platform as a Service)](http://edachi.blogspot.com/2011/05/cloudfoundry-nueva-paas-platform-as.html).

Ya hablaba del vértigo que estaba despertando la plataforma y las numerosas aportaciones para soportar PHP y Erlang. Otra muestra es un fork reciente para dar soporte a aplicaciones Python y Perl, llamado [Stackato](http://www.activestate.com/blog/2011/05/stackato-platform-python-and-perl-cloud). Esto es una muestra más del incentivo que supone disponer de soluciones abiertas y la garantía de calidad y competitividad en el mercado.

###IaaS
Se trata de la capa que gestiona la infraestructura como un servicio (Infrastructure as a Service). Es aquí donde se realiza la provisión de los recursos de bajo nivel, número de procesadores, cantidad de memoria, almacenamiento, ancho de banda... incluso el sistema operativo que será el último estrato de recubrimiento del servicio. Servicios de infraestructura encontramos en [Amazon](http://aws.amazon.com/), [RackSpace](http://www.rackspace.com/), [GoGrid](http://www.gogrid.com/index.v2.php), ...

[De la mano de RackSpace](http://www.genbeta.com/actualidad/openstack-cloud-computing-de-codigo-abierto) disponemos de una solución libre, [OpenStack](http://www.openstack.org/).  Una solución que está adquiriendo un protagonismo importante. Muestra de ello es [la elección de Ubuntu como plataforma Cloud](http://cloud.ubuntu.com/2011/03/coming-up-in-openstack-cactus%E2%80%A6/) para su paquetería de la nube en lugar de [Eucalyptus](http://www.eucalyptus.com/), como venía haciendo en versiones anteriores.

Como se puede apreciar, cada vez son más las soluciones y opciones en este nuevo reto. Medios de difusión, estrategias de mercado y apuestas innovadoras por parte de organizaciones grandes y pequeñas están despejando un camino que deja de estar tan en el aire como cabría pensar.

Esta vorágine aumenta el desafío constante de los usuarios, responsable e ingenieros de TI que vuelven a ver cómo se pone patas arriba los procedimientos y protocolos tradicionales de desarrollo, despliegue y aprovisionamiento. Uno experimenta la sensación de que... después de todo lo aprendido, volvemos a estar como al principio... aprendiendo.

Por esta razón trataré de hacercarme a las distintas capas con alguna prueba de concepto para conocer algo más de este nuevo mundo (si no pierdo más posts :D )

Siguiente parada... OpenStack.
