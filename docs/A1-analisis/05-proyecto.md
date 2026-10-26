# 7.5. Definición inicial del proyecto (B5)

> En este bloque **no** se eligen marcas, modelos, direcciones IP ni configuraciones. Solo se define qué debe existir y para qué. Las decisiones técnicas se tomarán en los módulos del ciclo.

**Tabla 9.** Ficha del proyecto

| Apartado | Definición |
|---|---|
| Nombre del proyecto | **Proyecto NEXO**: Sistema Informático Empresarial de Grutinet. El nombre refleja su función de unir oficina, almacén y canales de venta en un mismo sistema. |
| Finalidad | Dotar a Grutinet de una infraestructura informática propia, segura y escalable que centralice la información de catálogo, stock, pedidos y clientes, conecte la oficina con el almacén y garantice la continuidad del servicio, sobre todo en los picos de campaña. |
| Necesidades que resuelve | Las 16 necesidades del bloque 3, con prioridad para las de prioridad alta: N-01, N-02, N-03, N-04, N-06 y N-09 a N-13. |
| Alcance | Sede de Ontinyent completa: oficinas, sala de reuniones y almacén. Los nueve departamentos. Acceso remoto para usuarios autorizados.<br>**Fuera del alcance:** las plataformas de los marketplaces y de los transportistas (son externas: el sistema se relaciona con ellas, pero no las gestiona), la web pública corporativa y la contabilidad que lleva la asesoría externa. |
| Usuarios principales | Personal de oficina (unas 14 personas), personal de almacén (7–8 personas, más en campaña), dirección (con acceso remoto), técnico/a de sistemas (administración del sistema) y visitantes (solo acceso a Internet). |

## Elementos previstos del sistema

**Tabla 10.** Elementos previstos y necesidades a las que responden

| Elemento | Para qué se necesita en Grutinet | Necesidades |
|---|---|---|
| Servidores | Alojar los servicios internos: autenticación, ficheros compartidos, aplicación web y base de datos. | N-01, N-02, N-06, N-10 |
| Equipos cliente | Puestos de oficina y terminales o lectores del almacén para registrar movimientos y pedidos. | N-02, N-03, N-04 |
| Red LAN cableada | Conectar puestos de oficina, servidores y zonas fijas del almacén (expedición, recepción). | N-02, N-15 |
| Red inalámbrica | Cobertura en toda la nave para los terminales y en las oficinas; red de invitados separada para la sala de reuniones. | N-03, N-11 |
| Segmentación de la red (VLAN) | Separar oficinas, almacén, servidores, gestión e invitados. | N-11 |
| Servicio de directorio y autenticación centralizada | Una cuenta por persona, grupos por departamento y permisos por puesto. | N-10, N-06 |
| Almacenamiento centralizado | Carpetas compartidas por departamento y por marca, con historial de versiones. | N-01, N-06, N-08 |
| Sistema de copias de seguridad | Copias automáticas con una copia fuera de las instalaciones y pruebas de restauración. | N-12 |
| Aplicación web interna | Consultar pedidos, stock e incidencias; registrar la jornada; enviar avisos internos. | N-02, N-04, N-14, N-16 |
| Base de datos | Guardar de forma centralizada pedidos, stock, incidencias, ventas y fichajes. | N-02, N-05, N-14 |
| Monitorización | Supervisar servidores, red y servicios y avisar de los fallos. | N-09 |
| CPD / cuarto técnico | Espacio protegido para servidores y equipos de red, con alimentación ininterrumpida y climatización. | N-13, N-12 |
| Acceso remoto seguro | Conexión cifrada para dirección, comerciales y teletrabajo. | N-07 |
