# RutasAccesibles — Informe Parte 1

> **Nota de trabajo. Eliminar antes de la entrega.**
> Borrador generado el 2026-11-15 con apoyo de IA a partir de: pauta oficial F01 (`VF_IHC_Evaluacion_Laboratorio_Parte1_Estudiantes.pdf`), presentación de Fase 0 F03 (`PRESENTACION GRUPO 2.pdf`), guion F04 (`PREGUNTAS.md`), modelo de consentimiento F05 y documentación del repositorio (`docs/`).
> No hay entrevistas, citas ni participantes documentados en las fuentes revisadas. Por eso, todo el contenido empírico está marcado como `[PENDIENTE: …]` y las ideas sin validar se rotulan **[HIPÓTESIS]** o **[PROPUESTA]**. Ninguna marca debe borrarse sin incorporar antes la evidencia correspondiente.
> Antes de terminar este informe, el equipo debe resolver las siguientes decisiones del registro `docs/decisiones.md`: DEC-01 (territorio), DEC-02 (perfil de participantes), DEC-03 (guion aplicado), DEC-04 (grabaciones) y DEC-07 (datos ilustrativos en el prototipo).

---

## Portada

**Universidad Mayor**
Interacción Humano-Computador — Evaluación de Laboratorio, Primera parte (Fases 1 y 2)

**RutasAccesibles: información de accesibilidad para planificar desplazamientos urbanos de personas con movilidad reducida en extremidades inferiores**

Equipo *Wo bu zhi dao*

`[PENDIENTE: confirmar la ortografía de los nombres, el nombre de la docente, la sección y la fecha de entrega]`

---

## Índice

`[PENDIENTE: generar el índice automático al exportar a PDF]`

---

## 1. Introducción

En Santiago de Chile, un desplazamiento cotidiano suele combinar tramos peatonales con transporte público. Para una persona con movilidad reducida en las extremidades inferiores, que esa ruta sea viable puede depender de condiciones que cambian de un tramo a otro: pendientes, estado de las veredas, rebajes, escaleras y funcionamiento de ascensores. Muchas personas planifican estos recorridos con aplicaciones de mapas. Este equipo plantea como **supuesto inicial** que esas aplicaciones podrían no considerar suficientemente las diferencias de movilidad entre usuarios y, por ello, recomendar trayectos con barreras de accesibilidad. Este supuesto todavía no ha sido contrastado con usuarios.

El **público objetivo** son personas adultas con movilidad reducida, temporal o permanente, en extremidades inferiores, que se desplazan por Santiago `[PENDIENTE: delimitación territorial acordada — DEC-01]`. El **objetivo del producto** es apoyar a estas personas para que planifiquen y ajusten sus desplazamientos con información de accesibilidad comprensible, oportuna y pertinente para su condición. El producto no busca modificar la infraestructura urbana.

En la Fase 0 el equipo construyó esta frase del problema: *«Personas con movilidad reducida necesitan conocer de antemano el estado de las rutas de la comuna porque la infraestructura actual tiene barreras imprevistas y carece de información clara sobre vías accesibles»*. Para ajustarla al formato solicitado, se propone esta versión: **«Las personas con movilidad reducida en extremidades inferiores necesitan una manera de conocer de antemano las condiciones de accesibilidad de sus rutas, porque la infraestructura presenta barreras imprevistas y la información disponible sobre vías accesibles es poco clara»** `[PENDIENTE: aprobación del equipo y respaldo de la parte «porque» con hallazgos H…]`.

El trabajo aplica el Diseño Centrado en el Usuario (ISO, 2019). En la Fase 1 se realizan entrevistas semiestructuradas a por lo menos tres personas del público objetivo. Sus resultados se sintetizan en hallazgos, una proto-persona, un journey map y necesidades priorizadas. En la Fase 2 esas necesidades orientan la definición de tareas críticas, los flujos, los bocetos y un prototipo navegable de media fidelidad. Una matriz de trazabilidad vincula ambas fases.

> *Control de extensión: unas 330 palabras. Al maquetar, verificar que no supere media página (requisito F01, ítem 1). Si la supera, acortar primero el párrafo de metodología.*

---

## 2. Fase 1: Investigación y comprensión del usuario

### 2.1. Objetivos de investigación

**Objetivo general.** Comprender cómo las personas con movilidad reducida en extremidades inferiores planifican, realizan y ajustan sus desplazamientos urbanos. En particular, se busca entender qué información usan para decidir una ruta, qué papel cumplen las aplicaciones de mapas y otras fuentes, y en qué momentos esa información resulta insuficiente.

**Aspectos que se busca comprender:**

1. **Planificación.** Cómo deciden un trayecto antes de salir y qué tan anticipada es esa decisión según el destino (habitual o poco frecuente).
2. **Fuentes de información.** Qué herramientas digitales, personas u otros medios consultan, y por qué confían en ellas o no.
3. **Criterios de elección.** Qué condiciones del entorno determinan que una ruta sea viable, por ejemplo pendientes, superficies, escaleras, ascensores, distancia o tiempo.
4. **Relación con las aplicaciones de mapas.** Cuándo las usan, cuándo las abandonan y cómo evalúan la correspondencia entre la ruta sugerida y el terreno real.
5. **Imprevistos.** Cómo detectan y resuelven una barrera no anticipada durante el trayecto y qué consecuencias tiene, como tiempo adicional, cansancio, riesgo o dependencia de terceros.
6. **Intermodalidad.** Cómo gestionan los trayectos que combinan tramos a pie o en silla con Metro o buses.
7. **Interacción durante el trayecto.** Qué modalidades (texto, voz, elementos visuales) y qué condiciones de uso del dispositivo resultan pertinentes mientras se desplazan.
8. **Autonomía y apoyo.** En qué situaciones prefieren desplazarse solos, acompañados o pidiendo ayuda, y qué les da seguridad o inseguridad en un trayecto.

