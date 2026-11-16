# 7.6. Catálogo inicial de requisitos (B6)

Cada requisito sale de una o varias necesidades de B3 y tiene su misma prioridad (la más alta, si cubre varias). Ninguno impone una marca o tecnología concreta.

## 6.1. Requisitos funcionales

Indican qué deberá hacer el sistema.

**Tabla 11.** Requisitos funcionales

| Código | Requisito | Necesidad que cubre | Prioridad |
|---|---|---|---|
| RF-01 | El sistema deberá permitir la autenticación centralizada de los usuarios, con una cuenta personal para cada trabajador. | N-14 · Autenticación centralizada y control de accesos | Alta |
| RF-02 | El sistema deberá permitir asignar permisos por departamento y por puesto, y retirar todos los accesos de una persona cuando deja la empresa. | N-14 · Control de accesos; N-13 · Documentación con acceso restringido | Alta |
| RF-03 | El sistema deberá permitir compartir documentación en carpetas por departamento y entre los departamentos que trabajan juntos, con acceso solo para quien la necesita, incluida una carpeta restringida para la asesoría y el auditor. | N-13 · Documentación compartida con acceso restringido | Alta |
| RF-04 | El sistema deberá permitir gestionar un único catálogo multimarca (fichas, precios y stock) del que salgan los datos de todos los marketplaces, sin duplicar ficheros. | N-10 · Catálogos multimarca y multicanal | Alta |
| RF-05 | El sistema deberá disponer de una aplicación web interna para consultar y actualizar el stock y el estado de los pedidos desde las oficinas y desde el almacén. | N-11 · Consulta de stock y pedidos en el almacén; N-12 · Estado de los pedidos | Alta |
| RF-06 | El sistema deberá permitir registrar las incidencias y devoluciones de los pedidos y seguir su estado hasta cerrarlas. | N-12 · Gestión de incidencias | Alta |
| RF-07 | El sistema deberá almacenar en una base de datos centralizada el catálogo, el stock, los pedidos y las ventas de todos los canales. | N-05 · Datos de ventas centralizados; N-10; N-11 | Alta |
| RF-08 | El sistema deberá generar informes y cuadros de mando de ventas y tesorería para Dirección y Administración y finanzas, a partir de los datos bancarios y contables, que se incorporarán de forma automática. | N-01 · Información para decidir; N-02 · Cuadros de mando; N-05 | Alta |
| RF-09 | El sistema deberá calcular previsiones de aprovisionamiento a partir de las ventas y del stock. | N-06 · Previsión de aprovisionamiento | Alta |
| RF-10 | El sistema deberá permitir seguir la mercancía en tránsito y guardar la documentación de los envíos al extranjero. | N-08 · Mercancía en tránsito; N-07 · Documentación aduanera | Alta |
| RF-11 | El sistema deberá permitir registrar las marcas cliente y el seguimiento comercial de cada una, también desde fuera de la oficina. | N-04 · Seguimiento comercial en movilidad | Alta |
| RF-12 | El sistema deberá permitir el acceso remoto a los servicios internos solo a los usuarios autorizados, con su cuenta personal y con la conexión cifrada. | N-01 · Acceso remoto; N-04 | Alta |
| RF-13 | El sistema deberá permitir registrar la jornada de cada trabajador y consultar ese registro desde un portal del empleado. | N-03 · Portal del empleado y control de horarios | Media |
| RF-14 | El sistema deberá permitir supervisar el estado de servidores y dispositivos de red y avisar automáticamente cuando algo falle. | N-09 · Monitorización de red y servidores | Alta |
| RF-15 | El sistema deberá hacer copias de seguridad automáticas de los datos al menos una vez al día, permitir restaurarlos y comprobar periódicamente que la restauración funciona. | N-16 · Copias de seguridad | Alta |
| RF-16 | El sistema deberá ofrecer acceso a Internet a los visitantes sin darles acceso a ningún recurso interno. | N-15 · Separación del tráfico de invitados | Media |
| RF-17 | El sistema deberá permitir la comunicación interna entre todos los departamentos, y en especial entre las oficinas y el almacén, mediante un canal de comunicación interno accesible con la cuenta de cada trabajador. | N-11 · Stock y pedidos en el almacén; N-12 · Estado de pedidos e incidencias (B3, necesidad general 3; B4, oportunidad 3) | Alta |

## 6.2. Requisitos no funcionales

Indican cómo debe comportarse el sistema o qué características generales debe tener.

