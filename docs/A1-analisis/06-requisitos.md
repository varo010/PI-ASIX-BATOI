# 7.6. Catálogo inicial de requisitos (B6)

Los requisitos se han redactado para que sean **claros, comprobables y trazables**: cada uno indica la necesidad que cubre y tiene la misma prioridad que ella (o la más alta, si cubre varias). Ninguno impone una marca o tecnología concreta.

## Requisitos funcionales (qué deberá hacer el sistema)

**Tabla 11.** Requisitos funcionales

| Código | Requisito | Necesidad | Prioridad |
|---|---|---|---|
| RF-01 | El sistema deberá permitir que cada trabajador se identifique con una cuenta personal única, gestionada de forma centralizada, para acceder a los equipos y servicios. | N-10 | Alta |
| RF-02 | El sistema deberá permitir asignar permisos por departamento y por puesto, y retirar todos los accesos de una persona en el momento en que deja la empresa. | N-10, N-06 | Alta |
| RF-03 | El sistema deberá permitir almacenar y compartir documentación en carpetas por departamento y por marca cliente, con permisos de lectura y escritura diferenciados. | N-01, N-06, N-08 | Alta |
| RF-04 | El sistema deberá guardar el historial de versiones de los ficheros de catálogo (fichas, imágenes, tarifas) y permitir recuperar una versión anterior. | N-01 | Alta |
| RF-05 | El sistema deberá ofrecer una aplicación web interna para consultar el estado de cada pedido (recibido, preparado, enviado, entregado, devuelto). | N-02, N-04 | Alta |
| RF-06 | La aplicación deberá permitir consultar y actualizar el stock por referencia y ubicación desde los terminales del almacén. | N-02, N-03 | Alta |
| RF-07 | La aplicación deberá permitir registrar incidencias de pedidos (rotura, extravío, devolución, reclamación), asignarlas a una persona y seguir su estado hasta cerrarlas. | N-04 | Alta |
| RF-08 | El sistema deberá almacenar en una base de datos centralizada los pedidos, el stock, las incidencias y las ventas por marca y canal. | N-02, N-05 | Alta |
| RF-09 | El sistema deberá generar informes de ventas, stock e incidencias por marca, marketplace y periodo, exportables para enviarlos a las marcas. | N-05, N-07, N-08 | Media |
| RF-10 | El sistema deberá permitir el acceso remoto seguro a los servicios internos solo a los usuarios autorizados. | N-07 | Media |
| RF-11 | El sistema deberá supervisar servidores, red y servicios críticos y avisar automáticamente al responsable cuando uno falle o supere un umbral. | N-09 | Alta |
| RF-12 | El sistema deberá hacer copias de seguridad automáticas de los datos y permitir restaurarlos, completos o por ficheros sueltos. | N-12 | Alta |
| RF-13 | El sistema deberá ofrecer acceso a Internet a los visitantes sin darles acceso a ningún recurso interno. | N-11 | Alta |
| RF-14 | El sistema deberá permitir registrar la jornada de cada trabajador (entrada, salida y pausas) y consultar ese registro. | N-14 | Media |
| RF-15 | El sistema deberá permitir enviar avisos internos entre la oficina y el almacén. | N-16 | Baja |

## Requisitos no funcionales (cómo deberá comportarse el sistema)

**Tabla 12.** Requisitos no funcionales

| Código | Requisito | Necesidad | Prioridad |
|---|---|---|---|
| RNF-01 | **Escalabilidad.** El sistema deberá admitir, como mínimo, el doble de usuarios, terminales y marcas actuales, y la incorporación de una segunda nave, sin rediseñar su estructura. | N-15 | Media |
| RNF-02 | **Disponibilidad.** Los servicios de pedidos y stock deberán estar disponibles durante todo el horario del almacén, incluidas las campañas. | N-02, N-13 | Alta |
| RNF-03 | **Tolerancia a fallos.** La avería de un único disco o equipo de un servicio crítico no deberá provocar pérdida de datos. | N-12, N-13 | Alta |
| RNF-04 | **Alimentación.** Los equipos críticos deberán seguir funcionando ante un corte eléctrico breve y apagarse de forma ordenada si el corte se alarga. | N-13 | Alta |
| RNF-05 | **Recuperación.** Deberá poder recuperarse la información de cualquier día de las últimas cuatro semanas, y al menos una copia deberá estar fuera de las instalaciones. | N-12 | Alta |
| RNF-06 | **Segmentación.** La red deberá separar oficinas, almacén, servidores, gestión e invitados, y entre ellos solo se permitirán las comunicaciones imprescindibles. | N-11 | Alta |
| RNF-07 | **Confidencialidad.** La información económica, la de las marcas y los datos personales solo deberán ser accesibles a los perfiles autorizados, los accesos quedarán registrados y se cumplirán el RGPD y la LOPDGDD. | N-06, N-10 | Alta |
| RNF-08 | **Cobertura.** Toda la superficie de trabajo del almacén deberá tener conectividad inalámbrica estable para los terminales. | N-03 | Alta |
| RNF-09 | **Rendimiento.** La consulta de un pedido o del stock de una referencia deberá responder en menos de 3 segundos, con todos los usuarios conectados. | N-02, N-04 | Media |
| RNF-10 | **Usabilidad.** La aplicación interna deberá poder usarse desde los terminales del almacén y desde los puestos de oficina, y un usuario nuevo deberá aprender a usarla en menos de una jornada. | N-02, N-04 | Media |
| RNF-11 | **Mantenibilidad.** La infraestructura deberá estar documentada (inventario, esquemas, cuentas y procedimientos) y la documentación se actualizará con cada cambio. | N-09, N-15 | Media |
| RNF-12 | **Monitorización.** Equipos y servicios deberán poder supervisarse desde un punto central, y se conservará un historial de al menos 30 días. | N-09 | Alta |
| RNF-13 | **Cumplimiento legal.** Los registros de jornada se conservarán durante cuatro años y estarán disponibles para la plantilla y la Inspección de Trabajo. | N-14 | Media |