**Supuestos de partida y hechos comprobados.** La tabla siguiente separa lo que el equipo supone de lo que ya está comprobado. A la fecha de este borrador, **ningún supuesto ha sido validado empíricamente**.

| ID | Supuesto (Fase 0 y planteamiento posterior) | Origen | Evidencia que lo apoyaría o lo refutaría | Estado |
|---|---|---|---|---|
| HIP-01 | Las personas pierden tiempo al probar rutas no accesibles antes de encontrar un acceso adecuado. | Fase 0, paso 5 | Relatos de desvíos o de retrocesos durante trayectos reales. | `[PENDIENTE: contrastar con H…]` |
| HIP-02 | La incertidumbre aumenta en destinos poco frecuentes o cuando falla un ascensor o una rampa clave. | Fase 0, paso 5 | Comparación entre trayectos habituales y nuevos; experiencias con fallas de infraestructura. | `[PENDIENTE]` |
| HIP-03 | La información insuficiente sobre el estado de las rutas contribuye a retrasos, fatiga, riesgos y pérdida de autonomía. | Fase 0, paso 4 | Consecuencias descritas por participantes y estrategias de compensación. | `[PENDIENTE]` |
| HIP-04 | Las aplicaciones de navegación no representan las barreras relevantes para distintas necesidades de movilidad. | Planteamiento posterior del equipo | Uso real de aplicaciones, criterios para aceptar o modificar rutas, experiencia con indicadores de accesibilidad. | `[PENDIENTE]` |

**Hechos comprobados hasta ahora.** Por ahora solo se ha comprobado lo siguiente: el equipo formuló el problema en la Fase 0, preparó un borrador de guion de entrevista y dispone del modelo de consentimiento informado de la asignatura. Además, la retroalimentación docente recibida orientó al equipo a acotar el territorio y el público objetivo. Ninguno de estos antecedentes constituye evidencia sobre la experiencia de los usuarios.

### 2.2. Metodología

#### 2.2.1. Enfoque y técnica

La investigación tiene un enfoque **cualitativo y exploratorio**, coherente con la etapa de comprensión del contexto de uso del Diseño Centrado en el Usuario (ISO, 2019). Se utilizan **entrevistas semiestructuradas individuales**, presenciales o por videollamada. Esta técnica combina un guion común, que permite comparar respuestas entre participantes, con la flexibilidad necesaria para profundizar en experiencias concretas mediante preguntas de seguimiento. Se eligió porque el objetivo es entender por qué las personas deciden y actúan de cierta manera al desplazarse, no medir la frecuencia de un comportamiento.

`[PENDIENTE: indicar si las entrevistas ya se realizaron. Si no se realizaron, mantener esta sección en tiempo futuro («se realizarán»). Si se realizaron, cambiar a pasado y completar la tabla 2.2.5.]`

#### 2.2.2. Participantes y criterios de selección

Se entrevistará a un **mínimo de tres personas** del público objetivo, identificadas solo con los códigos P1, P2 y P3.

**Criterios de inclusión** `[PROPUESTA — pendiente de acuerdo, DEC-02]`:
- Tener 18 años o más, conforme al modelo de consentimiento de la asignatura.
- Tener movilidad reducida, temporal o permanente, en extremidades inferiores. Esto incluye a personas que usan silla de ruedas, bastón, muletas, andador u ortesis, o que tienen una limitación sin ayuda técnica.
- Desplazarse con regularidad por la zona de estudio `[PENDIENTE: DEC-01]`.

**Criterios de exclusión:**
- Personas que no puedan otorgar consentimiento informado.
- Integrantes del equipo.

No se exigirá que los participantes usen aplicaciones de mapas. Exigirlo introduciría un sesgo de selección y dejaría fuera precisamente a quienes podrían haber dejado de usarlas. Siempre que el reclutamiento lo permita, se buscará variedad en el tipo de condición (temporal o permanente), la ayuda técnica utilizada y el uso de transporte público, porque esa variedad permite identificar coincidencias y contradicciones entre participantes.

**Reclutamiento.** `[PENDIENTE: describir el canal real de contacto sin identificar a nadie, por ejemplo «contactos de la red cercana del equipo». Declarar este sesgo en Limitaciones.]`

#### 2.2.3. Procedimiento

1. **Contacto y consentimiento.** Antes de comenzar, se entrega a cada persona el consentimiento informado de la asignatura. En él se le explica que la participación es voluntaria y que puede omitir preguntas, pausar o terminar la entrevista. Se solicitan por separado las autorizaciones para grabar audio, grabar video, procesar la conversación con transcripción automática o IA y citar frases textuales sin datos identificables.
2. **Registro.** Si la persona autoriza la grabación, se graba la sesión. Si no lo autoriza, una persona del equipo toma notas detalladas mientras otra conduce la entrevista `[PENDIENTE: confirmar con la docente qué evidencia se acepta cuando no hay grabación — DEC-04]`.
3. **Desarrollo.** La entrevista comienza con una pregunta de apertura sobre los desplazamientos habituales y luego avanza por los temas del guion. Para obtener relatos concretos, se privilegian preguntas de seguimiento como «¿me cuentas la última vez que…?» por sobre opiniones generales.
4. **Cierre.** Se pregunta si la persona quiere agregar algo y se le agradece su participación.
5. **Resguardo.** Dentro de las 24 horas siguientes, se resume cada sesión en una ficha (Anexo C). Las grabaciones y los consentimientos firmados se custodian fuera del repositorio público y se entregan a la docente por un canal restringido.

**Duración estimada:** `[PENDIENTE: 30–45 min u otra, según lo aplicado]`.

#### 2.2.4. Guion de entrevista