**Tabla 12.** Requisitos no funcionales

| Código | Requisito | Necesidad que cubre | Prioridad |
|---|---|---|---|
| RNF-01 | La red deberá estar segmentada para separar oficinas, almacén, servidores e invitados, de forma que un fallo o una infección en una zona no se extienda al resto. | N-15 · Separación lógica del tráfico | Media |
| RNF-02 | Toda la zona de trabajo del almacén deberá tener cobertura inalámbrica para los lectores. | N-11 · Cobertura en el almacén | Alta |
| RNF-03 | Los equipos críticos deberán seguir funcionando durante un corte eléctrico de al menos 10 minutos y apagarse de forma ordenada si el corte dura más. | N-16 · Protección frente a cortes eléctricos | Alta |
| RNF-04 | Los servicios críticos deberán disponer de medidas frente a fallos: la avería de un solo equipo o disco no deberá provocar pérdida de datos, y habrá una copia fuera de la sede. | N-16 · Pérdida de datos | Alta |
| RNF-05 | Los servicios de stock y pedidos deberán estar disponibles durante todo el horario del almacén. | N-09 · Caídas que paralizan la logística; N-11 | Alta |
| RNF-06 | La información económica, la de las marcas y los datos personales solo deberán ser accesibles a los perfiles autorizados, cumpliendo el RGPD. | N-13 · Fugas de información; N-14 | Alta |
| RNF-07 | La aplicación interna deberá poder usarse desde los puestos de oficina, los lectores del almacén y los dispositivos móviles del equipo comercial. | N-04; N-11; N-12 | Alta |
| RNF-08 | El sistema deberá facilitar la monitorización y el mantenimiento desde un punto central: Sistemas (D9) deberá poder ver el estado de servidores, red y servicios y administrarlos sin desplazarse a cada equipo. | N-09 · Detectar fallos a tiempo | Alta |
| RNF-09 | La infraestructura deberá estar correctamente documentada (equipos, red, servicios, usuarios y procedimientos de copia y restauración), y la documentación se actualizará con cada cambio para que cualquier miembro de D9 pueda mantenerla. | N-09 · Mantenimiento del sistema | Alta |
| RNF-10 | El registro de jornada deberá cumplir la normativa laboral de fichaje. | N-03 · Sanciones por incumplir el fichaje | Media |
| RNF-11 | El sistema deberá permitir futuras ampliaciones (más trabajadores y terminales en campaña, más marcas, canales y datos, o una segunda nave) sin tener que rehacer la red ni los servidores: se deberán poder añadir puestos, dispositivos y servicios sin modificar los que ya funcionan. | N-10 · Más marcas y canales; N-11 · Más pedidos en el almacén (B4, pregunta 6 y oportunidad 7) | Alta |

## 6.3. Tabla de requisitos

Todos los requisitos del catálogo en una sola tabla. Los funcionales llevan el código **RF** y los no funcionales, **RNF**. La necesidad se indica siempre con su código y su nombre de B3, y la prioridad es la de esa necesidad (la más alta, si cubre varias).

**Tabla 13.** Tabla de requisitos

