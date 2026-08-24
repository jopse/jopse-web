---
title: 'El catálogo de datos dejó de ser un inventario'
description: 'Linaje a nivel de columna, agentes como consumidor principal y conectores como ecosistema: cuatro señales de que el gobierno del dato pasa de pasivo a activo.'
pubDate: 'Aug 25 2026'
---

Durante diez años, la pregunta que se le hacía a un catálogo de datos era "¿qué tenemos?". Un inventario bien mantenido, con sus propietarios, sus etiquetas y su glosario. Esa pregunta ya no basta, y el mercado lleva un par de años moviéndose hacia otra: "¿puedo operar sobre esto?".

Cuatro señales de ese cambio.

## El linaje a nivel de tabla se ha quedado corto

Saber que una tabla alimenta a otra sirve para dibujar diagramas. No sirve para responder a la pregunta que de verdad importa cuando algo se rompe o cuando llega una auditoría: qué campo concreto viajó hasta ese informe y qué transformación sufrió por el camino.

El linaje a nivel de columna, extraído del propio SQL, es la diferencia entre documentar el dato y poder rendir cuentas sobre él.

Y esto ya no es solo una discusión de arquitectura. El AI Act exige poder reconstruir cómo se produjo una decisión automatizada, con registros de granularidad suficiente para ello. Reconstruir una decisión sin saber qué columna alimentó al modelo es un ejercicio de fe.

## La búsqueda por coincidencia exacta es un modelo de 2015

Quien busca en un catálogo casi nunca sabe cómo se llama lo que necesita. Sabe qué problema tiene.

La búsqueda semántica no es una mejora de usabilidad: es lo que separa un catálogo que se usa de uno que se rellena por obligación y se abandona seis meses después.

## El consumidor del catálogo ha cambiado de especie

Los catálogos se diseñaron para que una persona entrara por una interfaz. Hoy quien pregunta cada vez más es un agente, y necesita una superficie pensada para máquinas, no una API pegada a posteriori sobre una UI.

Conviene ser preciso, porque el debate ya se movió: exponer el catálogo a un agente vía MCP ha dejado de ser un diferencial. DataHub y OpenMetadata lo tienen nativo, y el resto va detrás. La pregunta ya no es si un agente puede preguntarle a tu catálogo, sino si lo que recibe está gobernado en el momento exacto de preguntarlo: con los permisos de quien consulta, con el estado de calidad del dato y con el contexto de negocio que evita que el modelo se invente el resto.

## Los conectores son un ecosistema, no un roadmap

Ningún fabricante va a cubrir la matriz de fuentes de sus clientes desde su propio backlog. Los catálogos que ganen serán los que permitan a terceros construir conectores y publicarlos, con un modelo de extensión estable.

Es una decisión de arquitectura, y también de negocio.

## Una sola idea debajo

Debajo de las cuatro hay una sola idea, y no es mía: Gartner describe el paso de las plataformas de gobierno desde la documentación pasiva hacia planos de control activos. De describir políticas a aplicarlas.

Hay una razón por la que esto se ha acelerado justo ahora. Cuando los modelos empiezan a consumir datos corporativos, el catálogo deja de ser una herramienta de cumplimiento y se convierte en infraestructura crítica: es la capa que decide qué puede ver un agente, con qué calidad y bajo qué permiso.

La pregunta de 2027 no será si tienes catálogo. Será si un agente puede fiarse de él.
