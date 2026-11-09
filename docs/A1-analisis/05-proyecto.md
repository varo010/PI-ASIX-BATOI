# 7.5. Definición inicial del proyecto (B5)

En este bloque no se eligen marcas, modelos, direccionamiento ni configuraciones. Solo se define qué debe tener el sistema y para qué. Esas decisiones se tomarán en las prácticas de los módulos.

**Tabla 9.** Ficha del proyecto

| Apartado | Definición |
|---|---|
| Nombre del proyecto | **Proyecto NEXO**: Sistema Informático Empresarial de Grutinet. Se llama así porque une la oficina, el almacén y los canales de venta en un mismo sistema. |
| Finalidad | Dar a Grutinet un sistema informático que centralice la información (catálogo, stock, pedidos, ventas y documentación), conecte las oficinas con el almacén, controle quién accede a cada cosa y proteja el servicio frente a fallos y pérdidas de datos. |
| Problemas o necesidades que resuelve | Las 16 necesidades de B3 (N-01 a N-16). Primero las de prioridad alta: las que mantienen los pedidos en marcha (N-10, N-11, N-12), después las que protegen los datos y los equipos (N-09, N-13, N-14, N-16) y por último las de gestión interna (N-01, N-02, N-04, N-06, N-08). |
| Alcance general | La sede única de Ontinyent: las oficinas y el almacén. Afecta a los nueve departamentos del organigrama (D1-D9). Incluye el acceso desde fuera de la sede para los usuarios autorizados.<br>**Fuera del alcance:** las plataformas de los marketplaces y de los transportistas. Son externas: el sistema trabaja con sus datos, pero no las gestiona. |
| Usuarios principales | Personal de oficinas (D1-D6, D8), personal de almacén (D7), Sistemas (D9), que administra el sistema, y visitantes, que solo tendrán acceso a Internet. |

## Elementos previstos del sistema

**Tabla 10.** Elementos que previsiblemente formarán parte del sistema

| Elemento | Para qué se necesita en Grutinet | Necesidades |
|---|---|---|
| Servidores | Alojar los servicios internos: cuentas de usuario, documentación compartida, aplicación web y base de datos. | N-13, N-14 |
| Equipos cliente | Puestos de las oficinas y lectores o terminales del almacén para consultar y registrar stock y pedidos. | N-11, N-12 |
| Red LAN | Conectar los puestos, los servidores y las zonas fijas del almacén. | N-11, N-15 |
| Red Wi-Fi | Cobertura en el almacén para los lectores y red separada para los visitantes. | N-11, N-15 |
| VLAN | Separar el tráfico de oficinas, almacén, servidores e invitados. | N-15 |
| Almacenamiento | Documentación compartida por departamento con acceso restringido y copias de seguridad. | N-13, N-16 |
| Aplicación web | Herramienta interna para catálogo, stock, pedidos, incidencias, aprovisionamiento, envíos, seguimiento de marcas, informes y registro de jornada. | N-01 a N-08, N-10 a N-12 |
| Base de datos | Guardar en un solo sitio el catálogo, el stock, los pedidos, las ventas de todos los canales y los fichajes. | N-02, N-05, N-06, N-10, N-11 |
| Monitorización | Supervisar servidores, red y servicios y avisar cuando algo falla. | N-09 |
| CPD | Espacio protegido para servidores y equipos de red, con protección frente a cortes eléctricos. | N-09, N-16 |
| Acceso remoto seguro | Que Dirección y Comercial puedan trabajar desde fuera de la sede. | N-01, N-04 |