| Código | Requisito | Necesidad que cubre | Prioridad |
|---|---|---|---|
| RF-01 | El sistema deberá permitir la autenticación centralizada de los usuarios, con una cuenta personal para cada trabajador. | N-14 · Autenticación centralizada y control de accesos | Alta |
| RF-02 | El sistema deberá permitir asignar permisos por departamento y por puesto, y retirar todos los accesos de una persona cuando deja la empresa. | N-13 · Documentación con acceso restringido; N-14 · Autenticación centralizada y control de accesos | Alta |
| RF-03 | El sistema deberá permitir compartir documentación en carpetas por departamento y entre los departamentos que trabajan juntos, con acceso solo para quien la necesita, incluida una carpeta restringida para la asesoría y el auditor. | N-13 · Documentación con acceso restringido | Alta |
| RF-04 | El sistema deberá permitir gestionar un único catálogo multimarca (fichas, precios y stock) del que salgan los datos de todos los marketplaces, sin duplicar ficheros. | N-10 · Catálogos multimarca y multicanal | Alta |
| RF-05 | El sistema deberá disponer de una aplicación web interna para consultar y actualizar el stock y el estado de los pedidos desde las oficinas y desde el almacén. | N-11 · Stock y pedidos en el almacén; N-12 · Estado de pedidos e incidencias | Alta |
| RF-06 | El sistema deberá permitir registrar las incidencias y devoluciones de los pedidos y seguir su estado hasta cerrarlas. | N-12 · Estado de pedidos e incidencias | Alta |
| RF-07 | El sistema deberá almacenar en una base de datos centralizada el catálogo, el stock, los pedidos y las ventas de todos los canales. | N-05 · Datos de ventas centralizados y fiables; N-10 · Catálogos multimarca y multicanal; N-11 · Stock y pedidos en el almacén | Alta |
| RF-08 | El sistema deberá generar informes y cuadros de mando de ventas y tesorería para Dirección y Administración y finanzas, a partir de los datos bancarios y contables, que se incorporarán de forma automática. | N-01 · Información para decidir y acceso remoto; N-02 · Cuadros de mando de tesorería; N-05 · Datos de ventas centralizados y fiables | Alta |
| RF-09 | El sistema deberá calcular previsiones de aprovisionamiento a partir de las ventas y del stock. | N-06 · Previsión de aprovisionamiento | Alta |
| RF-10 | El sistema deberá permitir seguir la mercancía en tránsito y guardar la documentación de los envíos al extranjero. | N-07 · Documentación de envíos al extranjero; N-08 · Seguimiento de la mercancía en tránsito | Alta |
| RF-11 | El sistema deberá permitir registrar las marcas cliente y el seguimiento comercial de cada una, también desde fuera de la oficina. | N-04 · Seguimiento comercial en movilidad | Alta |
| RF-12 | El sistema deberá permitir el acceso remoto a los servicios internos solo a los usuarios autorizados, con su cuenta personal y con la conexión cifrada. | N-01 · Información para decidir y acceso remoto; N-04 · Seguimiento comercial en movilidad | Alta |
| RF-13 | El sistema deberá permitir registrar la jornada de cada trabajador y consultar ese registro desde un portal del empleado. | N-03 · Portal del empleado y control de horarios | Media |
| RF-14 | El sistema deberá permitir supervisar el estado de servidores y dispositivos de red y avisar automáticamente cuando algo falle. | N-09 · Detectar fallos de red y servidores | Alta |
| RF-15 | El sistema deberá hacer copias de seguridad automáticas de los datos al menos una vez al día, permitir restaurarlos y comprobar periódicamente que la restauración funciona. | N-16 · Copias de seguridad y cortes eléctricos | Alta |
| RF-16 | El sistema deberá ofrecer acceso a Internet a los visitantes sin darles acceso a ningún recurso interno. | N-15 · Separación del tráfico de red | Media |
| RF-17 | El sistema deberá permitir la comunicación interna entre todos los departamentos, y en especial entre las oficinas y el almacén, mediante un canal de comunicación interno accesible con la cuenta de cada trabajador. | N-11 · Stock y pedidos en el almacén; N-12 · Estado de pedidos e incidencias | Alta |
| RNF-01 | La red deberá estar segmentada para separar oficinas, almacén, servidores e invitados, de forma que un fallo o una infección en una zona no se extienda al resto. | N-15 · Separación del tráfico de red | Media |
| RNF-02 | Toda la zona de trabajo del almacén deberá tener cobertura inalámbrica para los lectores. | N-11 · Stock y pedidos en el almacén | Alta |
| RNF-03 | Los equipos críticos deberán seguir funcionando durante un corte eléctrico de al menos 10 minutos y apagarse de forma ordenada si el corte dura más. | N-16 · Copias de seguridad y cortes eléctricos | Alta |
| RNF-04 | Los servicios críticos deberán disponer de medidas frente a fallos: la avería de un solo equipo o disco no deberá provocar pérdida de datos, y habrá una copia fuera de la sede. | N-16 · Copias de seguridad y cortes eléctricos | Alta |
| RNF-05 | Los servicios de stock y pedidos deberán estar disponibles durante todo el horario del almacén. | N-09 · Detectar fallos de red y servidores; N-11 · Stock y pedidos en el almacén | Alta |
| RNF-06 | La información económica, la de las marcas y los datos personales solo deberán ser accesibles a los perfiles autorizados, cumpliendo el RGPD. | N-13 · Documentación con acceso restringido; N-14 · Autenticación centralizada y control de accesos | Alta |
| RNF-07 | La aplicación interna deberá poder usarse desde los puestos de oficina, los lectores del almacén y los dispositivos móviles del equipo comercial. | N-04 · Seguimiento comercial en movilidad; N-11 · Stock y pedidos en el almacén; N-12 · Estado de pedidos e incidencias | Alta |
| RNF-08 | El sistema deberá facilitar la monitorización y el mantenimiento desde un punto central: Sistemas (D9) deberá poder ver el estado de servidores, red y servicios y administrarlos sin desplazarse a cada equipo. | N-09 · Detectar fallos de red y servidores | Alta |
| RNF-09 | La infraestructura deberá estar correctamente documentada (equipos, red, servicios, usuarios y procedimientos de copia y restauración), y la documentación se actualizará con cada cambio para que cualquier miembro de D9 pueda mantenerla. | N-09 · Detectar fallos de red y servidores | Alta |
| RNF-10 | El registro de jornada deberá cumplir la normativa laboral de fichaje. | N-03 · Portal del empleado y control de horarios | Media |
| RNF-11 | El sistema deberá permitir futuras ampliaciones (más trabajadores y terminales en campaña, más marcas, canales y datos, o una segunda nave) sin tener que rehacer la red ni los servidores: se deberán poder añadir puestos, dispositivos y servicios sin modificar los que ya funcionan. | N-10 · Catálogos multimarca y multicanal; N-11 · Stock y pedidos en el almacén | Alta |

