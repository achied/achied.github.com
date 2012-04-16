---
layout: post
title: "Tanto leer y tan poco escribir!!!"
date: 2011-11-18
comments: true
categories:
- openstack
- cloud
- paas
- stackato
- iaas
- cloudfoundry
- stackops
---
Hace no mucho tiempo, comencé con mucha ilusión este blog. Decidí concentrar los primeros artículos sobre soluciones Cloud que a mi juicio aparecían de forma emergente en la mayoría de las noticias que iba leyendo. Conseguí hacer algún breve resumen, de forma introductoria, para luego poder profundizar de forma más detallada. Fue en este punto cuando empecé a entrar en una doble espiral:

1. Quería escribir un artículo sobre los componentes fundamentales y su instalación
2. Quería hacerlo perfecto

Entrar en detalle sobre algo que estás empezando a conocer... lleva tiempo y si encima quieres hacerlo perfecto y nunca terminan de gustarte los innumerables borradores que vas escribiendo...

Ahora no es que esté en mejores condiciones de abordar esta tarea, es que he decido escribir lo que sé y como lo sé. De forma sencilla, compartir aquello que ha sido capaz de captar mi atención y ha sido relevante para mí.

Por eso, en este artículo, serán muchas las referencias a un tiempo extenso y próspero de búsquedas y lecturas intensas. Como resultado, mencionar y enlazar aquellas cosas que otros me han mostrado y ... ¿para qué repetirlo si ellos lo han hecho y lo han hecho bien?

Han sido dos los proyectos que me han enganchado desde el primer momento:

* [OpenStack](http://www.openstack.org/)
* [CloudFoundry](http://cloudfoundry.org/)

Empecé con el primero haciendo las primeras instalaciones en base a varios artículos y documentaciones

* [OpenStack Beginner's Guide for Ubuntu 11.04](http://cssoss.wordpress.com/2011/04/20/openstack-beginners-guide-for-ubuntu-11-04-natt-narhwal/)
* [OpenStack Compute Installation Using VirtualBox, Vagrant and Chef](http://docs.openstack.org/cactus/openstack-compute/admin/content/openstack-compute-installation-using-virtualbox-vagrant-and-chef.html)

Artículos que ha sido de provecho pero que hay que ir complementando debido a la nueva versión liberada a finales de Septiembre, [Diablo Release](http://www.openstack.org/projects/compute/).

Quiero hacer una mención especial de [Stackops](http://www.stackops.com/) empresa española de referencia en la comunidad como lo constatan sus [participaciones](http://www.nubeblog.com/2011/10/03/en-la-openstack-conference-en-boston/) y sus [reconocimientos](http://www.bio-tecnologia.es/es/noticia.cfm?id_item=1839&amp;apartado=1).

No han sido pocas las noticias sobre la evolución del proyecto y la cantidad de compañías que se han ido adhiriendo a la marcha del mismo:

* [Cannonical](http://blog.canonical.com/2011/02/03/canonical-joins-the-openstack-community/)
* [Cisco](http://blogs.cisco.com/news/cisco-joins-openstack-community/)
* [Dell](http://www.zdnet.co.uk/news/cloud/2011/07/27/dell-launches-openstack-cloud-infrastructure-product-40093534/)
* [Piston](http://www.pistoncloud.com/)
* [HP](http://h30507.www3.hp.com/t5/Data-Central/HP-Announces-Support-for-OpenStack/ba-p/96283)
* [Suse](http://lxnews.org/2011/11/01/suse-joins-openstack/)
* [Stackato](http://www.activestate.com/blog/2011/10/infrastructure-agnostic-paas-why-we-joined-openstack-and-ova)
* ... [y muchos otros](http://www.openstack.org/community/companies/)

Su arquitectura sigue en evolución. Muestra de ello es el número de proyectos que están naciendo alrededor del proyecto añadiendo un valor muy interesante:

* [Quantum](http://wiki.openstack.org/Quantum)
* [Dashboard](http://wiki.openstack.org/OpenStackDashboard)
* [KeyStone](https://launchpad.net/keystone)

En la página principal del proyecto podemos ver una [referencia completa](http://www.openstack.org/projects/)

En cuanto a [CloudFoundry](http://cloudfoundry.org/) la cosa ha sido más vertiginosa si cabe, dado que he decidido hacer una apuesta personal por este proyecto siguiendo las líneas de desarrollo más de cerca. En muy poco tiempo se ha ido añadiendo soporte para muchos entornos y servicios. Entre los más destacados

* [Soporte para Python](http://blog.cloudfoundry.com/post/9374366916/cloud-foundry-adds-php-and-python-through-community)
* [Soporte para PHP](http://blog.cloudfoundry.com/post/9374366916/cloud-foundry-adds-php-and-python-through-community)
* Soporte para Neo4J
* Pendiente la [aprobación de Mono](https://github.com/cloudfoundry/vcap/pull/139)

Salen a escena [AppFog](http://www.appfog.com/) y [ActivateState](http://www.activestate.com/) ofreciendo sus esfuerzos llevándose como galardón el rol de _[Community Lead](http://cloudfoundry.org/leads)_ en sus respectivos campos. Recientemente [Joyent](http://www.joyent.com/) ha sido nombrado Community Lead para el soporte de Node.js

Numerosos los eventos y artículos relacionados con el proyecto, numerosas las iniciativas y esto sigue sin parar.

* [CloudFoundry deployment with Chef](http://blog.cloudfoundry.com/post/10816758982/using-chef-to-customize-multi-node-cloud-foundry)
* [CloudFoundry deployment with Puppet](http://www.kartar.net/2011/05/install-cloud-foundry-vcap-via-puppet/)
* [CloudFoundry deployment with Ensemble](http://blog.xtremeghost.com/2011/09/from-zero-to-drawbridge-via-ubuntu.html?m=1)

Aún queda mucho por aprender y mucho por seguir leyendo. Pero es de agradecer la cercanía y disposición que te prestan cuando muestras interés por colaborar.

Hasta aquí un breve resumen de todo este tiempo y la andadura por muchas tecnologías y conocimientos paralelos: Chef, Puppet, Rvm, Ruby, Rails, Vagrant, Nats, New Relic, Collectd, CEP, CEE... y un largo etcétera.

A partir de aquí tomaré la determinación de ir poniendo posts más breves, y no queriendo ser tan perfeccionista y organizado. Al final se trata de mostrar lo que sé y como lo sé. Ir compartiendo lo cotidiano de mi trabajo e inquietudes al ritmo al que se van presentando. Puede que sea menos atractivo pero desde luego es mucho más cercano y coherente.
