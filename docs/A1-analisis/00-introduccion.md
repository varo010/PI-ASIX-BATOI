# 1. Introducción

Esta memoria recoge la actividad A1 «Análisis de la empresa y definición del proyecto», la primera del Proyecto Intermodular de 1.º de ASIX. Pertenece a la situación de aprendizaje SA1 («De las necesidades de la empresa al proyecto») y trabaja el resultado de aprendizaje RA1, criterios a–f. Es el punto de partida del proyecto de todo el curso: antes de diseñar redes, servidores o servicios hay que entender a qué se dedica la empresa, cómo está organizada y qué problemas tiene.

El grupo 3 ha elegido **Grutinet S.L.**, una empresa de Ontinyent (Valencia) que gestiona la venta de marcas y fabricantes en marketplaces como Amazon, Shein, Miravia o TikTok Shop, con almacén logístico propio. Es una empresa real, cercana a nuestro centro y muy ligada a la informática: todo su negocio ocurre en plataformas digitales, envía cientos de paquetes al día y combina trabajo de oficina con trabajo de almacén. Esa mezcla genera necesidades variadas y fáciles de justificar con datos.

El resultado es un dossier que sigue la cadena **empresa → necesidades → oportunidades → proyecto → requisitos**. Como pide el enunciado, aquí no se toman decisiones técnicas (marcas, modelos, direccionamiento o configuraciones). Esas decisiones se concretarán más adelante, en las prácticas de cada módulo.

# 2. Descripción

El reto de la actividad es responder a la pregunta: **«¿Qué necesita realmente nuestra empresa y qué sistema informático debemos diseñar para responder a esas necesidades?»**. Para ello se elabora un dossier de análisis, necesidades y requisitos dividido en seis bloques:

- **B1 · Presentación y caracterización de la empresa:** sector, actividad, tamaño, sedes, clientes y relaciones.
- **B2 · Organización interna:** departamentos, funciones, perfiles, información que maneja cada uno y organigrama.
- **B3 · Necesidades detectadas:** problemas y riesgos de cada departamento, con su prioridad.
- **B4 · Oportunidades de mejora y justificación:** qué se puede mejorar y por qué la empresa necesita el proyecto.
- **B5 · Definición inicial del proyecto:** nombre, finalidad, alcance, usuarios y elementos previstos.
- **B6 · Catálogo de requisitos:** requisitos funcionales (RF) y no funcionales (RNF) codificados y con prioridad.

La actividad se desarrolla en cuatro sesiones de 55 minutos (lunes 19/10, 26/10, 02/11 y 09/11 de 2026), más trabajo en casa entre sesiones. Los entregables son:

- El documento final en PDF (esta memoria).
- El contenido incorporado al documento general del proyecto.
- El repositorio del proyecto (github.com/varo010/PI-ASIX-BATOI), actualizado durante toda la actividad.
- La bitácora individual y la de grupo (anexo A).

# 3. Objetivos

- Caracterizar Grutinet con fuentes reales y separar con claridad los datos confirmados de los supuestos.
- Identificar los departamentos de la empresa, sus funciones y perfiles, la información que manejan y con quién se comunican.
- Detectar las necesidades informáticas de cada departamento y priorizarlas según su impacto en el negocio.
- Relacionar cada necesidad con una oportunidad de mejora que justifique un Sistema Informático Empresarial.
- Definir el proyecto: finalidad, alcance, usuarios principales y elementos previstos del sistema.
- Redactar requisitos funcionales y no funcionales claros, comprobables, codificados y trazables hasta su necesidad.
- Trabajar en equipo con planificación (Trello) y control de versiones (Git y GitHub).

# 4. Prerrequisitos

## 4.1. Hardware y software

Esta actividad es de análisis, así que solo se han usado herramientas de investigación, documentación y coordinación. No se ha instalado ni configurado ningún equipo.

- Equipos del aula y equipos personales con navegador web.
- LibreOffice Writer para redactar la memoria y exportarla a PDF.
- Git y GitHub: repositorio varo010/PI-ASIX-BATOI, con una rama por persona e integración mediante pull requests.
- Trello: tablero «Proyecto Intermodular · A1 · Grutinet» para repartir y seguir las tareas.
- Graphviz y diagrams.net para el organigrama y los diagramas.
- Fuentes públicas: web corporativa de Grutinet, directorios mercantiles y redes profesionales.