El guion completo está en el **Anexo A**. Consta de **8 preguntas principales abiertas**, dentro del rango de 6 a 10 que exige la pauta. Cada pregunta tiene sondeos opcionales que se usan para profundizar en experiencias concretas. Las preguntas parten de un trayecto reciente y real, en vez de pedir opiniones generales. Además, la pregunta sobre herramientas admite explícitamente la posibilidad de no usar ninguna, para no suponer que todas las personas usan aplicaciones. La siguiente tabla muestra qué aspectos de investigación (sección 2.1) cubre cada pregunta:

| Pregunta (Anexo A) | Tema | Aspectos de 2.1 que cubre |
|---|---|---|
| P1 | Trayecto reciente | 1, 3, 5 |
| P2 | Planificación | 1 |
| P3 | Herramientas y fuentes | 2, 4 |
| P4 | Elegir el camino | 3, 4 |
| P5 | Imprevistos | 5 |
| P6 | Transporte y conexiones | 6, 7 |
| P7 | Autonomía y apoyo | 8 |
| P8 | Cierre | Abierta: temas no previstos |

*Nota:* en el guion, los códigos P1–P8 identifican **preguntas**; en las tablas de resultados, P1, P2 y P3 identifican **participantes**. `[PENDIENTE: al maquetar, renombrar las preguntas como Q1–Q8 o «Pregunta 1…» para evitar la ambigüedad]`.

La versión del guion presentada en el hito de control `[PENDIENTE: confirmar fecha y resultado de la aprobación docente — DEC-03]` es la que debe adjuntarse. Si el guion aplicado difiere de esa versión, el informe debe indicarlo y justificar el cambio.

#### 2.2.5. Registro de sesiones

| Código | Perfil general (no identificable) | Modalidad | Fecha | Duración | Registro | Consentimiento |
|---|---|---|---|---|---|---|
| P1 | `[PENDIENTE: p. ej., «movilidad reducida permanente; usa silla de ruedas»]` | `[PENDIENTE]` | `[PENDIENTE]` | `[PENDIENTE]` | `[Audio / notas]` | `[Anexo B-1]` |
| P2 | `[PENDIENTE]` | `[PENDIENTE]` | `[PENDIENTE]` | `[PENDIENTE]` | `[PENDIENTE]` | `[Anexo B-2]` |
| P3 | `[PENDIENTE]` | `[PENDIENTE]` | `[PENDIENTE]` | `[PENDIENTE]` | `[PENDIENTE]` | `[Anexo B-3]` |

Esta tabla no debe incluir nombres, comunas de residencia, lugares de estudio o trabajo, ni cualquier otro dato que, combinado con los demás, permita identificar a una persona.

#### 2.2.6. Análisis de la información

El análisis sigue un procedimiento de **síntesis por afinidad**:

1. **Extracción.** Se registra cada observación relevante de las notas o transcripciones en una unidad breve (una idea por nota), etiquetada con el código del participante y su ubicación en la fuente (minuto o línea).
2. **Agrupación.** Las notas se agrupan por similitud de significado, no por la pregunta del guion que las originó. Cada grupo recibe un nombre que expresa un patrón.
3. **Interpretación.** Cada grupo se redacta como un hallazgo (H1, H2…) que explica qué ocurre y por qué es relevante. El hallazgo se respalda con al menos una cita textual autorizada.
4. **Contraste.** Para cada hallazgo se registran los participantes que coinciden y los que difieren, y se comparan los resultados con los supuestos HIP-01 a HIP-04. Así queda explícito qué se confirmó, qué se matizó y qué no tuvo respaldo.
5. **Derivación.** Los hallazgos alimentan la proto-persona, el journey map y las necesidades. Cada rasgo, etapa o necesidad conserva la referencia a su hallazgo de origen.

Para reducir el sesgo de confirmación, al menos dos integrantes revisan la agrupación y se documentan los hallazgos que contradicen la hipótesis inicial.

### 2.3. Resultados y síntesis de hallazgos

`[PENDIENTE: completar con las entrevistas reales. No incluir contenido que no provenga de notas, transcripciones o grabaciones.]`

**Tabla 1.** Síntesis de hallazgos.

| ID | Hallazgo (patrón interpretado) | Evidencia: cita textual | Participantes que lo respaldan | Coincidencias y contradicciones | Supuesto relacionado |
|---|---|---|---|---|---|
| H1 | `[PENDIENTE]` | «`[PENDIENTE: cita P1]`» (P1) | `[P1, P…]` | `[PENDIENTE]` | `[HIP-0x / ninguno]` |
| H2 | `[PENDIENTE]` | «`[PENDIENTE: cita P2]`» (P2) | `[PENDIENTE]` | `[PENDIENTE]` | `[PENDIENTE]` |
| H3 | `[PENDIENTE]` | «`[PENDIENTE: cita P3]`» (P3) | `[PENDIENTE]` | `[PENDIENTE]` | `[PENDIENTE]` |
| H4 | `[PENDIENTE]` | «`[PENDIENTE]`» (P…) | `[PENDIENTE]` | `[PENDIENTE]` | `[PENDIENTE]` |
| H5… | `[PENDIENTE]` | | | | |

**Criterios para completar la tabla:**
- Debe haber al menos una cita textual por participante, copiada literalmente de la grabación o de las notas y con autorización de cita en el consentimiento.
- Un hallazgo explica un patrón, por ejemplo «las personas…, porque…». Una respuesta individual de un participante no es un hallazgo.
- Hay que señalar las contradicciones, por ejemplo cuando un participante confía en la aplicación y otro la evita.

**Contraste con los supuestos iniciales.** `[PENDIENTE: un párrafo que indique cuáles de HIP-01 a HIP-04 se confirmaron, cuáles se matizaron y cuáles no tuvieron respaldo, citando H…]`

**Hallazgos inesperados.** `[PENDIENTE]`

### 2.4. Proto-persona

Con tres entrevistas, la persona resultante es una **proto-persona**. Todos sus rasgos deben poder rastrearse a un hallazgo. Si un campo no tiene respaldo, se deja vacío; no se completa con supuestos.

**Tabla 2.** Proto-persona.

