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

![Image of Emerginov simple](https://raw.githubusercontent.com/arnaudmorinol/emerginov-vnf/master/docs/image1.png)

TODO: mettre une autre photo/schéma d'une gateway?

The gateway can communicate with a telecom network through multiples mecanism:

* For voice
  * T2/E1 connection
  * SIP Trunk
* For SMS
  * SMSC connection
  * SMS modem

## Architecture
### Functional architecture

![Image of Emerginov functions](https://raw.githubusercontent.com/arnaudmorinol/emerginov-vnf/master/docs/image3.png)

### Simple flow architecture

![Image of Emerginov architecture](https://raw.githubusercontent.com/arnaudmorinol/emerginov-vnf/master/docs/archi_dev_simple.png)

### Software architecture
![Image of Emerginov architecture](https://raw.githubusercontent.com/arnaudmorinol/emerginov-vnf/master/docs/archi_vm.png)

### Gateway

## Installation

Full install is on: http://emerginov.ow2.org/xwiki/bin/view/Support/Installation+Guide+Standard

### Procedure
1. Start by deploying Gardien:
 * Add a Personal Package Archive from Launchpad
 * Install emerginov-master package
 * Run emerginov-update (automation needed)
 * Run emerginov-init (automation needed)
 * Edit config file (automation needed)
 * Install emerginov-agent
 * Run emerginov-apply
 * Sign certificate with puppet (automation needed)
 * Run again emerginov-apply
1. Continue with Routing
 * Install emerginov-agent
 * Run emerginov-apply
 * Sign certificate with puppet (automation needed)
 * Run again emerginov-apply
1. Then dev
 * idem as routing
1. Then content
 * idem as routing
1. Then gateway
 * idem as routing
1. Test

### Needs
* Need 2 networks 
 * Public on routing
 * Private on all machines

### Orchestration possibility
#### Scale
* Add a Dev VM to have more projects in the emerginov platform
 * Need some configuration in content and routing

#### Heal
To be conforted

