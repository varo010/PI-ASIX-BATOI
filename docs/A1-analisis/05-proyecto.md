# 7.5. Definición inicial del proyecto (B5)

*Sistema Informático Empresarial de Grutinet · versión corregida con la v2 del Bloque 4*

## 1. Nombre del proyecto

Sistema Informático Empresarial de Grutinet (**SIE-Grutinet**).

## 2. Finalidad

Disponer de una infraestructura informática común que centralice usuarios y datos, proteja la información, reduzca el trabajo manual repetitivo, detecte los fallos antes de que afecten a las ventas y deje la infraestructura lista para crecer en marcas, productos y pedidos. Con ello, Grutinet ganaría eficiencia, seguridad y capacidad de respuesta ante las marcas y los compradores.

## 3. Problemas y necesidades que pretende resolver

- **Accesos y usuarios:** accesos no autorizados a sistemas críticos y mala gestión de las altas y bajas de personal.
- **Información:** fugas de información confidencial, descontrol documental e incumplimiento normativo.
- **Catálogo y canales:** desincronización de stock, errores en los precios publicados y sobrecarga de trabajo manual al actualizar cada canal.
- **Almacén:** cuellos de botella en el picking, envíos erróneos y paradas operativas (unos 440 pedidos diarios solo en Shein).
- **Red:** congestión que afecta al almacén y propagación de malware desde redes de invitados.
- **Disponibilidad:** caídas del ecommerce o del ERP que paralizan la facturación y la logística.
- **Datos:** pérdida irrecuperable por ransomware, fallos físicos o apagones.
- **Gestión empresarial:** falta de visibilidad en tesorería, compras, importación y documentación aduanera; decisiones de marketing basadas en datos erróneos; tiempos de respuesta lentos en atención al cliente; pérdida de seguimiento de cuentas B2B.
- **RR. HH.:** sanciones por incumplir la normativa de fichaje y carga de trámites manuales.
- **Dirección:** dependencia física de estar en las oficinas centrales para decidir.

## 4. Alcance general

El proyecto afecta a la sede única de Grutinet (oficinas y almacén) y a sus nueve departamentos, que dependen unos de otros: lo que se decide o se vende en las oficinas se ejecuta en el almacén. Los departamentos con necesidades recogidas son:

- D1 · Dirección / Gerencia, D2 · Administración y finanzas (administración, finanzas y RR. HH.), D3 · Comercial y D5 · Marketing y Paid Media / D6 · Análisis de datos (oficinas).
- D4 · Gestión de marketplaces, D8 · Atención al cliente y D7 · Logística y almacén (compras, importación y exportación).
- D7 · Logística y almacén y personal del almacén.
- D9 · Sistemas / Informática, como responsable de la gestión y la monitorización.

Además, el alcance incluye el acceso restringido de terceros (asesoría y auditor) y el acceso remoto seguro para Dirección y la red comercial.

## 5. Usuarios principales

- **Toda la plantilla:** cuenta única, carpetas compartidas por departamento y canal de comunicación interno.
- **D7 · Logística y almacén y personal del almacén:** consulta instantánea de stock y pedidos con lectores por Wi-Fi.
- **D4 · Gestión de marketplaces y D8 · Atención al cliente:** catálogo único, estado de pedidos e incidencias.
- **D1 · Dirección / Gerencia, D2 · Administración y finanzas (finanzas) y D3 · Comercial:** información unificada, cuadros de mando y acceso remoto (CRM en movilidad para la red de ventas).
- **D2 · Administración y finanzas (administración y RR. HH.):** documentación restringida, portal del empleado y control de horarios.
- **D7 · Logística y almacén (compras, importación y exportación):** previsión de compras, trazabilidad de mercancía y documentación aduanera.
- **D5 · Marketing y Paid Media / D6 · Análisis de datos:** datos de ventas unificados de todos los canales.
- **D9 · Sistemas / Informática:** administradores del sistema, gestión de usuarios y monitorización.
- **Terceros con acceso limitado:** asesoría y auditor.

## 6. Principales elementos previstos del sistema

- **Servidores:** gestión centralizada de usuarios y grupos, servidor de archivos, servidores de aplicaciones y de base de datos.
- **Equipos cliente:** puestos de las oficinas y lectores/dispositivos del almacén.
- **Red LAN:** red interna que cubra oficinas y almacén.
- **Red Wi-Fi:** cobertura en el almacén para los lectores, y red de invitados.
- **VLAN:** separación lógica del tráfico en tres zonas: oficinas, almacén e invitados.
- **Almacenamiento:** carpetas por departamento con permisos por grupo, carpeta restringida para asesoría y auditor, y copias de seguridad automatizadas y verificadas.
- **Aplicación web:** CRM accesible en movilidad, portal del empleado, sistema de incidencias, consulta del estado de pedidos y cuadros de mando.
- **Base de datos:** catálogo de productos único sincronizado con los marketplaces y el inventario, y datos de ventas de todos los canales.
- **Monitorización:** vigilancia de servidores, red y servicios con alertas automáticas a Sistemas.
- **CPD:** sala técnica que aloje servidores y equipamiento de red, con protección frente a cortes eléctricos.

Todo ello dimensionado con margen para crecer, sin decidir todavía marcas, modelos, direccionamiento ni configuraciones, tal como pide la actividad.

Versión maquetada en PDF (con los nombres de departamento del primer borrador): [Definición inicial SIE-Grutinet](pdf/Definicion_inicial_SIE-Grutinet.pdf).