| Campo | Contenido | Hallazgo de origen |
|---|---|---|
| Nombre ficticio y descriptor | `[PENDIENTE: nombre ficticio + rol, p. ej., «la persona que planifica cada salida»]` | — |
| Contexto de movilidad | `[PENDIENTE: tipo de condición y ayuda técnica, si es un patrón observado]` | `[H…]` |
| Desplazamientos habituales | `[PENDIENTE]` | `[H…]` |
| Objetivos al desplazarse | `[PENDIENTE]` | `[H…]` |
| Cómo planifica | `[PENDIENTE]` | `[H…]` |
| Herramientas y fuentes | `[PENDIENTE]` | `[H…]` |
| Frustraciones | `[PENDIENTE]` | `[H…]` |
| Necesidades principales | `[N…]` | `[H…]` |
| Cita representativa | «`[PENDIENTE: cita real]`» (P…) | `[H…]` |

**Exclusiones deliberadas:** solo se incluyen edad exacta, ocupación, nombre de la comuna o rasgos de personalidad si son un patrón entre participantes y si su inclusión no permite identificar a nadie. Si el equipo usa una imagen, debe ser genérica y no representar a un participante.

### 2.5. Journey map

Se propone modelar un desplazamiento urbano en las siguientes etapas. **Esta estructura es una hipótesis de trabajo:** debe ajustarse (fusionando, eliminando o agregando etapas) según lo que relaten los participantes.

1. **Decidir el desplazamiento.** Surge la necesidad de ir a un destino, que puede ser habitual o nuevo.
2. **Planificar.** Se elige la ruta y el medio de transporte antes de salir.
3. **Prepararse y salir.** Se ajustan horarios, compañía o ayudas técnicas.
4. **Recorrer el tramo peatonal.** Se avanza por veredas, cruces y pendientes.
5. **Acceder al transporte público y hacer transbordos.** Incluye estaciones, ascensores y buses.
6. **Enfrentar un imprevisto.** Aparece una barrera no anticipada y hay que ajustar la ruta.
7. **Llegar.** Se accede al destino.
8. **Evaluar después del viaje.** Lo aprendido se aplica a futuros trayectos.

**Tabla 3.** Estructura del journey map. El contenido rotulado **[HIPÓTESIS]** proviene de la Fase 0 o del guion, no de usuarios, y debe reemplazarse o eliminarse con los datos obtenidos.

