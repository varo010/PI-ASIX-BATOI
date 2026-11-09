# Matriz de trazabilidad: necesidad → oportunidad → requisito

La matriz une cada necesidad (B3) con la oportunidad de mejora de la que parte (B4), el elemento del proyecto que la resuelve (B5) y los requisitos que la cubren (B6). Así se ve la relación empresa → necesidades → proyecto → requisitos.

En la columna de oportunidad, **P1-P6** son las preguntas de mejora de B4 y **O1-O4** son las oportunidades de mejora de B4.

**Tabla 13.** Matriz de trazabilidad

| Necesidad (B3) | Prioridad | Oportunidad (B4) | Elemento del proyecto (B5) | Requisitos (B6) |
|---|---|---|---|---|
| N-01 · Información para decidir y acceso remoto (D1) | Alta | P4 (acceso seguro desde fuera), O3 (usar los datos para decidir) | Aplicación web, acceso remoto seguro | RF-08, RF-12 |
| N-02 · Cuadros de mando de tesorería (D2) | Alta | P3 (información centralizada), O3 | Aplicación web, base de datos | RF-08 |
| N-03 · Portal del empleado y control de horarios (D2) | Media | P4 (registro de jornada) | Aplicación web | RF-13, RNF-10 |
| N-04 · Seguimiento comercial en movilidad (D3) | Alta | P4 (acceso seguro desde fuera), O2 (nuevos clientes y marketplaces) | Aplicación web, acceso remoto seguro | RF-11, RF-12, RNF-07 |
| N-05 · Datos de ventas centralizados y fiables (D5, D6) | Media | P1 (informes para las marcas), P3, O3 | Aplicación web, base de datos | RF-07, RF-08 |
| N-06 · Previsión de aprovisionamiento (D7) | Alta | P2 (vender lo que no hay), O3 | Aplicación web, base de datos | RF-09 |
| N-07 · Documentación de envíos al extranjero (D7) | Media | O1 (nuevos mercados internacionales) | Aplicación web | RF-10 |
| N-08 · Seguimiento de la mercancía en tránsito (D7) | Alta | P3 (stock centralizado), O1 | Aplicación web | RF-10 |
| N-09 · Detectar fallos de red y servidores (D9) | Alta | P2 (fallos que nadie ve), P5 (supervisión continua) | Monitorización, CPD | RF-14, RNF-05, RNF-08, RNF-09 |
| N-10 · Catálogos multimarca y multicanal (D4) | Alta | P1 (actualizar los canales de venta), P3 (catálogo) | Aplicación web, base de datos | RF-04, RF-07 |
| N-11 · Stock y pedidos en el almacén (D7) | Alta | P1 (preparar los pedidos), P2 (vender lo que no hay) | Equipos cliente, red LAN, red Wi-Fi, aplicación web, base de datos | RF-05, RF-07, RNF-02, RNF-05, RNF-07 |
| N-12 · Estado de pedidos e incidencias (D8) | Alta | P2 (responder tarde), P4 (herramienta interna) | Equipos cliente, aplicación web | RF-05, RF-06, RNF-07 |
| N-13 · Documentación con acceso restringido (D2) | Alta | P3 (documentación administrativa), P5 (control de accesos) | Servidores, almacenamiento | RF-02, RF-03, RNF-06 |
| N-14 · Autenticación centralizada y control de accesos (toda la empresa) | Alta | P4 (cuenta personal), P5 (control de accesos) | Servidores | RF-01, RF-02, RNF-06 |
| N-15 · Separación del tráfico de red (toda la empresa) | Media | P5 (separar el tráfico) | Red LAN, red Wi-Fi, VLAN | RF-16, RNF-01 |
| N-16 · Copias de seguridad y cortes eléctricos (toda la empresa) | Alta | P2 (perder información), P5 (copias y cortes eléctricos) | Almacenamiento, CPD | RF-15, RNF-03, RNF-04 |

## Elementos del proyecto y requisitos

**Tabla 14.** Requisitos en los que aparece cada elemento de B5

| Elemento (B5) | Requisitos (B6) |
|---|---|
| Servidores | RF-01, RF-03, RNF-04 |
| Equipos cliente | RF-05, RNF-07 |
| Red LAN | RNF-01 |
| Red Wi-Fi | RF-16, RNF-02 |
| VLAN | RNF-01 |
| Almacenamiento | RF-03, RF-15 |
| Aplicación web | RF-05, RF-06, RF-08, RF-09, RF-10, RF-11, RF-13 |
| Base de datos | RF-07 |
| Monitorización | RF-14, RNF-08 |
| CPD | RNF-03, RNF-04 |
| Acceso remoto seguro | RF-12 |

## Comprobaciones

- [x] **Ninguna necesidad de prioridad alta se queda sin requisito.** Las 12 necesidades altas tienen al menos un requisito.
- [x] **Ningún requisito aparece sin necesidad que lo justifique.** Los 16 RF y los 10 RNF citan al menos una necesidad de B3.
- [x] **Los elementos del proyecto (B5) aparecen en los requisitos.** Los 11 elementos tienen al menos un requisito (tabla 14).
