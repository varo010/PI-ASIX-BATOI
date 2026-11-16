# 7.6. Catálogo inicial de requisitos (B6)

Cada requisito sale de una o varias necesidades de B3 y tiene su misma prioridad (la más alta, si cubre varias). Ninguno impone una marca o tecnología concreta.

## 7.6.1. Requisitos funcionales

Indican qué deberá hacer el sistema.

**Tabla 8.** Requisitos funcionales

| Código | Requisito | Necesidad que cubre | Prioridad |
|---|---|---|---|
| RF-01 | El sistema deberá permitir la autenticación centralizada de los usuarios, con una cuenta personal para cada trabajador. | N-14 · Autenticación centralizada y control de accesos | Alta |
| RF-02 | El sistema deberá permitir asignar permisos por departamento y por puesto, y retirar todos los accesos de una persona cuando deja la empresa, en menos de 15 minutos desde que se desactiva su cuenta. | N-14 · Control de accesos; N-13 · Documentación con acceso restringido | Alta |
| RF-03 | El sistema deberá permitir compartir documentación en carpetas por departamento y entre los departamentos que trabajan juntos, con acceso solo para quien la necesita, incluida una carpeta restringida para la asesoría y el auditor. | N-13 · Documentación compartida con acceso restringido | Alta |
| RF-04 | El sistema deberá permitir gestionar un único catálogo multimarca (fichas, precios y stock) del que salgan los datos de todos los marketplaces, sin duplicar ficheros. | N-10 · Catálogos multimarca y multicanal | Alta |
| RF-05 | El sistema deberá disponer de una aplicación web interna para consultar y actualizar el stock y el estado de los pedidos desde las oficinas y desde el almacén. Un cambio hecho en un puesto deberá verse en los demás en menos de 1 minuto. | N-11 · Consulta de stock y pedidos en el almacén; N-12 · Estado de los pedidos | Alta |
| RF-06 | El sistema deberá permitir registrar las incidencias y devoluciones de los pedidos y seguir su estado hasta cerrarlas. | N-12 · Gestión de incidencias | Alta |
| RF-07 | El sistema deberá almacenar en una base de datos centralizada el catálogo, el stock, los pedidos y las ventas de todos los canales. | N-05 · Datos de ventas centralizados; N-10; N-11 | Alta |
| RF-08 | El sistema deberá generar informes y cuadros de mando de ventas y tesorería para Dirección y Administración y finanzas, a partir de los datos bancarios y contables, que se incorporarán de forma automática al menos una vez al día. | N-01 · Información para decidir; N-02 · Cuadros de mando; N-05 | Alta |
| RF-09 | El sistema deberá calcular previsiones de aprovisionamiento a partir de las ventas y del stock. | N-06 · Previsión de aprovisionamiento | Alta |
| RF-10 | El sistema deberá permitir seguir la mercancía en tránsito y guardar la documentación de los envíos al extranjero. | N-08 · Mercancía en tránsito; N-07 · Documentación aduanera | Alta |
| RF-11 | El sistema deberá permitir registrar las marcas cliente y el seguimiento comercial de cada una, también desde fuera de la oficina. | N-04 · Seguimiento comercial en movilidad | Alta |
| RF-12 | El sistema deberá permitir el acceso remoto a los servicios internos solo a los usuarios autorizados, con su cuenta personal y con la conexión cifrada. | N-01 · Acceso remoto; N-04 | Alta |
| RF-13 | El sistema deberá permitir registrar la jornada de cada trabajador y consultar ese registro desde un portal del empleado. | N-03 · Portal del empleado y control de horarios | Media |
| RF-14 | El sistema deberá permitir supervisar el estado de servidores y dispositivos de red y avisar automáticamente a Sistemas (D9) en menos de 5 minutos cuando algo falle. | N-09 · Monitorización de red y servidores | Alta |
| RF-15 | El sistema deberá hacer copias de seguridad automáticas de los datos al menos una vez al día, conservar las de los últimos 7 días, permitir restaurarlos y comprobar cada mes que la restauración funciona. | N-16 · Copias de seguridad | Alta |
| RF-16 | El sistema deberá ofrecer acceso a Internet a los visitantes sin darles acceso a ningún recurso interno. | N-15 · Separación del tráfico de invitados | Media |
| RF-17 | El sistema deberá permitir la comunicación interna entre todos los departamentos, y en especial entre las oficinas y el almacén, mediante un canal de comunicación interno accesible con la cuenta de cada trabajador. | N-11 · Stock y pedidos en el almacén; N-12 · Estado de pedidos e incidencias (B3, necesidad general 3; B4, MI-3) | Alta |