## 4.2. Conocimientos previos

- Conceptos de empresa: sector, actividad, departamento, organigrama, clientes B2B y B2C.
- Funcionamiento básico de un marketplace: vendedor, catálogo, precio, stock, envío, devoluciones y valoraciones.
- Qué es un Sistema Informático Empresarial y cuáles son sus componentes generales (servidores, equipos cliente, red, almacenamiento y servicios).
- Diferencia entre necesidad, oportunidad de mejora, requisito funcional y requisito no funcional.
- Uso básico de Git (ramas, commits, pull requests) y de Markdown.

# 5. Planificación previa de las tareas

Como solo hay una sesión de clase a la semana, cada lunes tiene un objetivo cerrado y el resto se avanza en casa. La planificación se ha volcado en el tablero de Trello con una tarjeta por tarea.

**Tabla 1.** Planificación de la actividad por sesiones

| Fase | Tarea | Descripción y herramientas |
|---|---|---|
| 1 | Sesión 1 · lunes 19/10<br>Conocer la empresa | Reparto de tareas y lectura del enunciado. Investigación de Grutinet (web, directorios mercantiles, LinkedIn) con registro de fuentes. Borrador de B1 y lista de departamentos. Herramientas: navegador, Trello, GitHub. |
| 2 | Sesión 2 · lunes 26/10<br>Organización y necesidades | Tabla de organización (B2) y organigrama. Tabla de necesidades por departamento con su prioridad (B3). Primeras oportunidades de mejora (B4). Herramientas: Writer/Markdown, diagrams.net/Graphviz. |
| 3 | Sesión 3 · lunes 02/11<br>Proyecto y requisitos | Definición inicial del proyecto (B5). Catálogo de requisitos RF y RNF con código y prioridad (B6). Comprobar que cada requisito cubre una necesidad. |
| 4 | En casa · domingo 08/11<br>Trazabilidad y montaje | Matriz de trazabilidad necesidad → oportunidad → elemento → requisito. Montaje del dossier en Writer a partir de los Markdown del repositorio. |
| 5 | Sesión 4 · lunes 09/11<br>Revisión y entrega | Revisión de coherencia y ortografía. Exportación a PDF, incorporación al documento general, subida al repositorio, bitácoras y ensayo de la respuesta a la pregunta final. |

# 6. Organización y distribución del trabajo

Cada integrante se ha responsabilizado de un bloque, pero todos los bloques se han revisado en grupo para que cualquiera pueda explicar cualquier parte del dossier.

> **Para el grupo:** este reparto es una propuesta. Ajustadlo a lo que haya hecho realmente cada persona antes de entregar.

**Tabla 2.** Reparto del trabajo en el grupo 3

| Alumno/a | Tareas realizadas |
|---|---|
| Álvaro | Coordinación, tablero de Trello y repositorio. Definición del proyecto (B5) y montaje final del dossier. |
| Alex | Investigación de Grutinet, registro de fuentes y caracterización de la empresa (B1). |
| Mauro | Tabla de organización y organigrama (B2). |
| Adam | Tabla de necesidades por departamento y justificación de prioridades (B3). |
| Iván | Oportunidades de mejora, respuestas a las preguntas de mejora y justificación del proyecto (B4). |
| Juan Pablo | Catálogo de requisitos RF/RNF (B6) y matriz de trazabilidad. |
| Todo el grupo | Revisión cruzada de todos los bloques, bitácora de grupo y preparación de la respuesta a la pregunta final. |

# 7. Trabajo realizado

Este apartado contiene el dossier propiamente dicho. Cada subapartado corresponde a un bloque del enunciado. Para que los bloques se puedan relacionar entre sí, las necesidades, las oportunidades y los requisitos llevan un código (N-xx, OP-xx, RF-xx y RNF-xx).

Bloques del dossier:

1. [B1 · Presentación y caracterización de la empresa](01-empresa.md)
2. [B2 · Organización interna y departamentos](02-organizacion.md)
3. [B3 · Necesidades detectadas](03-necesidades.md)
4. [B4 · Oportunidades de mejora y justificación del proyecto](04-oportunidades.md)
5. [B5 · Definición inicial del proyecto](05-proyecto.md)
6. [B6 · Catálogo inicial de requisitos](06-requisitos.md)
