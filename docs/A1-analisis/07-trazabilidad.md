# Matriz de trazabilidad: necesidad → mejora u oportunidad → proyecto → requisito

La matriz une cada necesidad (B3) con la pregunta de mejora, la mejora interna y la oportunidad de negocio con las que se relaciona (B4), el elemento del proyecto que la resuelve (B5) y los requisitos que la cubren (B6). Así se ve la relación empresa → necesidades → proyecto → requisitos.

En la columna de B4, **P1-P6** son las preguntas de mejora, **MI-1 a MI-16** son las mejoras internas y **ON-1 a ON-3** son las oportunidades de negocio. Todas las necesidades tienen al menos una mejora interna. Solo llevan oportunidad de negocio las necesidades que la hacen posible.

**Tabla 15.** Matriz de trazabilidad

| Necesidad (B3) | Prioridad | Pregunta, mejora interna y oportunidad de negocio (B4) | Elemento del proyecto (B5) | Requisitos (B6) |
|---|---|---|---|---|
| N-01 · Información para decidir y acceso remoto (D1) | Alta | P4 (acceso seguro desde fuera), MI-8 | Aplicación web | RF-08, RF-12 |
| N-02 · Cuadros de mando de tesorería (D2) | Alta | P3 (información centralizada), MI-10 | Aplicación web, base de datos | RF-08 |
| N-03 · Portal del empleado y control de horarios (D2) | Media | P4 (registro de jornada), MI-14 | Aplicación web | RF-13, RNF-10 |
| N-04 · Seguimiento comercial en movilidad (D3) | Alta | P4 (acceso seguro desde fuera), MI-9, ON-2 (nuevos clientes y marketplaces) | Aplicación web | RF-11, RF-12, RNF-07 |
| N-05 · Datos de ventas centralizados y fiables (D5, D6) | Media | P1 (informes para las marcas), P3, MI-15, ON-3 (informes de rendimiento para las marcas) | Aplicación web, base de datos | RF-07, RF-08 |
| N-06 · Previsión de aprovisionamiento (D7) | Alta | P2 (vender lo que no hay), MI-11 | Aplicación web, base de datos | RF-09 |
| N-07 · Documentación de envíos al extranjero (D7) | Media | MI-13, ON-1 (nuevos mercados internacionales) | Aplicación web | RF-10 |
| N-08 · Seguimiento de la mercancía en tránsito (D7) | Alta | P3 (stock centralizado), MI-12, ON-1 | Aplicación web | RF-10 |
| N-09 · Detectar fallos de red y servidores (D9) | Alta | P2 (fallos que nadie ve), P5 (supervisión continua), MI-6 | Monitorización, CPD | RF-14, RNF-05, RNF-08, RNF-09 |
| N-10 · Catálogos multimarca y multicanal (D4) | Alta | P1 (actualizar los canales de venta), P3 (catálogo), MI-4, MI-7, ON-2 | Aplicación web, base de datos | RF-04, RF-07, RNF-11 |
| N-11 · Stock y pedidos en el almacén (D7) | Alta | P1 (preparar los pedidos), P2 (vender lo que no hay), MI-3, MI-7 | Equipos cliente, red LAN, red Wi-Fi, aplicación web, base de datos | RF-05, RF-07, RF-17, RNF-02, RNF-05, RNF-07, RNF-11 |
| N-12 · Estado de pedidos e incidencias (D8) | Alta | P2 (responder tarde), P4 (herramienta interna), MI-16 | Equipos cliente, aplicación web | RF-05, RF-06, RF-17, RNF-07 |
| N-13 · Documentación con acceso restringido (D2) | Alta | P3 (documentación administrativa), P5 (control de accesos), MI-2 | Servidores, almacenamiento | RF-02, RF-03, RNF-06 |
| N-14 · Autenticación centralizada y control de accesos (toda la empresa) | Alta | P4 (cuenta personal), P5 (control de accesos), MI-1, MI-5 | Servidores | RF-01, RF-02, RNF-06 |
| N-15 · Separación del tráfico de red (toda la empresa) | Media | P5 (separar el tráfico), MI-5 | Red LAN, red Wi-Fi, VLAN | RF-16, RNF-01 |
| N-16 · Copias de seguridad y cortes eléctricos (toda la empresa) | Alta | P2 (perder información), P5 (copias y cortes eléctricos), MI-6 | Almacenamiento, CPD | RF-15, RNF-03, RNF-04 |

## Elementos del proyecto y requisitos

**Tabla 16.** Requisitos en los que aparece cada elemento de B5

| Elemento (B5) | Requisitos (B6) |
|---|---|
| Servidores | RF-01, RF-03, RNF-04, RNF-11 |
| Equipos cliente | RF-05, RNF-07 |
| Red LAN | RF-17, RNF-01, RNF-11 |
| Red Wi-Fi | RF-16, RNF-02 |
| VLAN | RNF-01 |
| Almacenamiento | RF-03, RF-15 |
| Aplicación web | RF-05, RF-06, RF-08, RF-09, RF-10, RF-11, RF-12, RF-13 |
| Base de datos | RF-07 |
| Monitorización | RF-14, RNF-08 |
| CPD | RNF-03, RNF-04 |

## Comprobaciones

- [x] **Ninguna necesidad de prioridad alta se queda sin requisito.** Las 12 necesidades altas tienen al menos un requisito.
- [x] **Ningún requisito aparece sin necesidad que lo justifique.** Los 17 RF y los 11 RNF citan al menos una necesidad de B3.
- [x] **Todas las necesidades tienen mejora interna y todas las oportunidades de negocio aparecen en la matriz.** Las 16 necesidades citan al menos una mejora (MI-1 a MI-16) y las tres oportunidades de negocio (ON-1 a ON-3) aparecen en al menos una fila.
- [x] **Los elementos del proyecto (B5) aparecen en los requisitos.** Los 10 elementos tienen al menos un requisito (tabla 16).
