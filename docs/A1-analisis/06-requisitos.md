# 7.6. Catálogo inicial de requisitos (B6)

Cada requisito sale de una o varias necesidades de B3 y tiene su misma prioridad (la más alta, si cubre varias). Ninguno impone una marca o tecnología concreta.

## 6.1. Requisitos funcionales

Indican qué deberá hacer el sistema.

**Tabla 11.** Requisitos funcionales

| Código | Requisito | Necesidad que cubre | Prioridad |
|---|---|---|---|
| RF-01 | El sistema deberá permitir la autenticación centralizada de los usuarios, con una cuenta personal para cada trabajador. | N-14 · Autenticación centralizada y control de accesos | Alta |
| RF-02 | El sistema deberá permitir asignar permisos por departamento y por puesto, y retirar todos los accesos de una persona cuando deja la empresa. | N-14 · Control de accesos; N-13 · Documentación con acceso restringido | Alta |
| RF-03 | El sistema deberá permitir compartir documentación en carpetas por departamento, con acceso solo para quien la necesita. | N-13 · Documentación compartida con acceso restringido | Alta |
| RF-04 | El sistema deberá permitir gestionar un único catálogo multimarca (fichas, precios y stock) del que salgan los datos de todos los marketplaces, sin duplicar ficheros. | N-10 · Catálogos multimarca y multicanal | Alta |
| RF-05 | El sistema deberá disponer de una aplicación web interna para consultar y actualizar el stock y el estado de los pedidos desde las oficinas y desde el almacén. | N-11 · Consulta de stock y pedidos en el almacén; N-12 · Estado de los pedidos | Alta |
| RF-06 | La aplicación deberá permitir registrar las incidencias y devoluciones de los pedidos y seguir su estado hasta cerrarlas. | N-12 · Gestión de incidencias | Alta |
| RF-07 | El sistema deberá almacenar en una base de datos centralizada el catálogo, el stock, los pedidos y las ventas de todos los canales. | N-05 · Datos de ventas centralizados; N-10; N-11 | Alta |
| RF-08 | El sistema deberá generar informes y cuadros de mando de ventas y tesorería para Dirección y Administración y finanzas. | N-01 · Información para decidir; N-02 · Cuadros de mando; N-05 | Alta |
| RF-09 | El sistema deberá calcular previsiones de aprovisionamiento a partir de las ventas y del stock. | N-06 · Previsión de aprovisionamiento | Alta |
| RF-10 | El sistema deberá permitir seguir la mercancía en tránsito y guardar la documentación de los envíos al extranjero. | N-08 · Mercancía en tránsito; N-07 · Documentación aduanera | Alta |
| RF-11 | El sistema deberá permitir registrar las marcas cliente y el seguimiento comercial de cada una, también desde fuera de la oficina. | N-04 · Seguimiento comercial en movilidad | Alta |
| RF-12 | El sistema deberá permitir el acceso remoto seguro a los servicios internos solo a los usuarios autorizados. | N-01 · Acceso remoto; N-04 | Alta |
| RF-13 | El sistema deberá permitir registrar la jornada de cada trabajador y consultar ese registro desde un portal del empleado. | N-03 · Portal del empleado y control de horarios | Media |
| RF-14 | El sistema deberá permitir supervisar el estado de servidores y dispositivos de red y avisar automáticamente cuando algo falle. | N-09 · Monitorización de red y servidores | Alta |
| RF-15 | El sistema deberá hacer copias de seguridad automáticas de los datos y permitir restaurarlos. | N-16 · Copias de seguridad | Alta |
| RF-16 | El sistema deberá ofrecer acceso a Internet a los visitantes sin darles acceso a ningún recurso interno. | N-15 · Separación del tráfico de invitados | Media |

## 6.2. Requisitos no funcionales

Indican cómo debe comportarse el sistema o qué características generales debe tener.

**Tabla 12.** Requisitos no funcionales

| Código | Requisito | Necesidad que cubre | Prioridad |
|---|---|---|---|
| RNF-01 | La red deberá estar segmentada para separar oficinas, almacén, servidores e invitados. | N-15 · Separación lógica del tráfico | Media |
| RNF-02 | Toda la zona de trabajo del almacén deberá tener cobertura inalámbrica para los lectores. | N-11 · Cobertura en el almacén | Alta |
| RNF-03 | Los equipos críticos deberán seguir funcionando ante un corte eléctrico breve y apagarse de forma ordenada si el corte se alarga. | N-16 · Protección frente a cortes eléctricos | Alta |
| RNF-04 | Los servicios críticos deberán disponer de medidas frente a fallos: la avería de un solo equipo o disco no deberá provocar pérdida de datos, y habrá una copia fuera de la sede. | N-16 · Pérdida de datos | Alta |
| RNF-05 | Los servicios de stock y pedidos deberán estar disponibles durante todo el horario del almacén. | N-09 · Caídas que paralizan la logística; N-11 | Alta |
| RNF-06 | La información económica, la de las marcas y los datos personales solo deberán ser accesibles a los perfiles autorizados, cumpliendo el RGPD. | N-13 · Fugas de información; N-14 | Alta |
| RNF-07 | La aplicación interna deberá poder usarse desde los puestos de oficina, los lectores del almacén y los dispositivos móviles del equipo comercial. | N-04; N-11; N-12 | Alta |
| RNF-08 | El sistema deberá facilitar la monitorización y el mantenimiento desde un punto central. | N-09 · Detectar fallos a tiempo | Alta |
| RNF-09 | La infraestructura deberá estar correctamente documentada. | N-09 · Mantenimiento del sistema | Media |
| RNF-10 | El registro de jornada deberá cumplir la normativa laboral de fichaje. | N-03 · Sanciones por incumplir el fichaje | Media |
