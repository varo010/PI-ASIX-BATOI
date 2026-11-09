# 7.3. Necesidades detectadas (B3)

## Necesidades generales de Grutinet

1. **Mejorar continuamente su tecnología y organización.** Al trabajar con diferentes marketplaces, tiene que gestionar muchos productos, pedidos y precios. Por eso, automatizar tareas le permitiría ahorrar tiempo, reducir errores y trabajar de forma más eficiente.
2. **Mantener una buena logística y atención al cliente.** Los compradores esperan recibir sus pedidos a tiempo y solucionar cualquier problema rápidamente. Si se producen retrasos o errores, la imagen de la empresa y la confianza de sus clientes pueden verse perjudicadas.

   Además, Grutinet necesita controlar sus costes y adaptarse a los cambios del mercado. Las comisiones, la publicidad y los gastos de envío pueden reducir sus beneficios. Por eso, debe analizar qué productos y plataformas le resultan más rentables y actualizar sus estrategias cuando sea necesario.

3. **Formación y buena comunicación entre los departamentos,** ya que todas las áreas deben colaborar para ofrecer un servicio de calidad.

## Análisis de necesidades por departamento

Los departamentos siguen el organigrama de B2 (D1-D9). En el primer borrador la tabla usaba 13 departamentos; las necesidades de Financiero, RRHH y Administración están ahora en D2, y las de Compras, Importación y Exportación en D7. Las filas «Transversal» afectan a toda la empresa y las atiende sobre todo D9.

**Tabla 6.** Necesidades detectadas por departamento

| Cód. | Departamento | Necesidad detectada | Problema o riesgo asociado | Prioridad |
|---|---|---|---|---|
| N-01 | D1 · Dirección / Gerencia | Información clara para la toma de decisiones y capacidad de acceso remoto | Parálisis estratégica ante imprevistos y dependencia física de estar en las oficinas centrales. | Alta |
| N-02 | D2 · Administración y finanzas (finanzas) | Cuadros de mando en tiempo real e integración bancaria/ERP automatizada | Riesgo de impagos, desajustes de tesorería y retrasos en los cierres mensuales. | Alta |
| N-03 | D2 · Administración y finanzas (personal) | Portal del empleado, registro centralizado de tareas y control de horarios | Sanciones por incumplimiento de normativa de fichaje y carga manual de procesos burocráticos. | Media |
| N-04 | D3 · Comercial | Implantación de un CRM accesible en movilidad para la red de ventas | Pérdida de oportunidades comerciales y falta de seguimiento de las grandes cuentas B2B. | Alta |
| N-05 | D5 · Marketing y Paid Media / D6 · Análisis de datos | Disponer de datos de ventas que sean centralizados y fiables | Toma de decisiones comerciales basada en datos erróneos y campañas con bajo retorno (ROI). | Media |
| N-06 | D7 · Logística y almacén (aprovisionamiento) | Previsión automatizada de aprovisionamiento conectada a las ventas | Roturas de stock en productos clave o exceso de inventario inmovilizando capital. | Alta |
| N-07 | D7 · Logística y almacén (envíos al extranjero) | Plataforma para digitalización y seguimiento de documentación aduanera | Retrasos de entrega en el extranjero y posibles multas por errores documentales. | Media |
| N-08 | D7 · Logística y almacén (mercancía en tránsito) | Trazabilidad en tiempo real de contenedores y mercancía en tránsito | Falta de visibilidad en la cadena de suministro que impacte los tiempos de reposición. | Alta |
| N-09 | D9 · Sistemas / Informática | Monitorización para detectar fallos en la red y los servidores a tiempo | Caídas del sistema (plataformas de venta o programas de gestión) que paralicen la facturación y la logística de la empresa. | Alta |
| N-10 | D4 · Gestión de marketplaces | Trabajar simultáneamente sobre catálogos multimarca y multicanal sin duplicar ficheros | Desincronización de stock, errores en precios publicados y sobrecarga de trabajo manual. | Alta |
| N-11 | D7 · Logística y almacén | Consulta instantánea de stock/pedidos y cobertura Wi-Fi en almacén para lectores | Cuellos de botella en la preparación de pedidos (picking), envíos erróneos y paradas operativas. | Alta |
| N-12 | D8 · Atención al cliente | Acceso rápido y directo al estado de los pedidos y gestión de incidencias | Tiempos de respuesta lentos, insatisfacción del cliente B2B y pérdida de reputación. | Alta |
| N-13 | D2 · Administración y finanzas (documentación) | Sistema de documentación compartida con acceso restringido a los datos | Fugas de información confidencial, descontrol documental e incumplimiento normativo. | Alta |
| N-14 | Transversal (Toda la empresa) | Sistema de autenticación centralizada y control de accesos de usuarios | Accesos no autorizados a sistemas críticos y mala gestión de seguridad en las altas/bajas de personal. | Alta |
| N-15 | Transversal (Toda la empresa) | Separación lógica del tráfico de red (oficinas, almacén, invitados) | Propagación de malware desde redes de invitados y congestión que afecte al rendimiento del almacén. | Media |
| N-16 | Transversal (Toda la empresa) | Copias de seguridad automatizadas y protección frente a cortes eléctricos | Pérdida de datos irrecuperable (por ransomware o fallos físicos) y daños en el hardware por apagones. | Alta |

