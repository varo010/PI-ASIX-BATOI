# 10. Dificultades encontradas

- **Información interna no pública.** La web de Grutinet explica sus servicios, pero no su plantilla ni su organización. Lo hemos resuelto deduciendo los departamentos a partir de los servicios y marcando como supuesto todo lo no confirmado (tabla 4).
- **Datos que no coinciden.** Cada fuente daba un número de trabajadores distinto (21, 26 o el tramo de 11 a 50). Hemos trabajado con un rango y lo hemos indicado así.
- **Separar la necesidad de la solución.** Al principio escribíamos cosas como «necesitan un servidor». Las hemos reformulado como problemas («necesitan una única versión de cada ficha») para no adelantar decisiones técnicas.
- **Requisitos vagos.** Varios borradores decían «la red debe ir bien». Los hemos reescrito con valores comprobables (tiempos, número de días, cobertura).
- **Coordinación con una sola sesión semanal.** Hemos repartido el trabajo por bloques en Trello, con una rama por persona en GitHub y revisión en grupo al empezar cada sesión.

# 11. Ampliación de información

## Las métricas de los marketplaces como motor de las necesidades

Los marketplaces evalúan continuamente a sus vendedores. En Amazon, por ejemplo, se vigilan la tasa de pedidos defectuosos (objetivo por debajo del 1 %), la tasa de envíos tardíos (por debajo del 4 %), la tasa de cancelaciones del vendedor (por debajo del 2,5 %) y el tiempo de respuesta a los compradores (menos de 24 horas). Si se superan esos límites, la cuenta puede perder visibilidad o incluso ser suspendida. Como Grutinet envía los pedidos desde su propio almacén, esos indicadores dependen directamente de su organización interna. Por eso las necesidades de stock en tiempo real (N-02), cobertura en el almacén (N-03) y atención al cliente (N-04) tienen prioridad alta.

## Obligaciones legales que afectan al sistema

- **RGPD y LOPDGDD:** Grutinet trata datos personales de compradores (nombre, dirección, teléfono) y de su plantilla. Debe limitar el acceso a quien lo necesite y poder demostrarlo (RNF-07).
- **Registro de jornada (Real Decreto-ley 8/2019):** es obligatorio registrar a diario el inicio y el final de la jornada de cada trabajador y conservar los registros cuatro años (RF-14, RNF-13).

## Estacionalidad

En el comercio electrónico las ventas se concentran en campañas como Black Friday, Navidad, Prime Day o las rebajas. En esas semanas suben a la vez los pedidos, las consultas de clientes y, posiblemente, el personal temporal del almacén. Un sistema dimensionado solo para un día normal fallaría justo cuando más se vende, y por eso se han incluido requisitos de escalabilidad (RNF-01) y de disponibilidad en campaña (RNF-02).

# 12. Conclusiones

Esta actividad nos ha enseñado que un proyecto informático no empieza eligiendo equipos, sino entendiendo la empresa. Analizar Grutinet nos ha permitido ver que sus necesidades no son genéricas: nacen de su modelo de negocio, de vender en plataformas que penalizan los errores y de tener almacén propio, y por eso el stock en tiempo real, la cobertura del almacén y la continuidad del servicio pesan más que en una oficina corriente.

También hemos aprendido a redactar requisitos que se puedan comprobar y a mantener la trazabilidad: gracias a los códigos y a la matriz, cualquier requisito se puede justificar con una necesidad real. Este dossier será la base del resto del Proyecto Intermodular: en los módulos técnicos se diseñarán y montarán la red, los servidores y los servicios del Proyecto NEXO, y se comprobará que cumplen los requisitos definidos aquí.

Como mejora, nos habría gustado contrastar los supuestos con la propia empresa. Si fuera posible, el siguiente paso sería contactar con Grutinet para validar la organización interna y las necesidades detectadas.