## 7.6.2. Requisitos no funcionales

Indican cómo debe comportarse el sistema o qué características generales debe tener.

**Tabla 9.** Requisitos no funcionales

| Código | Requisito | Necesidad que cubre | Prioridad |
|---|---|---|---|
| RNF-01 | La red deberá estar segmentada para separar oficinas, almacén, servidores e invitados, de forma que un fallo o una infección en una zona no se extienda al resto. | N-15 · Separación lógica del tráfico | Media |
| RNF-02 | Toda la zona de trabajo del almacén deberá tener cobertura inalámbrica para los lectores. | N-11 · Cobertura en el almacén | Alta |
| RNF-03 | Los equipos críticos deberán seguir funcionando durante un corte eléctrico de al menos 10 minutos y apagarse de forma ordenada si el corte dura más. | N-16 · Protección frente a cortes eléctricos | Alta |
| RNF-04 | Los servicios críticos deberán disponer de medidas frente a fallos: la avería de un solo equipo o disco no deberá provocar pérdida de datos, y habrá una copia fuera de la sede, actualizada al menos una vez a la semana. | N-16 · Pérdida de datos | Alta |
| RNF-05 | Los servicios de stock y pedidos deberán estar disponibles al menos el 99 % del horario del almacén, medido cada mes, y ninguna caída deberá durar más de 1 hora. | N-09 · Caídas que paralizan la logística; N-11 | Alta |
| RNF-06 | La información económica, la de las marcas y los datos personales solo deberán ser accesibles a los perfiles autorizados, cumpliendo el RGPD. Las cuentas con acceso a esa información usarán un segundo paso de verificación y quedará registro de los accesos. | N-13 · Fugas de información; N-14 | Alta |
| RNF-07 | La aplicación interna deberá poder usarse desde los puestos de oficina, los lectores del almacén y los dispositivos móviles del equipo comercial. | N-04; N-11; N-12 | Alta |
| RNF-08 | El sistema deberá facilitar la monitorización y el mantenimiento desde un punto central: Sistemas (D9) deberá poder ver el estado de servidores, red y servicios y administrarlos sin desplazarse a cada equipo. | N-09 · Detectar fallos a tiempo | Alta |
| RNF-09 | La infraestructura deberá estar correctamente documentada (equipos, red, servicios, usuarios y procedimientos de copia y restauración), y la documentación se actualizará con cada cambio para que cualquier miembro de D9 pueda mantenerla. | N-09 · Mantenimiento del sistema | Alta |
| RNF-10 | El registro de jornada deberá cumplir la normativa laboral de fichaje: guardar la hora de inicio y de fin de cada jornada de cada trabajador, conservar los registros 4 años y tenerlos a disposición de los trabajadores, de sus representantes y de la Inspección de Trabajo (art. 34.9 del Estatuto de los Trabajadores, F8). | N-03 · Sanciones por incumplir el fichaje | Media |
| RNF-11 | El sistema deberá permitir futuras ampliaciones (más trabajadores y terminales en campaña, más marcas, canales y datos, o una segunda nave) sin tener que rehacer la red ni los servidores: se deberán poder añadir puestos, dispositivos y servicios sin modificar los que ya funcionan. | N-10 · Más marcas y canales; N-11 · Más pedidos en el almacén (B4, P6 y MI-7) | Alta |

## 7.6.3. Tabla de requisitos

Todos los requisitos del catálogo en una sola tabla. Los funcionales llevan el código **RF** y los no funcionales, **RNF**. La necesidad se indica siempre con su código y su nombre de B3, y la prioridad es la de esa necesidad (la más alta, si cubre varias). La última columna, **«Cómo se comprueba»**, da para cada requisito una prueba concreta que se podrá hacer cuando el sistema esté montado. Así cada requisito es medible y verificable.