## Priorización de las necesidades y justificación de los riesgos

Para dar la prioridad nos hemos hecho tres preguntas sobre cada necesidad:

1. **¿Para la venta o los envíos si no se resuelve?** Si la respuesta es sí, es Alta: Grutinet vive de que los pedidos salgan cada día.
2. **¿Puede hacer perder datos, dinero o la confianza de las marcas y los marketplaces?** Si es sí, también es Alta, aunque no pare el trabajo en el momento.
3. **¿Solo hace el trabajo más lento o más incómodo?** Entonces es Media: conviene resolverla, pero la empresa puede seguir funcionando mientras tanto.

**Tabla 6b.** Resumen de prioridades y por qué

| Prioridad | Necesidades | Por qué tienen esa prioridad |
|---|---|---|
| Alta | Stock y catálogo sincronizados (D4), consulta de stock y pedidos en el almacén (D7), estado de pedidos para atención al cliente (D8) | Afectan directamente a los unos 440 envíos diarios. Un error vende productos agotados, retrasa pedidos o hace pasar los plazos de respuesta, y el marketplace penaliza la cuenta de todas las marcas. |
| Alta | Copias de seguridad y protección frente a cortes eléctricos, monitorización de red y servicios (D9) | Sin ellas, una avería, un apagón o un ataque pueden parar toda la empresa o hacer perder datos que no se recuperan. |
| Alta | Control de accesos centralizado y documentación compartida con acceso restringido (D2 y toda la empresa) | Grutinet guarda datos de compradores, de trabajadores y de las marcas. Una fuga supone incumplir el RGPD y perder la confianza de los clientes. |
| Alta | Información para decidir y acceso remoto (D1), cuadros de mando de tesorería (D2), seguimiento de las marcas (D3), aprovisionamiento y mercancía en tránsito (D7) | Si fallan, se toman malas decisiones, se pierden marcas cliente o hay roturas de stock en productos clave. |
| Media | Registro de jornada y portal del empleado (D2), datos de ventas para las campañas (D5/D6), documentación de envíos al extranjero (D7), separación del tráfico de red (toda la empresa) | Son importantes, pero hoy se pueden cubrir con más trabajo manual sin que se paren las ventas. El registro de jornada es obligatorio, así que no puede esperar mucho. |

**Orden de atención:** primero lo que mantiene los pedidos en marcha (D4, D7, D8), después lo que protege los datos y los equipos (D9 y control de accesos) y por último lo que mejora la gestión interna (D1, D2, D3, D5 y D6).

Versiones maquetadas en PDF: [Necesidades por departamento B3](pdf/Necesidades%20por%20departamento%20B3.pdf) · [Sesión 2 · Necesidades y oportunidades](pdf/Sesi%C3%B3n%202%20%C2%B7%20Necesidades%20y%20oportunidades.pdf).
