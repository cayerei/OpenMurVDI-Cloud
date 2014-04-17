# Introducción #
![Openstack](./openstack.png) 

## Marco de realización ##
El **IES Ingeniero de la Cierva (Murcia)**, a través de su Departamento de Informática y Comunicaciones, durante el curso 2013-2014 ha llevado a cabo este proyecto, denominado **_OpenMurVdi: Despliegue de infraestructura de clientes ligeros orientados a Cloud Computing_**, al amparo de la convocatoria de realización de proyectos de innovación de formación profesional convocada, de forma conjunta por:

1. La Dirección General de Recursos Humanos y Calidad Educativa

2. La Dirección General de Formación Profesional y Enseñanzas de Personas Adultas

a través de la _Resolución de 25 de julio de 2013 por la que se regula el proceso de selección y de seguimiento para la realización de proyectos de innovación educativa realizados por el profesorado de formación profesional de la región de Murcia_.

Asimismo la _Resolución conjunta de 28 de noviembre de 2013_ de ambas direccione generales resuelve finalmente y de forma favorable para que se subvencione y desarrolle el presente proyecto si bien dotándole de un importe subvencionado de aproximadamente el 50% menos de lo inicialmente presupuestado.

## Motivación técnica ##
La principal motivación para el diseño y realización del presente proyecto, radica en:  

1. La gran evolución que han venido experimentando, en los últimos años, las tecnologías orientándose éstas hacia la utilización tanto de recursos de datos y como de aplicaciones en la _nube_. 

2. La expansión exponencial que se ha producido en el uso de dispositivos ligeros o incluso de terminales móviles para la utilización de estos recursos.

3. La necesidad, cada vez más imperiosa, en los centros educativos, de virtualizar, de forma centralizada, los sistemas tanto de explotación como de escritorio, para poder ampliar la vida útil del puesto de trabajo del usuario final.

4. La existencia tanto en plataformas propietarias como libres de plataformas de creación y gestión de _Cloud_ orientados a la virtualización centralizada.

5. La gran reducción de costes al utilizar plataformas libres como **OpenStack** para la implantación de virtualización centralizada frente a soluciones propietarias como VMWare o Citrix.

6. La carencia actual de sistemas de interconectividad en software libre que permitan, de forma ágil, desplegar infraestructuras de clientes ligeros con conectivdad a sistemas virtualizados en _Cloud Computing_ u _Openstack_ 

## Objetivos generales ## 

Así este proyecto se diseña tanto para cubrir objetivos técnicos como objetivos didácticos:

1. Obtener experiencias reales y de buenas prácticas para la utilización de clientes ligeros con conectividad a recursos en una _nube privada o Cloud Privado_ en el propio centro educativo.

2. Profundizar sobre la utilización de tecnologías de virtualización de sistemas de escritorios en entornos de _Cloud Computing_ a través de plataformas libres

3. Desplegar una infraestructura de clientes ligeros en entorno VDI para la conectividad a sistemas alojados en el _Cloud_

4. Desarrollar e implantar software intermedio denominado _"broker"_ con software libre 

5. Difundir las experiencias realizadas como la documentación técnica para su posterior reutilización por otros centros educativos u organismos interesados







# Objetivos específicos #

## Lineas directrices principales##
Atendiendo a las bases técnicas iniciales, el proyecto se ha llevado a cabo en base a 4 líneas directrices principales:

1. Partir de una infraestructura IaaS libre ya implantada (OpenStack en nuestro caso)
y convertirla a través de configuraciones y conectores en una plataforma DaaS
orientada a virtualización de escritorios.

2. Desarrollar y/o implantar un componente libre que sirva de punto de integración y
que actúe de “broker” central como eje para las conexiones multiprotocolo de los
clientes. Este componente será el que permita facilitar tanto a los administradores
para la gestión, como a los usuarios para la utilización de la infraestructura basada
en “Cloud” para VDI.

3. Provisión de métodos para que los clientes tengan facilidades de elección “on the
fly” de protocolos de acceso a sus escritorios virtualizados.

4. Implantación y despliegue de gestor integral de escritorios virtuales para clientes
ligeros VDI.

Estas lineas directrices se corresponden fundamentalmente con la bases técnicas para dar una respuesta a las deficiencias detectadas en las soluciones existentes de software libre para el despliegue de infraestructuras de VDI.

## Objetivos específicos ##

Los objetivos específicos planteados inicialmente se  relacionan  con las líneas directrices descritas y se pueden desglosar en:

1. Análisis exhaustivo y formación para profesores y alumnos en tecnologías de virtualización de escritorios y sus peculiaridades.

2. Convertir, a través de configuraciones y conectores existentes, una plataforma ya existente de _Cloud Computing_ basada en IaaS en una plataforma DaaS orientada a virtualización de escritorios VDI.