**Tabla 10.** Tabla de requisitos

| Código | Requisito | Necesidad que cubre | Prioridad | Cómo se comprueba |
|---|---|---|---|---|
| RF-01 | El sistema deberá permitir la autenticación centralizada de los usuarios, con una cuenta personal para cada trabajador. | N-14 · Autenticación centralizada y control de accesos | Alta | Un trabajador entra con su cuenta personal en todos los servicios internos (archivos, aplicación y canal interno). En el listado de usuarios no hay cuentas compartidas. |
| RF-02 | El sistema deberá permitir asignar permisos por departamento y por puesto, y retirar todos los accesos de una persona cuando deja la empresa, en menos de 15 minutos desde que se desactiva su cuenta. | N-13 · Documentación con acceso restringido; N-14 · Autenticación centralizada y control de accesos | Alta | Se desactiva una cuenta de prueba y pierde el acceso a todos los servicios en menos de 15 minutos. Un usuario sin permiso no puede abrir las carpetas de otro departamento. |
| RF-03 | El sistema deberá permitir compartir documentación en carpetas por departamento y entre los departamentos que trabajan juntos, con acceso solo para quien la necesita, incluida una carpeta restringida para la asesoría y el auditor. | N-13 · Documentación con acceso restringido | Alta | Un usuario de D2 abre su carpeta y una compartida con otro departamento. Un usuario de D7 no puede abrir la de D2. La asesoría y el auditor solo ven su carpeta. |
| RF-04 | El sistema deberá permitir gestionar un único catálogo multimarca (fichas, precios y stock) del que salgan los datos de todos los marketplaces, sin duplicar ficheros. | N-10 · Catálogos multimarca y multicanal | Alta | Se cambia el precio de un producto en el catálogo y es el mismo dato que sale hacia todos los canales. No existen dos fichas para el mismo producto. |
| RF-05 | El sistema deberá disponer de una aplicación web interna para consultar y actualizar el stock y el estado de los pedidos desde las oficinas y desde el almacén. Un cambio hecho en un puesto deberá verse en los demás en menos de 1 minuto. | N-11 · Stock y pedidos en el almacén; N-12 · Estado de pedidos e incidencias | Alta | El mismo pedido se consulta desde un puesto de oficina y desde un lector del almacén con el mismo estado. Un cambio hecho en uno se ve en el otro en menos de 1 minuto. |
| RF-06 | El sistema deberá permitir registrar las incidencias y devoluciones de los pedidos y seguir su estado hasta cerrarlas. | N-12 · Estado de pedidos e incidencias | Alta | Se registra una incidencia de prueba, se cambia su estado y se cierra. Queda el historial con fechas. |
| RF-07 | El sistema deberá almacenar en una base de datos centralizada el catálogo, el stock, los pedidos y las ventas de todos los canales. | N-05 · Datos de ventas centralizados y fiables; N-10 · Catálogos multimarca y multicanal; N-11 · Stock y pedidos en el almacén | Alta | Un pedido de prueba de cualquier marketplace aparece en la base de datos central junto con su producto, su stock y su venta. |
| RF-08 | El sistema deberá generar informes y cuadros de mando de ventas y tesorería para Dirección y Administración y finanzas, a partir de los datos bancarios y contables, que se incorporarán de forma automática al menos una vez al día. | N-01 · Información para decidir y acceso remoto; N-02 · Cuadros de mando de tesorería; N-05 · Datos de ventas centralizados y fiables | Alta | Dirección y D2 abren un cuadro de mando con las ventas y la tesorería del día anterior sin haber introducido datos a mano. |
| RF-09 | El sistema deberá calcular previsiones de aprovisionamiento a partir de las ventas y del stock. | N-06 · Previsión de aprovisionamiento | Alta | Con un histórico de ventas de prueba, el sistema propone una cantidad a pedir para cada producto. |
| RF-10 | El sistema deberá permitir seguir la mercancía en tránsito y guardar la documentación de los envíos al extranjero. | N-07 · Documentación de envíos al extranjero; N-08 · Seguimiento de la mercancía en tránsito | Alta | Un envío al extranjero de prueba muestra su estado en tránsito y tiene sus documentos adjuntos consultables. |
| RF-11 | El sistema deberá permitir registrar las marcas cliente y el seguimiento comercial de cada una, también desde fuera de la oficina. | N-04 · Seguimiento comercial en movilidad | Alta | Un comercial registra el seguimiento de una marca desde un móvil fuera de la red de la empresa, y se ve desde la oficina. |
| RF-12 | El sistema deberá permitir el acceso remoto a los servicios internos solo a los usuarios autorizados, con su cuenta personal y con la conexión cifrada. | N-01 · Información para decidir y acceso remoto; N-04 · Seguimiento comercial en movilidad | Alta | Desde fuera de la empresa, un usuario autorizado entra con su cuenta y uno no autorizado no puede. Se comprueba que la conexión va cifrada. |
| RF-13 | El sistema deberá permitir registrar la jornada de cada trabajador y consultar ese registro desde un portal del empleado. | N-03 · Portal del empleado y control de horarios | Media | Un trabajador ficha la entrada y la salida y consulta su registro en el portal. D2 puede sacar el informe de un mes. |
| RF-14 | El sistema deberá permitir supervisar el estado de servidores y dispositivos de red y avisar automáticamente a Sistemas (D9) en menos de 5 minutos cuando algo falle. | N-09 · Detectar fallos de red y servidores | Alta | Se para un servicio de prueba y D9 recibe el aviso en menos de 5 minutos. |
| RF-15 | El sistema deberá hacer copias de seguridad automáticas de los datos al menos una vez al día, conservar las de los últimos 7 días, permitir restaurarlos y comprobar cada mes que la restauración funciona. | N-16 · Copias de seguridad y cortes eléctricos | Alta | Hay una copia de cada uno de los últimos 7 días. Se restaura un archivo borrado a propósito. Queda anotada la fecha de la última prueba de restauración, que se hace cada mes. |
| RF-16 | El sistema deberá ofrecer acceso a Internet a los visitantes sin darles acceso a ningún recurso interno. | N-15 · Separación del tráfico de red | Media | Desde la red de invitados se navega por Internet, pero no se llega a ningún servidor ni equipo interno. |
| RF-17 | El sistema deberá permitir la comunicación interna entre todos los departamentos, y en especial entre las oficinas y el almacén, mediante un canal de comunicación interno accesible con la cuenta de cada trabajador. | N-11 · Stock y pedidos en el almacén; N-12 · Estado de pedidos e incidencias | Alta | Un usuario de oficina envía un mensaje a uno del almacén con su cuenta personal y le llega. |
| RNF-01 | La red deberá estar segmentada para separar oficinas, almacén, servidores e invitados, de forma que un fallo o una infección en una zona no se extienda al resto. | N-15 · Separación del tráfico de red | Media | Desde cada zona solo se llega a los servicios permitidos. Desde invitados no se llega a ninguno interno. Un fallo provocado en una zona no afecta a las demás. |
| RNF-02 | Toda la zona de trabajo del almacén deberá tener cobertura inalámbrica para los lectores. | N-11 · Stock y pedidos en el almacén | Alta | Se recorren todas las zonas de trabajo del almacén con un lector y no pierde la conexión en ningún punto. |
| RNF-03 | Los equipos críticos deberán seguir funcionando durante un corte eléctrico de al menos 10 minutos y apagarse de forma ordenada si el corte dura más. | N-16 · Copias de seguridad y cortes eléctricos | Alta | En un corte de luz de prueba, los equipos críticos siguen funcionando 10 minutos y después se apagan solos de forma ordenada. |
| RNF-04 | Los servicios críticos deberán disponer de medidas frente a fallos: la avería de un solo equipo o disco no deberá provocar pérdida de datos, y habrá una copia fuera de la sede, actualizada al menos una vez a la semana. | N-16 · Copias de seguridad y cortes eléctricos | Alta | Se retira un disco o se apaga un equipo en una prueba y no se pierden datos. Existe una copia fuera de la sede con fecha de la última semana. |
| RNF-05 | Los servicios de stock y pedidos deberán estar disponibles al menos el 99 % del horario del almacén, medido cada mes, y ninguna caída deberá durar más de 1 hora. | N-09 · Detectar fallos de red y servidores; N-11 · Stock y pedidos en el almacén | Alta | Durante un mes, la monitorización registra una disponibilidad de al menos el 99 % del horario del almacén. Ninguna caída dura más de 1 hora. |
| RNF-06 | La información económica, la de las marcas y los datos personales solo deberán ser accesibles a los perfiles autorizados, cumpliendo el RGPD. Las cuentas con acceso a esa información usarán un segundo paso de verificación y quedará registro de los accesos. | N-13 · Documentación con acceso restringido; N-14 · Autenticación centralizada y control de accesos | Alta | Con un usuario de cada perfil, solo los autorizados abren contabilidad, nóminas y datos de marcas, y al entrar se les pide el segundo paso de verificación. Queda registro de los accesos. |
| RNF-07 | La aplicación interna deberá poder usarse desde los puestos de oficina, los lectores del almacén y los dispositivos móviles del equipo comercial. | N-04 · Seguimiento comercial en movilidad; N-11 · Stock y pedidos en el almacén; N-12 · Estado de pedidos e incidencias | Alta | La misma operación (consultar un pedido) se hace desde un PC, un lector y un móvil. |
| RNF-08 | El sistema deberá facilitar la monitorización y el mantenimiento desde un punto central: Sistemas (D9) deberá poder ver el estado de servidores, red y servicios y administrarlos sin desplazarse a cada equipo. | N-09 · Detectar fallos de red y servidores | Alta | D9 ve en una sola pantalla el estado de todos los servidores, la red y los servicios, y puede administrarlos sin ir a cada equipo. |
| RNF-09 | La infraestructura deberá estar correctamente documentada (equipos, red, servicios, usuarios y procedimientos de copia y restauración), y la documentación se actualizará con cada cambio para que cualquier miembro de D9 pueda mantenerla. | N-09 · Detectar fallos de red y servidores | Alta | Una persona de D9 que no montó el sistema restaura una copia siguiendo solo la documentación. Cada cambio en la infraestructura tiene su fecha en la documentación. |
| RNF-10 | El registro de jornada deberá cumplir la normativa laboral de fichaje: guardar la hora de inicio y de fin de cada jornada de cada trabajador, conservar los registros 4 años y tenerlos a disposición de los trabajadores, de sus representantes y de la Inspección de Trabajo (art. 34.9 del Estatuto de los Trabajadores, F8). | N-03 · Portal del empleado y control de horarios | Media | El registro guarda la hora de inicio y de fin de cada jornada de cada trabajador. Se pueden consultar registros de hasta 4 años atrás, y el trabajador puede ver los suyos. |
| RNF-11 | El sistema deberá permitir futuras ampliaciones (más trabajadores y terminales en campaña, más marcas, canales y datos, o una segunda nave) sin tener que rehacer la red ni los servidores: se deberán poder añadir puestos, dispositivos y servicios sin modificar los que ya funcionan. | N-10 · Catálogos multimarca y multicanal; N-11 · Stock y pedidos en el almacén | Alta | Se añaden un usuario, un puesto y un dispositivo nuevos sin cambiar la configuración de los que ya funcionan. |

