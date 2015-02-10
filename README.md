#Emerginov VNF
## Intro

Emerginov is a platform that help developers build **web & telecom** applications.

By web, we mean that Emerginov let developers build web pages by providing a **PHP web server hosting** infrastructure.

By telecom, we mean that developers will also have access to **RESTfull API** such as:

 * receiving & sending SMS
 * receiving & making calls
 * etc.

It's aim is to simplify creation of application that needs to use such telecoms API.

For example, it can be used as a backend for Internet of Things (Objets Connectés). It may also be used to create vocal kiosk or SMS based applications.

### Free software
Note that the platform is built with 100% of free software, and the code source to deploy a new platform can easily be downloaded from http://emerginov.ow2.org
 
## A bridge between telecom & web

In a very basic view, Emerginov can be seen a web server to serve multiple PHP/HTML/CSS/Javascript applications. But it also provide a way to these applications to communicate with users on mobile phones (SMS & voice).

To do so, the platform is extended with a **Gateway**.

TODO: mettre une photo/schéma d'une gateway?

![Image of Emerginov simple](/docs/archi_reseau.png)

The gateway can communicate with a telecom network throuhg multiples mecanism:

* For voice
  * T2/E1 connection
  * SIP Trunk
* For SMS
  * SMSC connection
  * SMS modem

## Architecture
### Functional architecture
TODO : mettre le schéma de la page 4 emerginov presentation light
### Simple flow architecture
TODO: mettre schéma archi_dev_simple.png

### Software architecture
TODO : mettre un schéma ou on retrouve les principaux softs dans des VM, idéalement avec les flux entre les softs

TODO : mettre aussi un schéma des VM pour les identifier

### Gateway

## Installation
5 machines to deploy through puppet
Need 2 networks (pub & priv)
automatic deployment
quand meme besoin d'ordonner un peu
faire un fichier de conf
voir pour le healing
voir pour le dimensionnement et l'intégration de nouvelles machines
ca va etre rigolo ya un peu de conf à faire
