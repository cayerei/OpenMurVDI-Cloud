# Descripción del proyecto #

Este proyecto denominado _OpenMurVdi: Despliegue de infraestructura de clientes ligeros orientados a Cloud-Computing_ se encuadra dentro del marco tecnológico actual dónde se prima la utilización de dispositivos clientes ubicuos y de capacidad de procesamiento limitado junto con la conectividad a recursos de datos y de procesamiento de gran productividad en la _nube_.

En este sentido las tecnologías _orientadas a la nube_ y la expansión de dispositivos y hardware de clientes móviles y ligeros, se ven, sin embargo, contrapuestas a la creciente demanda de recursos, en la parte cliente, de los nuevos sistemas operativos orientados al usuario. 

Para salvar esta brecha entre dispositivos ligeros o _Thin Clients_ y la alta demanda de recursos de los sistemas operativos de escritorio modernos (MS Windows7-8, MS Windows Server, Ubuntu 14.04, Ubuntu Server...) se plantea utilizar una infraestructura híbrida de _Cloud Computing_ dónde se ejecuten  remotamente los sistemas operativos pesados complementada con un despliegue de clientes ligeros (con mínimos recursos: Raspberry Pi, equipos antiguos, tecnologías móviles)  que sirvan de meros dispositivos de conexión con estos sistemas operativos en el _Cloud_.

Así este proyecto se vertebra sobre **tres tecnologías complementarias**:

1. **Clientes ligeros o Thin Clients**

2. **Tecnología de _Cloud Computing_ orientadas a _IaaS_ o _DaaS_** dónde se ejecutan los sistemas operativos virtualizados

3. **Tecnología de _VDI(Virtualización de Escritorios)_** que es la parte que permite al usuario conectarse con los sistemas operativos virtualizados.

## Clientes ligeros o Thin Clients ##
Un cliente ligero (Thin Clients o slim client en inglés) es un ordenador cliente o un software de cliente en una arquitectura de red que depende primariamente del servidor central para las tareas de procesamiento, y se encarga principalmente en
transportar la entrada y la salida entre el usuario y el servidor remoto, siendo totalmente dependiente del servidor.

Ejemplos de posibles clientes ligeros: Raspberry Pi, móviles _smartphones_, tablets, sistemas operativos ligeros en equipos obsoletos, etc...

En contraste, un cliente pesado realiza tanto procesamiento como le sea posible y transmite solamente los datos para las comunicaciones y el almacenamiento al servidor siendo autónomo incluso sin la presencia de servidor.


## Cloud Computing: IaaS vs DaaS##

### IaaS: Infraestructure as a Service ###
La evolución de la infraestructura clásica de servidores físicos en las empresas, sustituyéndolos por servidores virtuales con ubicación en la propia empresa o Internet. Destaca en este ámbito la implementación comercial Amazon EC2 (Elastic Compute Cloud) y las implementaciones de software libre OpenSatck y Eucalyptus, que son compatibles con el API de Amazon EC2, pero que permiten un control total sobre la tecnología.

### DaaS: Desktop as Service as a Service ###
Hace referencia a la arquitectura de cloud computing orientada a ofrecer a los clientes escritorios virtualizados como servicio. Funcionalmente es similar a VDI, pero en cuanto a terminología se centra más en las necesidades, requisitos e implantación de la parte servidor.

## VDI (Virtualización de Escritorios) ##
Esta parte junto al DaaS de la parte servidora es la parte que permite ofrecer a los usuarios la conectividad a los escritorios virtualizados en la nube.

Se hace referencia al proceso de separación entre el escritorio, que engloba los datos y programas que utilizan los usuarios para trabajar, de la máquina física. El escritorio _virtualizado_ es almacenado, por lo tanto, remotamente en la infraestrucura de la nube, implantada como DaaS, en lugar de en el disco duro del ordenador personal. 

Esto significa que, en este escenario, cuando los usuarios trabajan en su escritorio, todos sus programas, aplicaciones, procesos y datos se almacenan y ejecutan centralmente, permitiendo a los usuarios acceder remotamente a sus escritorios
desde cualquier dispositivo capaz de conectarse remotamente al escritorio, tales como un portátil, PC, o cliente ligero.

Un aspecto importante de este marco tecnológico es que se procede a virtualizar todo el escritorio para ofrecérselo a los clientes. De esta forma cada cliente ligero puede acceder de forma remota a su propio escritorio/sistema (o a varios de ellos) de manera diferenciada del resto de clientes.

Además también se permite que el escritorio virtualizado pueda tener persistencia a lo largo de las distintas conexiones/desconexiones realizadas.