3. Desarrollar y/o implantar un componente libre que sirva de punto de integración y que actúe de _broker_ central como eje para las conexiones multiprotocolo de los clientes. Este componente será el que permita facilitar tanto a los administradores para la gestión, como a los usuarios para la utilización de la infraestructura basada en _Cloud_ para VDI.

4. Provisión de métodos para que los clientes tengan facilidades de protocolos de acceso a sus escritorios virtualizados.

5. Utilización con los alumnos de la infraestructura DaaS obtenida a través del _broker_ implantado.

6. Experiencia de prueba de uso de conexión al _broker_ implantado o desarrollado.

7. Realización de experiencia de conectividad con clientes ligeros tanto software como hardware (Ejemplo: dispositivos móviles, tablets, clientes ligeros tipo Raspberry Pi)

## Objetivos conseguidos ##

De los siete objetivos planteados al iniciar el proyecto, al finalizar éste se han conseguido seis de forma completa y uno de forma parcial. 

Unicamente **no se ha podido realizar la formación a profesores a través de un curso de formación** debido al **ajuste económico** realizado como consecuencia de la reducción del presupuesto a la hora de la adjudicación del proyecto.

Este objetivo de formación se ha sustituido por **tareas de investigación y auto estudio** por parte de los profesores participantes. 

Destacar que, aunque estas tareas no han podido suplir, al cien por cien, lo que se hubiese conseguido con un curso de formación específico, tanto para los profesores participantes en el proyecto como para los demás profesores del departamento, se ha podido llevar a término el proyecto gracias a la mayor dedicación en horas de investigación propia de los miembros participantes.












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








# Antecedentes y escenario inicial #

## Proyectos anteriores ##
El IES Ingeniero de la Cierva en colaboración con tres centros más:

+ IES Los Albares (Cieza-Murcia)

+ IES Gonzalo Nazareno (Dos Hermanas-Sevilla)

+ IES La Campiña (Arahal-Sevilla)

participó en el desarrollo y puesta en marcha del proyecto de innovación _“Implantación y puesta a punto de un cloud computing privado para despliegue de servicios en la nube”_ al amparo de la convocatoria que realizó el Ministerio de Educación y Ciencia en la _Resolución de 5 de abril de 2011 de la Secretaría de Estado de Educación y Formación_.

Este proyecto culminó satisfactoriamente en el tercer trimestre del curso 2011-2012 y como resultados destacables se pueden resaltar:

+ Un análisis y comparativa de las distintas soluciones en software libre de _“Cloud Computing”_

+ **Una implantación de infraestructura de _“Cloud Computing”_ basada en la solución libre OpenStack.**

+ La utilización de la infraestructura de _“Cloud Privado”_ en clase.

+ Formación del profesorado participante en tecnologías de _“Cloud Computing”_.

+ Elaboración de documentación técnica y manuales para su utilización en distintos módulos de los ciclos de la familia profesional de informática y comunicaciones

## Escenario inicial ##

Como resultado técnico más importante del proyecto anteriormente desarrollado cabe destacar el estudio, análisis y puesta en marcha funcional de un _“cloud privado”_ por cada centro participante.

Estos _“cloud privados”_ basados en la solución libre OpenStack permiten de forma nativa:

+ Centralización de máquinas virtuales que pueden albergar tanto sistemas operativos de entornos servidores (Linux Server o Microsoft Windows Server) como sistemas operativos de entornos clientes (Distribuciones Linux de Escritorio o Microsoft Windows Clientes tipo Windows XP, Windows 7, Windows 8...)

+ Acceso directo, por parte de alumnos y profesores desde PC's tradicionales, a las máquinas virtuales gestionadas por OpenStack. Estos accesos permiten a alumnos y profesores, de forma simultánea, la utilización de sistemas operativos de servidores y clientes virtuales con capacidades mucho más potentes que las propias que les ofrecen los equipos físicos de escritorio de los que se disponen habitualmente.

+ Facilidades de gestión centralizada, para los administradores, de los recursos virtualizados y de gestión de plantillas para ofrecer autoprovisionamiento a los usuarios.

Sin embargo actualmente ésta y otras **soluciones libres orientadas a IaaS no cuentan de forma nativa con**:

+ Infraestructura de gestión integrada y ágil de usuarios y perfiles asociados a recursos virtualizados.

+ Acceso descentralizado a través de soluciones que permitan elección “on the fly” de protocolos de acceso altamente compatibles como VNC, SPICE o Rdesktop. (Actualmente, en estas soluciones, los accesos automáticos a las máquinas virtuales se basan fundamentalmente en protocolo VNC, dejando la utilización de los otros protocolos para escenarios dónde el administrador debe realizar grandes labores de configuración para su utilización).

+ Gestión integral de escritorios virtuales para clientes ligeros VDI.

Esta situación se debe a que las infraestructuras libres IaaS aún centralizando los recursos virtualizados y pudiéndose convertir, a través de tareas de configuración, en plataformas DaaS, no están todavía adaptadas de forma nativa para despliegue completo de infraestructuras VDI.