Los 10 minutos de RNF-03 y la copia diaria de RF-15 son valores fijados por el grupo, porque las fuentes no dan datos de Grutinet sobre esto.

### Control de calidad de los requisitos

Cada requisito se ha revisado con cinco criterios:

1. **Claro y concreto:** dice exactamente qué se pide, sin expresiones como «debe funcionar bien».
2. **Se puede comprobar:** se puede verificar con una prueba o una observación cuando el sistema esté montado.
3. **Cubre una necesidad de B3:** cita al menos una necesidad N-01 a N-16.
4. **No adelanta una decisión técnica:** no impone marcas, productos, modelos, direccionamiento ni configuraciones.
5. **Prioridad coherente:** tiene la prioridad de su necesidad (la más alta, si cubre varias).

**Tabla 14.** Control de calidad de los requisitos

| Código | Claro y concreto | Se puede comprobar | Cubre una necesidad de B3 | No adelanta una decisión técnica | Prioridad coherente | Nota |
|---|---|---|---|---|---|---|
| RF-01 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-02 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-03 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-04 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-05 | ✓ | ✓ | ✓ | ✓ | ✓ | «Aplicación web interna» es un ejemplo del enunciado; no fija producto ni lenguaje. |
| RF-06 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-07 | ✓ | ✓ | ✓ | ✓ | ✓ | «Base de datos» es un ejemplo del enunciado; no fija el gestor. |
| RF-08 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-09 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-10 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-11 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-12 | ✓ | ✓ | ✓ | ✓ | ✓ | Corregido: «acceso remoto seguro» no se podía comprobar; ahora pide cuenta personal y conexión cifrada. |
| RF-13 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-14 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-15 | ✓ | ✓ | ✓ | ✓ | ✓ | Corregido: se añade la frecuencia (al menos diaria) y la prueba periódica de restauración. |
| RF-16 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RF-17 | ✓ | ✓ | ✓ | ✓ | ✓ | Fusiona la necesidad general 3 de B3 con N-11 y N-12. |
| RNF-01 | ✓ | ✓ | ✓ | ✓ | ✓ | «Red segmentada» es un ejemplo del enunciado; no fija cómo se segmenta. |
| RNF-02 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RNF-03 | ✓ | ✓ | ✓ | ✓ | ✓ | Corregido: «corte breve» no se podía comprobar; ahora fija 10 minutos (valor decidido por el grupo). |
| RNF-04 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RNF-05 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RNF-06 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RNF-07 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RNF-08 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RNF-09 | ✓ | ✓ | ✓ | ✓ | ✓ | Corregido: la prioridad pasa de Media a Alta, la de su necesidad N-09. |
| RNF-10 | ✓ | ✓ | ✓ | ✓ | ✓ | — |
| RNF-11 | ✓ | ✓ | ✓ | ✓ | ✓ | Corregido: se quita «se dimensionará con margen», que no se podía comprobar y adelantaba el diseño. |

En la revisión se corrigieron cuatro requisitos que no se podían comprobar (RF-12, RF-15, RNF-03 y RNF-11) y la prioridad de RNF-09. Las correcciones también están aplicadas en las tablas 11 y 12. Tras ellas, los 28 requisitos cumplen los cinco criterios.