| | 1. Decidir | 2. Planificar | 3. Preparar | 4. Tramo peatonal | 5. Transporte | 6. Imprevisto | 7. Llegar | 8. Evaluar |
|---|---|---|---|---|---|---|---|---|
| **Acciones** | `[PEND.]` | [HIPÓTESIS] Consulta una aplicación de mapas u otra fuente | `[PEND.]` | `[PEND.]` | `[PEND.]` | [HIPÓTESIS] Busca una alternativa en el lugar | `[PEND.]` | `[PEND.]` |
| **Canales / herramientas** | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` |
| **Pensamientos (cita)** | «`[PEND.]`» | «`[PEND.]`» | | | | | | |
| **Emoción** | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` |
| **Puntos de dolor** | | [HIPÓTESIS, HIP-02] Incertidumbre ante destinos poco frecuentes | | [HIPÓTESIS, HIP-01] Rutas no accesibles | [HIPÓTESIS, HIP-02] Ascensor o rampa fuera de servicio | [HIPÓTESIS, HIP-03] Retraso y fatiga | | |
| **Hallazgo de origen** | `[H…]` | `[H…]` | `[H…]` | `[H…]` | `[H…]` | `[H…]` | `[H…]` | `[H…]` |
| **Oportunidad** | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` | `[PEND.]` |

La fila de emociones solo debe completarse con lo que los participantes expresaron, ya sea en palabras o por el tono documentado en las notas. Para la versión final se recomienda graficar la curva emocional y destacar los dos o tres puntos de dolor más críticos.

### 2.6. Necesidades de usuario

Una necesidad describe **lo que la persona requiere lograr o saber**. Una función describe **lo que el sistema hace** para responder a esa necesidad. Las funciones se definen recién en la Fase 2.

> *Ejemplo de formulación (solo ilustra la redacción; no es una necesidad del proyecto):* correcto: «Saber, antes de salir, si un tramo incluye escaleras»; incorrecto: «Un filtro de rutas sin escaleras».

**Criterio de priorización** `[PROPUESTA — ratificar en equipo]`. Cada necesidad se califica de 1 a 3 en tres dimensiones:
- **Frecuencia (F):** cuántos participantes la expresaron directa o indirectamente (1, 2 o 3 o más).
- **Impacto (I):** cuánto afecta la seguridad, la autonomía o la posibilidad de completar el trayecto (1 = molestia; 2 = retraso o esfuerzo significativo; 3 = riesgo o imposibilidad de llegar).
- **Cobertura actual (C):** cuánto se resuelve hoy con las herramientas existentes (1 = bien resuelta; 3 = sin alternativa).

**Prioridad = F + I + C** (entre 3 y 9). Las necesidades con 7 o más puntos son de prioridad alta y originan las tareas críticas. Si hay un empate, prevalece el mayor impacto.

**Tabla 4.** Necesidades de usuario priorizadas.

| Código | Necesidad (redactada desde la persona usuaria) | Hallazgo de origen | F | I | C | Total | Prioridad |
|---|---|---|---|---|---|---|---|
| N1 | `[PENDIENTE]` | `[H…]` | | | | | |
| N2 | `[PENDIENTE]` | `[H…]` | | | | | |
| N3 | `[PENDIENTE]` | `[H…]` | | | | | |
| N4 | `[PENDIENTE]` | `[H…]` | | | | | |
| N5 | `[PENDIENTE]` | `[H…]` | | | | | |
| N6 | `[PENDIENTE: opcional]` | | | | | | |
| N7 | `[PENDIENTE: opcional]` | | | | | | |
| N8 | `[PENDIENTE: opcional]` | | | | | | |

Se requieren entre 5 y 8 necesidades. Cada una debe derivar de al menos un hallazgo. Si alguna no tiene origen, se elimina.

---

## 3. Fase 2: Diseño y prototipado de la interacción

> **Estado.** Esta sección presenta una **propuesta preliminar** derivada de la problemática y de los supuestos de la Fase 0. A la fecha **no existen bocetos ni prototipo**. Las tareas, los flujos y las pantallas que siguen son candidatos. Antes de adoptarlos, cada uno debe vincularse a una necesidad N de prioridad alta. Las candidaturas que no reciban respaldo de la investigación se descartan, y pueden aparecer otras nuevas. Para no confundir las propuestas con decisiones fundamentadas, se usan los rótulos TC-A, TC-B y TC-C. Los códigos T1… y D1… se asignarán una vez establecida la trazabilidad.

### 3.1. Tareas críticas candidatas

| Candidata | Descripción | Supuesto que la motiva | Necesidad que debe respaldarla |
|---|---|---|---|
| **TC-A** | Planificar un trayecto hacia un destino y comparar alternativas según sus condiciones de accesibilidad, además del tiempo y la distancia. | HIP-01, HIP-04 | `[PENDIENTE: N…]` |
| **TC-B** | Revisar antes de salir las barreras conocidas de cada tramo de una ruta elegida, por ejemplo pendientes, escaleras o ascensores. | HIP-02, HIP-03 | `[PENDIENTE: N…]` |
| **TC-C** | Encontrar una alternativa viable cuando, durante el trayecto, aparece una barrera no prevista. | HIP-02, HIP-03 | `[PENDIENTE: N…]` |

La pauta exige 2 o 3 tareas críticas. La selección final debe corresponder a las necesidades de mayor puntaje en la Tabla 4.

### 3.2. Flujos de interacción candidatos

**TC-A — Planificar y comparar rutas**
1. **Inicio:** la persona indica su origen y su destino.
2. **Decisión:** ¿ya configuró sus condiciones de desplazamiento? Si no lo hizo, el sistema ofrece configurarlas o continuar con valores generales. Esta configuración se basa en necesidades declaradas por la persona; no pide diagnósticos.
3. El sistema muestra las rutas con su tiempo, su distancia y un resumen de las barreras conocidas.
4. **Decisión:** ¿alguna ruta es adecuada? Si ninguna lo es, la persona puede ajustar sus condiciones o el horario.
5. La persona abre el detalle de una ruta.
6. **Fin:** la persona selecciona la ruta y la guarda o la inicia.
7. **Alternativas y errores:** no hay rutas que cumplan las condiciones (estado vacío explicado, con sugerencias); el destino no se encuentra; no hay datos de accesibilidad para un tramo (mostrar la incertidumbre en lugar de omitirla).

**TC-B — Revisar barreras de una ruta antes de salir**
1. **Inicio:** la persona abre una ruta guardada o sugerida.
2. El sistema presenta la ruta dividida en tramos. Cada tramo indica su condición, la fuente del dato y su fecha de actualización.
3. **Decisión:** ¿hay un tramo con una barrera incompatible? Si lo hay, la persona puede solicitar una variante que lo evite.
4. **Fin:** la persona confirma la ruta o la descarta.
5. **Errores:** información desactualizada o no disponible, señalada explícitamente.

**TC-C — Encontrar una alternativa ante un imprevisto**
1. **Inicio:** durante el trayecto, la persona encuentra una barrera no prevista.
2. La persona indica que no puede continuar por ese tramo con una acción directa y visible.
3. El sistema propone alternativas desde la ubicación actual e indica qué barreras tiene cada una.
4. **Decisión:** ¿alguna alternativa sirve? Si ninguna sirve, el sistema ofrece opciones de contingencia `[PENDIENTE: definir según los hallazgos; p. ej., otro medio de transporte]`.
5. **Fin:** la persona continúa por la alternativa elegida.
6. **Opcional:** registrar la barrera para otros usuarios `[PROPUESTA — evaluar si responde a una necesidad]`.
7. **Errores:** sin conexión, ubicación imprecisa o ninguna alternativa disponible.

Los diagramas de flujo definitivos, con símbolos de inicio, fin, decisión y error, se elaborarán en `[PENDIENTE: herramienta]` y se incluirán como Figuras `[PENDIENTE]`.

### 3.3. Pantallas candidatas

| Pantalla candidata | Propósito | Tarea candidata |
|---|---|---|
| P-01 Búsqueda de origen y destino | Iniciar la planificación | TC-A |
| P-02 Condiciones de desplazamiento | Declarar qué barreras evitar o priorizar | TC-A |
| P-03 Resultados comparados | Comparar rutas según accesibilidad, tiempo y distancia | TC-A |
| P-04 Detalle de ruta por tramos | Revisar barreras, fuente y actualidad de la información | TC-B |
| P-05 Alternativa ante imprevisto | Reportar el obstáculo y elegir un nuevo trayecto | TC-C |
| P-06 Estados de vacío, error y sin datos | Comunicar la ausencia de resultados o de información | TC-A, TC-B, TC-C |

La pauta exige bocetos de al menos tres pantallas. Los identificadores definitivos se asignarán junto con la matriz de trazabilidad.

**Bocetos de baja fidelidad.** `[PENDIENTE: fotografías o archivos digitales; anotar los elementos y las iteraciones (Figuras X–Y)]`

**Prototipo de media fidelidad.** `[PENDIENTE: enlace con permiso de visualización + capturas de cada pantalla]`. El prototipo debe permitir completar de principio a fin las tareas críticas elegidas, y mostrar retroalimentación y estados de error. Los datos de rutas que se usen en el prototipo serán ilustrativos y deberán rotularse como tales. Esos datos ilustrativos no constituyen resultados de investigación `[PENDIENTE: confirmar el criterio con la docente — DEC-07]`.

### 3.4. Criterios de usabilidad

De acuerdo con ISO 9241-11 (ISO, 2018), la usabilidad se considera en tres dimensiones, aplicadas aquí a las tareas candidatas:

- **Eficacia.** La persona logra elegir una ruta que se ajusta a sus condiciones declaradas y comprende qué barreras contiene.
- **Eficiencia.** La persona compara las alternativas sin tener que abrir cada ruta por separado. Además, ante un imprevisto, obtiene una alternativa con pocas acciones mientras se desplaza.
- **Satisfacción.** La persona percibe la información como confiable, porque se indican su fuente, su fecha y su grado de certeza, y se siente en control de la decisión final.

Estos criterios se operacionalizarán y medirán en la evaluación de la Parte 2.

### 3.5. Consideraciones de accesibilidad

El producto se dirige a personas con movilidad reducida en las extremidades inferiores, pero la interfaz también debe ser accesible para usuarios con otras condiciones. Además, algunas condiciones de uso son verosímiles en este contexto, como usar el teléfono en movimiento, con una sola mano, con luz solar o con ayudas técnicas. Estas condiciones son **[HIPÓTESIS]** y deben contrastarse con los hallazgos sobre la interacción durante el trayecto. A continuación se enumeran los criterios de WCAG 2.2 (W3C, 2023) que se tomarán como referencia:

| Criterio WCAG 2.2 | Nivel | Aplicación prevista |
|---|---|---|
| 1.4.3 Contraste mínimo | AA | Texto con una relación de contraste de al menos 4.5:1, para facilitar la lectura en exteriores. |
| 1.4.11 Contraste sin texto | AA | Iconos de barreras y controles con un contraste de al menos 3:1. |
| 1.4.1 Uso del color | A | Las barreras no se comunican solo mediante el color de la ruta; se acompañan de iconos y texto. |
| 2.5.8 Tamaño del objetivo (mínimo) | AA | Objetivos táctiles de al menos 24×24 px CSS. Como **[PROPUESTA]**, se usarán tamaños mayores para las acciones críticas en movimiento. |
| 2.5.7 Movimientos de arrastre | AA | El mapa y las listas pueden operarse sin arrastrar, mediante botones alternativos. |
| 2.4.7 Foco visible / 2.4.11 Foco no oculto (mínimo) | AA | Navegación compatible con lectores de pantalla y teclado externo. |
| 3.3.1 Identificación de errores / 3.3.2 Etiquetas o instrucciones | A | Mensajes claros cuando no se encuentra un destino o una ruta. |
| 4.1.3 Mensajes de estado | AA | Avisos de recálculo o de falta de datos que se anuncian sin cambiar el foco. |
| 3.3.7 Entrada redundante | A | Reutilizar las condiciones de desplazamiento ya declaradas en lugar de volver a pedirlas. |
| 1.4.4 Cambio de tamaño del texto / 1.4.10 Reajuste del contenido | AA | La interfaz sigue siendo usable con texto ampliado. |

### 3.6. Principios y pautas de diseño aplicables

Las heurísticas de Nielsen (2024) y las pautas anteriores ofrecen la fundamentación para las decisiones D1… Sin embargo, **un principio no justifica una decisión por sí solo**: cada decisión debe responder primero a una necesidad N.

| Principio | Posible aplicación `[PROPUESTA]` | Supuesto relacionado |
|---|---|---|
| Visibilidad del estado del sistema | Indicar la fuente y la fecha de actualización de cada dato de accesibilidad, así como el estado de recálculo de la ruta. | HIP-02 |
| Coincidencia entre el sistema y el mundo real | Usar el vocabulario de los propios participantes para nombrar las barreras, en lugar de terminología técnica. | `[PENDIENTE: términos observados en entrevistas]` |
| Control y libertad del usuario | Permitir que la persona descarte una sugerencia, ajuste sus condiciones y vuelva atrás sin perder lo configurado. | HIP-04 |
| Prevención de errores | Advertir sobre la barrera de un tramo antes de iniciar el trayecto, no durante él. | HIP-01 |
| Reconocimiento antes que recuerdo | Mostrar en los resultados las condiciones declaradas por la persona, sin obligarla a recordarlas. | — |
| Ayudar a reconocer, diagnosticar y recuperarse de errores | Explicar por qué no hay rutas disponibles y qué puede cambiar la persona para obtenerlas. | HIP-03 |

### 3.7. Decisiones de diseño

`[PENDIENTE: se requieren como mínimo 4 decisiones, registradas una vez que existan necesidades priorizadas y bocetos]`

**Tabla 5.** Decisiones de diseño justificadas.

| Código | Decisión | Necesidad | Principio o pauta (cita precisa) | Alternativa descartada y motivo | Pantalla |
|---|---|---|---|---|---|
| D1 | `[PENDIENTE]` | `[N…]` | `[p. ej., WCAG 2.2, 1.4.1]` | `[PENDIENTE]` | `[P-0…]` |
| D2 | `[PENDIENTE]` | `[N…]` | `[PENDIENTE]` | `[PENDIENTE]` | |
| D3 | `[PENDIENTE]` | `[N…]` | `[PENDIENTE]` | `[PENDIENTE]` | |
| D4 | `[PENDIENTE]` | `[N…]` | `[PENDIENTE]` | `[PENDIENTE]` | |

---

## 4. Matriz de trazabilidad

**Tabla 6.** Matriz de trazabilidad.

| Hallazgo (con cita) | Necesidad | Tarea crítica | Decisión de diseño | Pantalla |
|---|---|---|---|---|
| H1: «`[PENDIENTE]`» (P…) | `[N…]` | `[T…]` | `[D…]` | `[Pantalla …]` |
| H2: «`[PENDIENTE]`» (P…) | `[N…]` | `[T…]` | `[D…]` | `[Pantalla …]` |
| H3: «`[PENDIENTE]`» (P…) | `[N…]` | `[T…]` | `[D…]` | `[Pantalla …]` |
| H…: | | | | |

**Instrucciones para completarla sin inventar evidencia:**

1. La matriz se completa **de izquierda a derecha**. Cada fila parte de un hallazgo de la Tabla 1 con su cita literal y su código de participante. No se agregan filas que comiencen en una pantalla o en una función.
2. Cada necesidad de prioridad alta de la Tabla 4 debe aparecer en la matriz y llegar hasta una pantalla del prototipo.
3. Cada pantalla y cada elemento relevante del prototipo deben aparecer en al menos una fila. Si un elemento no tiene origen, se elimina del prototipo o se justifica que no proviene de una necesidad, por ejemplo un elemento de navegación general.
4. Las celdas de una fila pueden contener varios códigos (por ejemplo, «D1, D3»), pero cada código debe existir en su tabla de origen.
5. Antes de entregar, un integrante que no haya armado la matriz revisa que no haya cadenas rotas, códigos inexistentes ni contradicciones con el texto del informe.

---

## 5. Comentarios finales

### 5.1. Aprendizajes

Los aprendizajes siguientes provienen del trabajo efectivamente realizado hasta ahora.

- **Delimitar el problema es parte de la investigación.** En la revisión de la Fase 0 se constató que el planteamiento alternaba entre una comuna (Providencia), el campus universitario y, posteriormente, Santiago. La retroalimentación docente recibida apuntó en la misma dirección: acotar el territorio y el público para que la investigación fuera abordable. Un alcance amplio dificulta reclutar participantes comparables y vuelve genérica la frase del problema.
- **El guion puede inducir respuestas.** Al revisar el borrador de preguntas se identificaron formulaciones que suponen que la persona usa aplicaciones de mapas. Esto llevó a condicionar esas preguntas y a abrir la pregunta sobre herramientas a la posibilidad de no usar ninguna.
- **El acceso al público es una condición del diseño.** El equipo identificó tempranamente la dificultad de contactar a personas del público objetivo, lo que influye en la factibilidad del alcance elegido.

`[PENDIENTE: aprendizajes derivados de las entrevistas, la síntesis y el prototipado]`

### 5.2. Limitaciones

- **Tamaño de la muestra.** Con tres o pocas más entrevistas, los resultados son exploratorios. No representan a todas las personas con movilidad reducida ni permiten generalizar frecuencias.
- **Reclutamiento** `[PENDIENTE: confirmar]`. Si los participantes provienen de la red cercana del equipo, puede existir un sesgo hacia perfiles similares (por ejemplo, en edad, nivel de uso tecnológico o zona de residencia).
- **Heterogeneidad del público.** Las condiciones temporales y permanentes, y las distintas ayudas técnicas, implican necesidades diferentes. Con una muestra pequeña, es posible que algunas de ellas no queden representadas.
- **Datos autodeclarados.** Las entrevistas recogen relatos y no observación directa del trayecto, por lo que pueden omitir barreras que la persona ya no percibe como tales.
- **Datos ilustrativos en el prototipo.** El prototipo no utiliza datos reales de accesibilidad urbana.

`[PENDIENTE: limitaciones adicionales surgidas en la ejecución]`

### 5.3. Próximos pasos

`[PENDIENTE: completar al cierre]`. Se proponen como base:
1. Validar el prototipo con personas del público objetivo mediante pruebas de usabilidad en la Parte 2.
2. Explorar la observación acompañada de un trayecto real, si se cuenta con el consentimiento correspondiente.
3. Investigar qué fuentes de datos de accesibilidad existen y cuál es su grado de actualización `[PENDIENTE DE INVESTIGACIÓN]`.

---

## Declaración de uso de IA

En la elaboración de este trabajo se utilizaron herramientas de inteligencia artificial generativa como apoyo a la documentación, redacción, organización y desarrollo. Codex se empleó para inventariar los insumos del proyecto, extraer y resumir los requisitos de la pauta y preparar la documentación de colaboración del repositorio. Claude se empleó para redactar un primer borrador de la estructura y el texto de este informe a partir de la pauta y de los documentos del equipo. `[PENDIENTE: verificar con cada integrante si se usó ChatGPT u otras herramientas, para qué y en qué secciones, y completar o eliminar esta mención]`. Ninguna herramienta de IA se utilizó para generar participantes, entrevistas, citas, hallazgos ni resultados. Tampoco reemplazó la investigación ni las pruebas con usuarios. `[PENDIENTE: indicar si se procesaron grabaciones o transcripciones de entrevistas con IA y, de ser así, con qué autorización de los participantes]`. El equipo revisó, corrigió y validó todo el contenido generado y es responsable de la versión final.

---

## Referencias

International Organization for Standardization. (2018). *Ergonomics of human-system interaction — Part 11: Usability: Definitions and concepts* (ISO Standard No. 9241-11:2018).

International Organization for Standardization. (2019). *Ergonomics of human-system interaction — Part 210: Human-centred design for interactive systems* (ISO Standard No. 9241-210:2019).

Nielsen, J. (2024, 30 de enero). *10 usability heuristics for user interface design*. Nielsen Norman Group. https://www.nngroup.com/articles/ten-usability-heuristics/ `[VERIFICAR fecha de actualización en la página]`

World Wide Web Consortium. (2023). *Web Content Accessibility Guidelines (WCAG) 2.2* (W3C Recommendation). https://www.w3.org/TR/WCAG22/

**Fuentes pendientes de investigación** (no citar hasta revisarlas):
- `[PENDIENTE: datos oficiales sobre la prevalencia de discapacidad o de movilidad reducida en Chile, para respaldar el contexto de la Introducción]`.
- `[PENDIENTE: normativa chilena sobre accesibilidad del espacio público y del transporte, si se menciona en el informe]`.
- `[PENDIENTE: estudios sobre navegación y accesibilidad para personas con movilidad reducida, si se usan para contrastar los hallazgos]`.
- `[PENDIENTE: referencia formal del material de clase, si se cita la Fase 0 o el journey map según el formato del curso]`.

---

## Anexos

> Los anexos no cuentan para el límite de 20 páginas. **No incluir nombres, firmas, contactos ni otros datos identificables en la versión pública.** Las grabaciones y los consentimientos firmados se entregan solo por el canal restringido que indique la docente; nunca se suben a GitHub.

### Anexo A. Guion de entrevista

`[PENDIENTE: confirmar que esta es la versión aprobada o aplicada efectivamente — DEC-03]`

**Apertura (no se cuenta entre las preguntas principales).** Presentación del equipo y del objetivo de la conversación. Confirmación del consentimiento y de lo que la persona autorizó (grabación, uso de IA, citas textuales). Recordatorio de que puede omitir preguntas o terminar la entrevista en cualquier momento.

**P1. Trayecto reciente.** Cuénteme de algún desplazamiento que haya hecho en la última semana o mes: desde dónde, hacia dónde y cómo lo hizo.
- Sondeos: ¿Era un trayecto habitual o nuevo? ¿Qué fue lo más fácil y lo más complicado?

**P2. Planificación.** Antes de salir hacia un lugar que no conoce, ¿qué hace para decidir cómo llegar?
- Sondeos: ¿Cuánto tiempo antes lo piensa? ¿Le pregunta a alguien? ¿Cambia algo si el trayecto es habitual?

**P3. Herramientas y fuentes.** ¿Qué herramientas, aplicaciones o personas consulta para eso, si es que consulta alguna?
- Sondeos: ¿Para qué le sirven? ¿En qué momento deja de usarlas o deja de confiar en ellas? Si no usa ninguna: ¿por qué?

**P4. Elegir el camino.** Cuando hay varias formas de llegar, ¿cómo decide cuál tomar?
- Sondeos: ¿Qué características de calles, veredas, pendientes, cruces o accesos considera? ¿Cómo se entera de cómo está el terreno antes de llegar?

**P5. Imprevistos.** Cuénteme de alguna vez en que tuvo que cambiar su recorrido a mitad de camino.
- Sondeos: ¿Qué pasó? ¿Cómo encontró otra opción? ¿Qué información le habría servido en ese momento?

**P6. Transporte y conexiones.** ¿Cómo combina caminar o desplazarse en silla con otros medios de transporte?
- Sondeos: ¿Cómo sabe antes de salir si una estación, paradero o acceso le sirve? ¿Qué información le gustaría ver y cómo, antes y durante el viaje?

**P7. Autonomía y apoyo.** ¿Hay situaciones en que prefiere ir acompañado/a o pedir ayuda, y otras en que no?
- Sondeos: ¿Qué hace que se sienta seguro/a o inseguro/a en un trayecto?

**P8. Cierre.** ¿Hay algo sobre cómo se desplaza por la ciudad que no le haya preguntado y que considere importante?

**Cierre.** Agradecimiento y recordatorio sobre el uso y la conservación de la información.

*Observaciones de revisión para el equipo (eliminar antes de entregar):*
- *Hay sondeos que dan algo por supuesto o piden una solución. «¿En qué momento deja de confiar en ellas?» (P3) supone que la persona desconfía; se puede reemplazar por «¿Cómo se compara lo que ve en la aplicación con lo que encuentra en la calle?». «¿Qué información le habría servido?» (P5) y «¿Qué información le gustaría ver?» (P6) invitan a diseñar la solución; conviene dejarlas al final o reemplazarlas por «¿Qué hizo después, en viajes siguientes?».*
- *«¿Le pregunta a alguien?» (P2) es una pregunta cerrada; se puede reemplazar por «¿Y después de eso, qué más hace?».*
- *Esta versión (8 preguntas) reemplaza el borrador anterior de 10 preguntas. Si el guion presentado en el hito fue el anterior, hay que justificar el cambio en la sección 2.2.4.*

### Anexo B. Consentimientos informados

- B-0: Modelo de consentimiento utilizado (formato de la asignatura, sin datos).
- B-1, B-2, B-3: `[PENDIENTE: consentimiento firmado de cada participante — entregar solo por el canal restringido; en la versión del informe, indicar «consentimiento disponible para la docente» o adjuntarlo con los datos censurados, según lo que indique la docente]`.

### Anexo C. Notas o transcripciones resumidas

Se usará una ficha por participante con la siguiente estructura:

| Campo | Contenido |
|---|---|
| Código | P… |
| Fecha, modalidad y duración | `[PENDIENTE]` |
| Tipo de registro | Audio / video / notas |
| Autorizaciones otorgadas | Audio [ ] Video [ ] IA [ ] Citas [ ] |
| Resumen por bloque del guion | `[PENDIENTE]` |
| Citas textuales autorizadas (con minuto o línea) | `[PENDIENTE]` |
| Observaciones del entrevistador | `[PENDIENTE]` |

### Anexo D. Grabaciones

`[PENDIENTE: indicar el canal restringido de entrega acordado con la docente (no un enlace público) y el listado de archivos por código P…]`. Las grabaciones se eliminarán al término de la asignatura, según se indica en el consentimiento.

### Anexo E. Enlace al prototipo

`[PENDIENTE: enlace con permiso de visualización; comprobar que se abra en una sesión sin iniciar]`

### Anexo F. Bocetos complementarios

`[PENDIENTE: iteraciones y versiones descartadas]`

### Anexo G. Resultado de la Fase 0

Presentación del hito de control: tema inicial, usuario, objetivo, problema, supuestos, preguntas de investigación, frase del problema y reto («¿Cómo podríamos informar y guiar a personas con movilidad reducida de forma intuitiva, oportuna y accesible sobre las mejores rutas de desplazamiento…?»). `[PENDIENTE: incluir la versión presentada y actualizar el reto, que en la Fase 0 se refería al campus, según el alcance acordado en DEC-01]`.
