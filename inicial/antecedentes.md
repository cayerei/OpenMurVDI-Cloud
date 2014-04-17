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