Las cifras de los requisitos son **valores fijados por el grupo**, porque las fuentes no dan datos de Grutinet sobre esto: 15 minutos (RF-02), 1 minuto (RF-05), carga diaria de datos (RF-08), 5 minutos (RF-14), copia diaria, 7 días de copias y prueba mensual (RF-15), 10 minutos (RNF-03), copia semanal fuera de la sede (RNF-04) y 99 % de disponibilidad con caídas de 1 hora como máximo (RNF-05). Los 4 años de RNF-10 no los fija el grupo: los marca la ley (F8).

### Control de calidad de los requisitos

Cada requisito se ha revisado con cinco criterios:

1. **Claro y concreto:** dice exactamente qué se pide, sin expresiones como «debe funcionar bien».
2. **Se puede comprobar:** tiene una cifra o una condición concreta y una prueba en la columna «Cómo se comprueba» de la tabla 10.
3. **Cubre una necesidad de B3:** cita al menos una necesidad N-01 a N-16.
4. **No adelanta una decisión técnica:** no impone marcas, productos, modelos, direccionamiento ni configuraciones.
5. **Prioridad coherente:** tiene la prioridad de su necesidad (la más alta, si cubre varias).

**Tabla 11.** Control de calidad de los requisitos

| Código | Claro y concreto | Se puede comprobar | Cubre una necesidad de B3 | No adelanta una decisión técnica | Prioridad coherente | Nota |
|---|---|---|---|---|---|---|
| RF-01 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-02 | ✓ | ✓ | ✓ | ✓ | ✓ | Concretado: plazo de 15 minutos para retirar los accesos. |
| RF-03 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-04 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-05 | ✓ | ✓ | ✓ | ✓ | ✓ | «Aplicación web interna» es un ejemplo del enunciado; no fija producto ni lenguaje. Concretado: los cambios se ven en menos de 1 minuto. |
| RF-06 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-07 | ✓ | ✓ | ✓ | ✓ | ✓ | «Base de datos» es un ejemplo del enunciado; no fija el gestor. |
| RF-08 | ✓ | ✓ | ✓ | ✓ | ✓ | Concretado: los datos se cargan al menos una vez al día. |
| RF-09 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-10 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-11 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-12 | ✓ | ✓ | ✓ | ✓ | ✓ | Corregido: «acceso remoto seguro» no se podía comprobar; ahora pide cuenta personal y conexión cifrada. |
| RF-13 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-14 | ✓ | ✓ | ✓ | ✓ | ✓ | Concretado: aviso en menos de 5 minutos. |
| RF-15 | ✓ | ✓ | ✓ | ✓ | ✓ | Corregido: se añade la frecuencia (al menos diaria), los 7 días de copias y la prueba mensual de restauración. |
| RF-16 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-17 | ✓ | ✓ | ✓ | ✓ | ✓ | Fusiona la necesidad general 3 de B3 con N-11 y N-12. |
| RNF-01 | ✓ | ✓ | ✓ | ✓ | ✓ | «Red segmentada» es un ejemplo del enunciado; no fija cómo se segmenta. |
| RNF-02 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RNF-03 | ✓ | ✓ | ✓ | ✓ | ✓ | Corregido: «corte breve» no se podía comprobar; ahora fija 10 minutos (valor decidido por el grupo). |
| RNF-04 | ✓ | ✓ | ✓ | ✓ | ✓ | Concretado: la copia de fuera de la sede se actualiza cada semana. |
| RNF-05 | ✓ | ✓ | ✓ | ✓ | ✓ | Concretado: 99 % de disponibilidad y caídas de 1 hora como máximo. |
| RNF-06 | ✓ | ✓ | ✓ | ✓ | ✓ | Añadido: segundo paso de verificación y registro de accesos, que B4 (MI-5) ya proponía. |
| RNF-07 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RNF-08 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RNF-09 | ✓ | ✓ | ✓ | ✓ | ✓ | Corregido: la prioridad pasa de Media a Alta, la de su necesidad N-09. |
| RNF-10 | ✓ | ✓ | ✓ | ✓ | ✓ | Concretado: lo que exige el art. 34.9 del Estatuto de los Trabajadores (F8). |
| RNF-11 | ✓ | ✓ | ✓ | ✓ | ✓ | Corregido: se quita «se dimensionará con margen», que no se podía comprobar y adelantaba el diseño. |

En la revisión se corrigieron cuatro requisitos que no se podían comprobar (RF-12, RF-15, RNF-03 y RNF-11) y la prioridad de RNF-09. Después se añadieron cifras a RF-02, RF-05, RF-08, RF-14, RF-15, RNF-04, RNF-05 y RNF-10, y el segundo paso de verificación a RNF-06. Las correcciones también están aplicadas en las tablas 8 y 9. Tras ellas, los 28 requisitos cumplen los cinco criterios y tienen su prueba en la tabla 10.
