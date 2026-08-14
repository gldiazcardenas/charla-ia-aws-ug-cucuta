# El futuro del desarrollo de software luego de la Inteligencia Artificial

**AWS User Group Cúcuta** · Guion v2

---

## Cómo leer este documento

Cada sección tiene dos columnas separadas en bloques:

- **PANTALLA** — qué se ve proyectado en ese momento. Una idea por pantalla.
- **GUION** — qué se dice en voz alta. Escrito para leer y ensayar, no para proyectar.
- **NOTA** — indicaciones de entrega: pausas, preguntas al público, cambios de ritmo.
- **TIEMPO** — en qué minuto deberías empezar y terminar esa sección.
- **CONTROL DE RELOJ** — al inicio de cada acto: el rango que ocupa y a partir de qué minuto vas atrasado.

Cuando pasemos esto a slides, cada `PANTALLA` se convierte en una diapositiva y su `GUION` en las notas del presentador.

El desglose completo de tiempos, los puntos de control y el plan de recorte están en un documento aparte: [`Cronometraje-charla-IA-AWS-UG.md`](Cronometraje-charla-IA-AWS-UG.md).

---

## Ficha de la charla

| | |
|---|---|
| **Público** | Estudiantes de ingeniería de sistemas, desarrolladores en ejercicio, comunidad AWS |
| **Idea central** | La IA no está acabando con los ingenieros de software. Está acabando con una definición demasiado pequeña de lo que significa ser ingeniero de software. |
| **Pregunta que abre** | Si escribir código deja de ser nuestra principal ventaja competitiva, ¿cuál será nuestro valor? |
| **Respuesta que cierra** | Nuestro valor estará cada vez menos en producir líneas de código y cada vez más en entender problemas, diseñar sistemas, tomar decisiones, evaluar alternativas y garantizar que lo que construimos realmente funcione. |
| **Frase que se llevan** | El código se está volviendo barato. El criterio sigue siendo caro. |
| **Actos** | 5 + cierre · 25 secciones · 37 pantallas |
| **Duración estimada** | **39:58** de charla, sobre un espacio de 60 min → ~20 min para Q&A |
| **Palabras habladas** | 2.606 |

---
---

# ACTO 0 · Esta no era la charla que iba a dar

**CONTROL DE RELOJ** · Este acto ocupa de **00:00** a **08:08** (8m 08s, 20% de la charla). Si al terminarlo tu reloj pasa de **09:38**, estás atrasado. Es recuperable: acelera 1.3.

## 0.1 · Quién les habla

**TIEMPO** · 00:00 → 01:15 · 1m 15s

**PANTALLA** — Foto a la izquierda. A la derecha, bullets simples y los tres enlaces al pie.

**GUION**

Antes de empezar, un minuto sobre mí, para que sepan desde dónde les estoy hablando.

Soy Gabriel Díaz. Soy ingeniero de sistemas de la UFPS — de aquí.

Llevo diecisiete años en desarrollo de software. Hoy soy CEO y fundador de GLD Consulting, y trabajo como consultor de TI para empresas en Estados Unidos: Twilio, Livevox, Inpowered AI, Attain Outcomes.

Soy Arquitecto de Soluciones AWS y programador Java certificado.

Y en este momento estoy cursando un Máster en Inteligencia Artificial en el Instituto Europeo de Postgrado — que es, en buena parte, de dónde sale la inquietud que originó esta charla.

**NOTA** — Menciona la UFPS con intención. Si en la sala hay estudiantes de allí, esa frase hace más por tu credibilidad que toda la lista de clientes. Estás diciendo "yo estuve sentado donde ustedes están".

**NOTA** — Un minuto. No más. Los enlaces están en pantalla; no los leas en voz alta, solo di "ahí quedan mis datos si quieren escribirme". Un speaker que se presenta largo pierde la sala antes de empezar.

---

## 0.2 · El cambio de tema

**TIEMPO** · 01:15 → 02:55 · 1m 40s

**PANTALLA** — El tema original: *AWS Lambda · microVMs*. Un diagrama simple o solo las palabras, sobre fondo oscuro. Es la charla que no van a ver.

**GUION**

Quiero comenzar contándoles algo.

Esta no era la charla que originalmente iba a dar.

Cuando comenzamos a pensar en este evento, la idea inicial era hablar de **las microVMs detrás de AWS Lambda**.

Y era un tema buenísimo. Cómo AWS logra arrancar una máquina virtual completa en milisegundos, con su propio kernel y su propio aislamiento, para ejecutar la función de un solo cliente y después destruirla. Cómo eso resuelve al mismo tiempo el problema de la seguridad multi-tenant y el del arranque en frío. Podía mostrar el modelo de ejecución, hacer una demo, y terminar con recomendaciones prácticas.

Es exactamente la clase de tema que a mí me gusta: entender cómo funciona algo por dentro.

**NOTA** — Este párrafo tiene que sonar entusiasta, no como excusa. El giro funciona solo si el público cree que el tema original valía la pena. No lo despaches en dos segundos.

Pero mientras preparaba esa charla apareció una pregunta mucho más incómoda.

**NOTA** — Pausa. Deja que la pregunta llegue sola antes de proyectarla.

**PANTALLA** — Una sola línea, grande:
> ¿Tiene sentido hablar solamente de nuevas tecnologías cuando está cambiando la manera misma en la que construimos tecnología?

**GUION**

Porque algo extraño está pasando en nuestra industria.

---

## 0.3 · Por qué esta vez es diferente

**TIEMPO** · 02:55 → 04:54 · 1m 59s

**PANTALLA** — A la izquierda, la lista: *nuevo lenguaje · nuevo framework · nueva arquitectura · nueva plataforma cloud · nueva forma de desplegar*. A la derecha, la infografía `multimedia/1786485118307.jpeg`: el stack de un desarrollador Java en 2015 contra 2026 — una mochila con seis items frente a una silueta cubierta por cincuenta tecnologías.

**GUION**

Quienes trabajamos en tecnología estamos acostumbrados al cambio.

Cada cierto tiempo aparece un nuevo lenguaje, un nuevo framework, una nueva arquitectura, una nueva plataforma cloud, una nueva forma de desplegar software.

Y nuestra reacción como ingenieros siempre ha sido bastante sencilla:

> "Bueno... toca aprenderlo."

Aprendimos Git. Aprendimos contenedores. Aprendimos cloud. Aprendimos CI/CD. Aprendimos nuevos frameworks.

Y seguimos adelante.

Miren esta imagen. A la izquierda, lo que necesitaba saber un desarrollador Java en 2015: seis cosas en una mochila. A la derecha, 2026.

**NOTA** — Deja la imagen en pantalla y haz la pregunta al público: *"¿esto es progreso, o es carga?"* No la respondas todavía — la respuesta llega en 1.3, cuando hablemos de que la abstracción mueve el nivel en vez de eliminarlo. Vale unos treinta segundos de reacción de la sala.

Pero con la inteligencia artificial empecé a pensar que estaba pasando algo distinto.

**NOTA** — Baja el ritmo aquí. Esta es la primera idea fuerte de la charla.

**PANTALLA** — Una línea:
> La nueva herramienta puede hacer una parte del trabajo que durante años usamos para definir nuestra profesión.

**GUION**

Porque esta vez la nueva herramienta no solamente nos ayuda a hacer nuestro trabajo.

**Puede hacer una parte del trabajo que durante años usamos para definir nuestra profesión.**

Puede escribir código. Puede crear pruebas. Puede explicar un repositorio completo. Puede modificar repositorios completos. Puede encontrar errores. Puede crear infraestructura. Puede proponer arquitecturas. Puede documentar. Puede tomar una tarea y empezar a implementarla sola.

Entonces la pregunta dejó de ser una y pasó a ser otra.

**PANTALLA** — Dos preguntas, la primera tachada:
> ~~¿Qué nueva tecnología debería aprender un ingeniero?~~
> **¿Qué significa ser ingeniero cuando una máquina también puede programar?**

---

## 0.4 · La misma pregunta, tres versiones

**TIEMPO** · 04:54 → 07:08 · 2m 14s

**PANTALLA** — Tres bloques con las tres preguntas, apareciendo uno por uno.

**GUION**

Seguramente muchos de los estudiantes que están aquí han pensado alguna vez:

> "¿Será que escogí la carrera correcta?"

O quizá:

> "Estoy aprendiendo Java, Python o JavaScript mientras ChatGPT, Claude, Kiro y Copilot ya pueden generar todo esto."

Y entonces aparece inevitablemente:

> **¿Para qué estoy aprendiendo a programar?**

Pero esta pregunta no es solamente de los estudiantes.

Los que llevamos algunos años trabajando tenemos nuestra propia versión:

> **¿Lo que sé hacer hoy seguirá siendo valioso dentro de cinco años?**

Y las empresas tienen otra:

> **¿Qué debería esperar de un ingeniero de software si tiene inteligencia artificial disponible todo el tiempo?**

Tres perspectivas diferentes sobre el mismo cambio.

**NOTA** — Si el público es mayoritariamente estudiantes, pregunta a mano alzada quién se ha hecho la primera pregunta. Genera complicidad temprana.

---

## 0.5 · Lo que vamos a conversar hoy

**TIEMPO** · 07:08 → 08:08 · 1m 00s

**PANTALLA** — Cinco preguntas numeradas. Esta pantalla se puede repetir como marcador entre actos.

**GUION**

Así que decidí cambiar el tema.

Porque quizá lo más útil que puedo hacer hoy no es enseñarles otra herramienta, sino conversar sobre qué está pasando con nuestra profesión.

Hoy quiero que respondamos cinco preguntas:

1. ¿Qué cambió realmente con la inteligencia artificial?
2. ¿Se va a acabar el trabajo para los programadores?
3. ¿Qué pasa cuando dejamos que la IA escriba software que nosotros mismos no entendemos?
4. ¿Vale la pena aprender a programar?
5. ¿Qué deberíamos aprender ahora?

**NOTA** — Cada pregunta corresponde exactamente a un acto, en orden. Si proyectas esta pantalla entre actos, resalta la que estás por responder.

No tengo una bola de cristal. Pero sí podemos mirar lo que está ocurriendo hoy y entender hacia dónde se está moviendo la profesión.

---
---

# ACTO I · De dónde venimos

**CONTROL DE RELOJ** · Este acto ocupa de **08:08** a **15:09** (7m 01s, 18% de la charla). Si al terminarlo tu reloj pasa de **16:39**, estás atrasado. Todavía es recuperable: acelera 2.1 y 2.4.

## 1.1 · Las tres horas y los treinta segundos

**TIEMPO** · 08:08 → 10:01 · 1m 53s

**PANTALLA** — Arriba, el contraste en dos líneas: *3 horas — aprendiendo a construirlo* · *30 segundos — para que una IA lo escriba*. Abajo, grande: **¿Perdieron esas tres horas?**

**GUION**

Quiero empezar con una pregunta para los estudiantes.

¿Cuántos están aprendiendo ahora mismo Java, Python, JavaScript, C#, Go o algún otro lenguaje?

**NOTA** — Espera las manos. No sigas hasta que se levanten.

Ahora imaginen que mañana aparece una herramienta capaz de escribir en treinta segundos el código que a ustedes les tomó tres horas aprender a construir.

¿Perdieron esas tres horas?

**NOTA** — Pausa larga. Tres segundos completos. No respondas todavía.

¿O estaban aprendiendo algo mucho más importante que escribir código?

Esa es probablemente una de las preguntas más importantes para cualquier persona que esté estudiando ingeniería en este momento.

Vamos a volver a ella al final.

**NOTA** — Este es el gancho que se cierra en el Acto de cierre. No lo resuelvas aquí.

---

## 1.2 · Cuatro etapas de la abstracción

**TIEMPO** · 10:01 → 12:34 · 2m 34s

**PANTALLA** — Línea de tiempo con cuatro hitos, revelados uno a uno.

**GUION**

Para entender hacia dónde vamos, primero hay que recordar de dónde venimos.

Porque hay algo que solemos olvidar: **esta no es la primera vez que una tecnología hace que programar sea más fácil.** De hecho, prácticamente toda la historia de nuestra industria consiste en eso.

**Primera etapa: programar era hablar con la máquina.**

El desarrollador tenía que conocer profundamente memoria, estructuras de datos, sistemas operativos, compiladores, lenguajes, infraestructura.

Construir software era costoso. El código era escaso.

**Segunda etapa: aparecen las abstracciones.**

Llegaron los frameworks, las bibliotecas, cloud computing, los servicios administrados, las APIs, Infrastructure as Code, CI/CD, los contenedores.

Antes alguien configuraba servidores físicamente. Después escribíamos scripts. Después aparecieron Terraform, CloudFormation, CDK. Después, plataformas completamente administradas.

Cada generación permitió hacer más con menos esfuerzo. **La industria siempre ha avanzado eliminando trabajo manual.**

**NOTA** — Callback opcional al tema abandonado. Funciona muy bien aquí y cuesta veinte segundos.

Y fíjense en algo, volviendo al tema del que les iba a hablar.

Cuando ustedes suben una función a Lambda, escriben veinte líneas y se olvidan del resto. Esa es la abstracción.

Pero debajo de esas veinte líneas alguien tuvo que diseñar una microVM que arranca en milisegundos, aislar la ejecución de miles de clientes distintos y decidir qué pasa cuando algo falla.

La abstracción no eliminó ese trabajo. **Lo movió de lugar.** Y alguien lo sigue haciendo.

Guárdense esa idea, porque vamos a volver a ella.

**Tercera etapa: Google, Stack Overflow y GitHub.**

El desarrollador dejó de memorizar todo. Aprendimos a buscar. Y una habilidad fundamental pasó a ser *saber encontrar la respuesta correcta*.

**Cuarta etapa: IA generativa.**

Aquí pasa algo distinto. Ya no solamente buscamos la respuesta. Ahora podemos decir "construye esta funcionalidad" — y la máquina lo hace.

Por primera vez estamos automatizando parcialmente **la producción del código mismo**.

Ahí está el verdadero cambio.

**NOTA** — La infografía "2015 vs 2026" ya la mostraste en 0.3. Si alguien la trae de vuelta aquí, retómala: la segunda etapa es exactamente lo que hizo crecer esa silueta.

---

## 1.3 · La abstracción nunca eliminó al ingeniero

**TIEMPO** · 12:34 → 14:00 · 1m 25s

**PANTALLA** — Cuatro pares en columna: *Calculadora / matemáticas · Hoja de cálculo / financieros · Compilador / programadores · Cloud / ingenieros de infraestructura*.

**GUION**

Y aquí conviene recordar algo, porque esta conversación ya la tuvimos antes.

Las calculadoras no hicieron innecesario aprender matemáticas. Hicieron innecesario hacer ciertos cálculos a mano.

Las hojas de cálculo no eliminaron a los financieros. Los hicieron capaces de trabajar con problemas más grandes.

Los compiladores no eliminaron a los programadores porque dejamos de escribir ensamblador. Los lenguajes de alto nivel tampoco.

Cloud no eliminó a los ingenieros porque dejamos de instalar servidores físicamente.

**NOTA** — Ritmo de lista. Cada par debe caer con confianza, sin explicación adicional.

**PANTALLA** — Una línea:
> La abstracción mueve el nivel en el que resolvemos los problemas.

**GUION**

**La abstracción mueve el nivel en el que resolvemos los problemas.**

La IA está haciendo exactamente eso. Nos está obligando a subir un nivel.

---

## 1.4 · El código se volvió barato

**TIEMPO** · 14:00 → 15:09 · 1m 09s

**PANTALLA** — La frase sola, en grande:
> El código se está volviendo barato. El criterio sigue siendo caro.

**GUION**

Lo que pasó, en el fondo, es que **la IA cambió radicalmente la economía de producir software**.

Durante décadas el código fue escaso y caro. Eso ya no es cierto.

Y si tuviera que resumir toda esta charla en una frase, sería esta:

**El código se está volviendo barato. El criterio sigue siendo caro.**

Generar trescientas líneas de código puede tomar segundos.

Pero sigue siendo difícil responder si son las trescientas líneas correctas.

Y de eso quiero hablar ahora.

---
---

# ACTO II · Lo que cambió en el trabajo

**CONTROL DE RELOJ** · Este acto ocupa de **15:09** a **21:06** (5m 57s, 15% de la charla). Si al terminarlo tu reloj pasa de **22:36**, estás atrasado. No toques el Acto III — recorta 5.2 según el plan del cronometraje.

## 2.1 · Las preguntas que la IA no responde por ti

**TIEMPO** · 15:09 → 16:06 · 57s

**PANTALLA** — Lista de preguntas, apareciendo una por una, acumulándose hasta llenar la pantalla.

**GUION**

Estas son las preguntas que siguen siendo difíciles:

¿Resuelve el problema que teníamos? ¿Es seguro? ¿Escala? ¿Cuánto va a costar en producción? ¿Qué pasa cuando falle un servicio del que depende? ¿Estamos almacenando bien los datos? ¿Cumplimos con privacidad y regulación? ¿Es esta realmente la arquitectura que necesitamos?

**NOTA** — Lee rápido, en avalancha. El efecto es acumulativo: que se sienta el peso de todo lo que la IA no decide.

La IA puede producir una respuesta.

**El ingeniero sigue siendo responsable de determinar si es una buena respuesta.**

---

## 2.2 · La nueva unidad de productividad

**TIEMPO** · 16:06 → 17:21 · 1m 15s

**PANTALLA** — Dos diagramas, uno encima del otro:
> Problema → desarrollador → código
> Problema → ingeniero → IA / agentes / herramientas → software

**GUION**

Antes pensábamos así: problema, desarrollador, código.

Ahora es así: problema, ingeniero, IA y agentes y herramientas, software.

Esto significa que una persona puede producir mucho más que antes.

Pero también significa algo más incómodo.

**NOTA** — Pausa antes de la línea siguiente. Es el giro del acto.

**PANTALLA** — Una línea:
> Una mala decisión también se puede producir muchísimo más rápido.

**GUION**

**Una mala decisión también se puede producir muchísimo más rápido.**

Con IA podemos acelerar buenas decisiones. Pero también podemos acelerar deuda técnica, vulnerabilidades, arquitecturas deficientes, complejidad innecesaria, costos cloud y errores.

La velocidad no reemplaza al conocimiento.

**La velocidad multiplica aquello que ya sabemos hacer.**

---

## 2.3 · De programador a ingeniero aumentado

**TIEMPO** · 17:21 → 19:15 · 1m 54s

**PANTALLA** — Tres columnas: *Ayer · Hoy · Mañana*. Se llenan una por una.

**GUION**

Y si esto es la dirección, vale la pena preguntarse cómo se ve el trabajo en el tiempo.

**Ayer**, el desarrollador escribía a mano la mayor parte del código.

**Hoy**, el desarrollador escribe código junto con asistentes de IA.

**Mañana** — y aquí especulo, pero no mucho — el ingeniero probablemente va a coordinar múltiples agentes y herramientas trabajando en paralelo: implementando funcionalidades, escribiendo pruebas, **revisando código**, desplegando infraestructura, **analizando vulnerabilidades**, generando documentación, **investigando incidentes**.

Fíjense en el verbo. No "escribir". **Coordinar.**

**NOTA** — Esta es la transición conceptual más importante del acto. Si algo se recuerda de esta sección, que sea el cambio de encargo que viene ahora.

**PANTALLA** — Dos encargos de trabajo, el primero pequeño y gris, el segundo grande:
> "Escribe esta función."
> "Este es el sistema que necesitamos. Estas son sus restricciones. Estas son las condiciones bajo las cuales debe funcionar. **Demuestra que cumple con ellas.**"

**GUION**

Y eso cambia la forma del encargo que uno recibe.

El trabajo se va a parecer cada vez menos a:

> "Escribe esta función."

Y cada vez más a:

> "Este es el sistema que necesitamos. Estas son sus restricciones. Estas son las condiciones bajo las cuales debe funcionar. **Demuestra que cumple con ellas.**"

**NOTA** — Pausa en "demuestra". Esa palabra es la bisagra de toda la charla: la carga de la prueba se queda con el ingeniero, no con la herramienta.

Esa última parte es la que no se delega.

La IA puede construir el sistema. **Demostrar que cumple sigue siendo tu trabajo.**

---

## 2.4 · Qué buscan ahora las empresas

**TIEMPO** · 19:15 → 21:06 · 1m 51s

**PANTALLA** — Dos frases, la de arriba desvaneciéndose:
> "Sé programar en X."
> **"Sé resolver problemas usando software."**

**GUION**

Durante muchos años una entrevista podía estar dominada por preguntas como: ¿conoces Java? ¿sabes React? ¿has trabajado con Spring? ¿sabes hacer una API REST?

Eso sigue teniendo valor. Pero cada vez es menos suficiente.

Porque la empresa no contrata a alguien porque sabe escribir Java.

La empresa tiene clientes, procesos, restricciones, riesgos, dinero, infraestructura, datos y problemas.

Y necesita personas capaces de convertir todo eso en sistemas confiables.

Por eso el perfil valioso se está moviendo de *"sé programar en X"* hacia *"sé resolver problemas usando software"*.

**NOTA** — Aquí baja el registro. Deja el tono de conferencia y habla como si le contaras algo a un amigo. Esta es la única parte de la charla donde el argumento deja de ser una idea y pasa a ser tu vida.

**PANTALLA** — Dos columnas. A la izquierda, *Lo que sé*: **Java**. A la derecha, *Lo que uso todos los días*: **Rust · Python · TypeScript · GCP · Terraform**.

**GUION**

Y les voy a contar algo personal, porque para mí esto no es teoría.

Hace un año y medio trabajo para un cliente en Estados Unidos. El proyecto es en Rust, Python y TypeScript, sobre infraestructura en Google Cloud manejada con Terraform.

Yo soy programador Java. Java neto. Y me encanta Java.

No sabía Rust cuando entré. Y si por "saber Rust" ustedes entienden poder sentarme a escribirlo de memoria, todavía no sé Rust. Tampoco Python.

**NOTA** — Pausa aquí. Deja que la sala procese que acabas de admitir eso en público.

Y la empresa lo sabía. Desde la primera entrevista sabían que yo venía de Java.

Me contrataron igual.

¿Por qué?

Porque no me estaban contratando por la sintaxis. Me contrataron porque sé construir software.

Llevo año y medio entregando en ese proyecto, y lo he logrado por dos cosas — en este orden.

Primero: porque entiendo cómo se diseña un sistema, cómo se modela la información, cómo se maneja la concurrencia, qué es una buena prueba, qué significa operar algo en producción.

Segundo: porque tengo inteligencia artificial disponible para todo lo que no me sé de memoria.

**NOTA** — El orden importa y hay que decirlo con énfasis. Si el público invierte esos dos factores, se lleva exactamente la lección contraria a la que quieres dejar.

Fíjense en el orden. Si fuera solamente la IA, no funcionaría.

**NOTA** — Este párrafo es obligatorio. Sin él, un estudiante de primer semestre concluye "entonces no necesito aprender a programar" — y le habrás hecho daño. No lo recortes nunca, aunque vayas pasado de tiempo.

Y quiero ser muy claro con esto, porque es fácil sacar la lección equivocada.

Esto no significa que no haya que aprender a programar. Significa exactamente lo contrario.

Yo puedo trabajar en Rust sin dominar Rust **porque pasé años dominando Java lo suficientemente bien como para entender qué está haciendo un programa por debajo**.

Sin esos años, la IA me habría entregado código que yo no habría sabido evaluar.

---
---

# ACTO III · La trampa

**CONTROL DE RELOJ** · Este acto ocupa de **21:06** a **25:45** (4m 39s, 12% de la charla). Si al terminarlo tu reloj pasa de **27:15**, estás atrasado. Este es el punto de control que más importa: aplica el plan de recorte del cronometraje ahora, no más adelante.

## 3.1 · Vibe coding: lo que sí funciona

**TIEMPO** · 21:06 → 22:31 · 1m 25s

**PANTALLA** — Secuencia de prompts, tipo conversación de chat:
> "Haz que este botón funcione." → "Ahora agrega autenticación." → "Ahora conecta una base de datos." → "Corrige este error."

**GUION**

Quiero hablar del vibe coding, y quiero hablarlo con justicia — porque es extraordinariamente útil.

Una persona describe lo que quiere, la IA genera algo, lo prueba superficialmente y sigue iterando.

"Haz que este botón funcione." "Ahora agrega autenticación." "Ahora conecta una base de datos." "Corrige este error."

Y en poco tiempo tenemos una aplicación funcionando.

Para prototipos, experimentos, hackathones, aprender y validar ideas, esto es increíble. De verdad. No estoy aquí a decirles que no lo usen.

El problema empieza en otro punto.

**PANTALLA** — Dos frases, la segunda apareciendo después:
> "Funciona en mi computador."
> "Está listo para producción."

**GUION**

El problema empieza cuando confundimos *"funciona en mi computador"* con *"está listo para producción"*.

---

## 3.2 · El interrogatorio

**TIEMPO** · 22:31 → 24:30 · 1m 59s

**PANTALLA** — Cada pregunta aparece sola. La respuesta "No sabemos." aparece debajo, en rojo, y se queda acumulándose.

**GUION**

Imaginemos que le pedimos a una IA crear una aplicación.

Después de veinte prompts tenemos frontend, backend, login, base de datos, API y despliegue.

Todo parece funcionar.

Entonces alguien pregunta:

**NOTA** — Aquí baja la voz y cambia el ritmo. Pregunta y responde tú mismo, dejando un segundo entre cada par. Este es el momento más memorable de la charla — no lo apures.

¿Cómo funciona la autenticación?

*No sabemos.*

¿Por qué elegimos esta base de datos?

*No sabemos.*

¿Qué pasa si tenemos diez mil usuarios concurrentes?

*No sabemos.*

¿Dónde están almacenados los secretos?

*No sabemos.*

¿Cuánto cuesta operar esto?

*No sabemos.*

**NOTA** — Pausa larga.

**PANTALLA** — Una línea, sola, sobre negro:
> Somos propietarios de un sistema que no entendemos.

**GUION**

Y aparece el problema de fondo.

**Somos propietarios de un sistema que no entendemos.**

Ese es, para mí, el riesgo más importante de construir software solamente mediante prompts.

---

## 3.3 · La paradoja de la IA

**TIEMPO** · 24:30 → 25:45 · 1m 15s

**PANTALLA** — Una línea:
> Mientras más código pueda escribir la IA, más importantes se vuelven los fundamentos de ingeniería.

**GUION**

Lo que nos lleva a la idea más contraintuitiva de esta charla.

**Mientras más código pueda escribir la IA, más importantes se vuelven los fundamentos de ingeniería.**

¿Por qué? Porque alguien tiene que reconocer cuándo la IA propone algo incorrecto.

Para detectar una mala arquitectura necesitas conocer arquitectura.

Para detectar una vulnerabilidad necesitas conocer seguridad.

Para detectar una consulta ineficiente necesitas entender bases de datos.

Para evaluar código concurrente necesitas entender concurrencia.

Para diseñar un sistema distribuido necesitas entender sistemas distribuidos.

**NOTA** — Ritmo de lista otra vez. Cada línea con la misma cadencia, sin adornos.

La IA reduce la necesidad de recordar sintaxis.

Pero aumenta la necesidad de **comprender conceptos**.

**NOTA** — Callback a tu historia. Es importante hacerlo: desde que la contaste, parte del público viene pensando *"pero lo que él hace, ¿no es lo mismo que el vibe coding que acaba de criticar?"*. Esta es la respuesta. No la dejes sin dar.

Y aquí quiero volver un momento a lo que les conté de mí.

Yo no sé Rust de memoria. Pero si la IA me propone un manejo de concurrencia equivocado en Rust, lo detecto.

No porque sepa Rust. Porque entiendo concurrencia.

**NOTA** — Pausa. Esta es la distinción más fina de toda la charla.

Esa es exactamente la diferencia entre lo que yo hago y el vibe coding del que hablábamos hace un momento.

No está en la herramienta. Las dos personas usan la misma herramienta.

**Está en lo que uno trae.**

---
---

# ACTO IV · ¿Entonces vale la pena aprender a programar?

**CONTROL DE RELOJ** · Este acto ocupa de **25:45** a **30:00** (4m 15s, 11% de la charla). Si al terminarlo tu reloj pasa de **31:30**, estás atrasado: entrega 5.2 como referencia rápida a las slides.

## 4.1 · Sí — pero qué significa programar

**TIEMPO** · 25:45 → 27:00 · 1m 16s

**PANTALLA** — Bloque de código con las palabras `for` `if` `while` `class` `function`, tachadas. Al lado, la lista de lo que programar realmente enseña.

**GUION**

Volvamos a la pregunta que muchos estudiantes tienen de verdad: ¿vale la pena pasar años aprendiendo a programar si una IA puede escribir código?

**Sí.**

Pero tenemos que ser mucho más precisos sobre qué significa aprender a programar.

Porque aprender a programar no consiste en recordar cómo escribir `for`, `if`, `while`, `class` y `function`.

Programar enseña a dividir problemas grandes en problemas pequeños. A construir abstracciones. A modelar información. A pensar en estados. A manejar errores. A comprender algoritmos. A razonar sobre eficiencia. A diseñar interfaces. A depurar sistemas. A pensar sistemáticamente.

Eso no se depreció. Eso subió de valor.

---

## 4.2 · Del prompt a la especificación

**TIEMPO** · 27:00 → 28:20 · 1m 19s

**PANTALLA** — Dos flujos, uno encima del otro:
> Prompt → código → prompt → más código
> Idea → requisitos → diseño → tareas → implementación → pruebas

**GUION**

Y aquí hay algo particularmente interesante.

Si la IA es capaz de escribir el código, entonces una de las habilidades más valiosas pasa a ser **explicar con precisión qué queremos construir**.

Eso nos mueve de *prompt-driven development* a *spec-driven development*.

No decir simplemente "créame una aplicación para reservas", sino definir qué problema resuelve, cuáles son sus requisitos, cuáles son sus restricciones, qué comportamientos esperamos, cuáles son los criterios de aceptación y cómo debería probarse.

**NOTA** — Aquí entra Kiro por primera y única vez como concepto. No lo trates como "otro editor con IA" — trátalo como la evidencia de que la industria se está moviendo en esta dirección.

Y noten algo del segundo flujo: la IA no participa solo en el paso de escribir código. Participa en todos — ayudando a redactar los requisitos, a proponer el diseño, a partir el trabajo en tareas, a implementar y a probar.

Esto no es una teoría mía. Es hacia donde se está moviendo el tooling.

AWS tiene una herramienta que se llama **Kiro**, y su propuesta es exactamente esta: convertir prompts en requisitos, diseños arquitectónicos y tareas ordenadas, y después implementarlos.

Y hay un detalle que me parece revelador: antes de escribir código, Kiro revisa los requisitos buscando **contradicciones y vacíos**.

Piénsenlo un segundo. La herramienta no está optimizando la escritura de código. Está optimizando la calidad de la especificación.

**PANTALLA** — Una línea:
> La IA no elimina la ingeniería. Nos obliga a hacerla explícita.

**GUION**

**La IA no elimina la ingeniería. Nos obliga a hacerla explícita.**

---

## 4.3 · Las cinco capas

**TIEMPO** · 28:20 → 30:00 · 1m 40s

**PANTALLA** — Cinco capas apiladas, construyéndose de abajo hacia arriba. Cada capa se destaca mientras hablas de ella.

**GUION**

Entonces, ¿qué debería aprender hoy un estudiante? Yo lo agruparía en cinco capas.

**Capa 1 — Fundamentos.**

No abandonen programación, estructuras de datos, algoritmos, bases de datos, redes, sistemas operativos, concurrencia, Git.

No porque vayamos a escribirlo todo a mano. Sino porque necesitamos saber **qué está haciendo la máquina por nosotros**.

Les dije que volvíamos a las microVMs de Lambda. Es esto.

Nadie necesita saber cómo arranca un microVM para escribir una función. Hasta el día en que la función tarda tres segundos en responder, y hay que entender qué es un arranque en frío, por qué existe y qué se puede hacer al respecto.

Ese día, el que entendió la capa de abajo resuelve el problema. El que solo sabía la de arriba, abre un ticket.

**NOTA** — Este es el cierre del hilo que abriste en 0.1 y retomaste en 1.2. Con esto el tema abandonado deja de ser una anécdota y se convierte en argumento.

**Capa 2 — Ingeniería de software.**

Diseño, testing, patrones, APIs, observabilidad, seguridad, mantenibilidad, refactoring, documentación, arquitectura.

Cuando generar código es barato, distinguir **buen software de software que simplemente funciona** se vuelve mucho más importante.

**Capa 3 — Cloud.**

Cómputo, redes, almacenamiento, bases de datos, identidad, seguridad, serverless, observabilidad, infraestructura como código.

Porque escribir la aplicación es solo una parte del problema. Después la aplicación tiene que existir en el mundo real.

**Capa 4 — Inteligencia artificial.**

No todos tienen que convertirse en investigadores de machine learning. Pero sí deberían entender modelos fundacionales, contexto, tokens, embeddings, RAG, agentes, tool use, MCP, evaluación, seguridad de aplicaciones con IA, y los costos y límites de los modelos.

La IA tiene que volverse parte normal del toolbox del ingeniero.

**Capa 5 — Habilidades humanas.**

Y aquí posiblemente esté la ventaja competitiva más grande: pensamiento crítico, comunicación, entendimiento del negocio, capacidad de hacer buenas preguntas, capacidad de trabajar con ambigüedad, criterio técnico, liderazgo, responsabilidad.

**NOTA** — Pausa antes del remate.

Porque una IA puede producir veinte alternativas.

**Alguien todavía tiene que escoger una.**

---
---

# ACTO V · La ruta concreta

**CONTROL DE RELOJ** · Este acto ocupa de **30:00** a **35:33** (5m 34s, 14% de la charla). Si al terminarlo tu reloj pasa de **37:03**, estás atrasado. Salta directo a 6.1: el cierre son 4m 25s y se entregan completos, siempre.

**NOTA** — Aquí la charla deja de ser conceptual y se vuelve accionable. Cambia la energía: menos reflexión, más instrucción. Si vas corto de tiempo, este es el acto que se comprime — pero nunca se elimina, porque es lo único que el público se puede llevar y ejecutar el lunes.

## 5.1 · El orden importa

**TIEMPO** · 30:00 → 32:11 · 2m 12s

**PANTALLA** — Siete pasos numerados, revelados uno a uno.

**GUION**

Las cinco capas responden *qué* aprender. Ahora quiero responder *en qué orden*.

Si yo hoy estuviera empezando ingeniería, haría esto:

**Uno. Aprendería un lenguaje suficientemente bien.**

Python, Java, JavaScript, C#, Go. El lenguaje concreto importa mucho menos que aprender bien los fundamentos con él.

**Dos. Aprendería Git.**

Porque el software real se construye entre varias personas.

**Tres. Construiría dos o tres proyectos que pueda explicar.**

No veinte tutoriales. Dos o tres sistemas que pueda defender en una entrevista, línea por línea si hace falta.

**Cuatro. Desplegaría esos proyectos.**

Infraestructura, base de datos, logs, seguridad, monitoreo. Es aquí donde cloud deja de ser un tema de examen y se vuelve real. Y es aquí donde uno entiende por qué la arquitectura y el diseño de sistemas se volvieron tan valiosos: es ahí donde se están desplazando las decisiones que importan.

**Cinco. Usaría IA desde el primer día.**

Pero con una sola regla, siempre:

> ¿Entiendo lo que acaba de generar?

Si la respuesta es no, ese es el trabajo de hoy.

**Seis. Aprendería a escribir especificaciones, no solamente prompts.**

**Siete. Construiría evidencia de que sé hacer cosas.**

GitHub. Proyectos desplegados. Arquitecturas documentadas. Experimentos. Contribuciones. Certificaciones. Experiencia.

---

## 5.2 · Los recursos: la escalera de AWS

**TIEMPO** · 32:11 → 35:33 · 3m 22s

**PANTALLA** — Cuatro escalones: *AWS Educate → AWS Skill Builder → Kiro → Certificaciones*.

**GUION**

Y todo esto se puede hacer con recursos gratuitos. Déjenme darles la escalera concreta.

**Escalón uno: AWS Educate.**

Es gratuito, abierto a cualquier persona sin importar su nivel educativo o su experiencia, y no pide tarjeta de crédito. Se puede registrar desde los trece años con solo un correo.

Tiene laboratorios prácticos sobre almacenamiento con S3, cómputo con EC2, redes con VPC, bases de datos con RDS y operaciones en la nube. Y da insignias digitales que se pueden compartir.

Si tienen dieciocho años o más, además tienen acceso a la bolsa de empleo de AWS Educate.

El mensaje aquí es sencillo:

> No necesitan esperar a conseguir su primer empleo para empezar a trabajar con tecnologías cloud.

**Escalón dos: AWS Skill Builder.**

Aquí el aprendizaje se vuelve estructurado: cloud, arquitectura, seguridad, datos, inteligencia artificial.

Es importante que sepan qué es gratis y qué no, porque la diferencia importa cuando uno es estudiante:

- **Gratis:** los sets oficiales de preguntas de práctica de veinte preguntas, los cursos Exam Prep de dos horas, y AWS Cloud Quest, que es aprender cloud jugando.
- **Con suscripción (desde 29 dólares al mes):** los exámenes de práctica oficiales completos, laboratorios, y los cursos Exam Prep extendidos de seis a ocho horas.

Se puede llegar muy lejos con solo lo gratuito.

**Escalón tres: Kiro.**

Aquí es donde practican lo que hablamos en el Acto IV: pasar de prompts a especificaciones.

Tiene una capa gratuita, funciona como IDE, como CLI y en el navegador, y no necesitan una cuenta de AWS — pueden entrar con GitHub, Google o un AWS Builder ID.

**NOTA IMPORTANTE — sé honesto con esto.** Kiro tiene un plan de estudiantes con 1.000 créditos mensuales gratis por un año, pero hoy solo aplica a un listado de universidades de Estados Unidos y Canadá. Ninguna universidad colombiana está en la lista todavía. No prometas lo que no hay.

Pero sí hay algo concreto que pueden hacer: en `kiro.dev/students` hay un formulario para registrar su correo institucional y pedir que incluyan su universidad. Si suficientes estudiantes de acá lo hacen, es una señal real. Y mientras tanto, la capa gratuita ya les alcanza para aprender.

**Escalón cuatro: las certificaciones.**

Y aquí quiero ser cuidadoso, porque no las voy a vender como "saca este certificado y consigues trabajo".

Una certificación es dos cosas: **una estructura para aprender**, y **una forma de validar lo que ya sabes**.

AWS las organiza en cuatro niveles: Foundational, Associate, Professional y Specialty. Y ya tiene certificaciones específicas de IA — la de Generative AI Developer a nivel Professional está abierta para registro ahora mismo.

Pero les propongo pensarlas no por el nivel del examen sino como una ruta de conocimiento, y esa ruta depende de la carrera que cada uno quiera:

> **fundamentos → arquitectura y cloud → especialización → IA**

Alguien que quiera ser arquitecto y alguien que quiera trabajar en datos van a recorrer esa misma secuencia con contenidos distintos.

También existen las **microcredenciales**, que a mí me parecen especialmente interesantes para quien está empezando: se evalúan en un entorno real de AWS, no con preguntas de selección múltiple. Hay temas como serverless, agentic AI, redes de aplicaciones y respuesta a incidentes. Y no requieren suscripción a Skill Builder.

**PANTALLA** — Cuatro líneas, apareciendo una por una:
> La certificación no reemplaza la experiencia.
> El proyecto no reemplaza los fundamentos.
> La IA no reemplaza ninguna de las dos.
> **Las tres cosas se complementan.**

**GUION**

Pero el mensaje importante es este:

La certificación no reemplaza la experiencia.

El proyecto no reemplaza los fundamentos.

La IA no reemplaza ninguna de las dos.

**Las tres cosas se complementan.**

---
---

# CIERRE

**CONTROL DE RELOJ** · Este acto ocupa de **35:33** a **39:58** (4m 25s, 11% de la charla). Si al terminarlo tu reloj pasa de **41:28**, no pasa nada. Este bloque no se recorta ni se acelera nunca — es lo único que el público se lleva.

## 6.1 · Volver a la pregunta inicial

**TIEMPO** · 35:33 → 36:25 · 52s

**PANTALLA** — Exactamente la misma pantalla de 1.1, sin un pixel de diferencia: el contraste *3 horas / 30 segundos* y la pregunta grande. La repetición literal es el recurso; si la cambias, el público no la reconoce.

**GUION**

Al principio les pregunté algo.

Si una IA puede escribir en treinta segundos el código que a ustedes les tomó tres horas aprender a construir, ¿perdieron esas tres horas?

**NOTA** — Pausa. Que el público reconozca la pantalla.

La respuesta es no.

Porque el objetivo nunca fue aprender a escribir código.

**El objetivo era aprender a construir sistemas.**

---

## 6.2 · No compitas con la IA

**TIEMPO** · 36:25 → 37:29 · 1m 04s

**PANTALLA** — Una línea:
> No intenten ser la persona que escribe código más rápido que una IA.

**GUION**

Y de ahí sale el consejo más práctico que les puedo dar.

No intenten convertirse en la persona que escribe código más rápido que una IA. Esa carrera está perdida.

Conviértanse en la persona que sabe qué código debe existir. Qué arquitectura usar. Qué riesgos hay. Cómo verificar la solución. Cuándo la IA está equivocada. Y cómo llevar algo desde una idea hasta producción.

Porque la habilidad no es *usar IA*.

**La habilidad es hacer ingeniería con IA.**

---

## 6.3 · Tres ideas para llevarse a casa

**TIEMPO** · 37:29 → 38:48 · 1m 19s

**PANTALLA** — Tres bloques numerados, uno por uno.

**GUION**

Tres cosas, y con eso cierro.

**Primera.** Sí, vale la pena aprender a programar. Pero aprender a programar ya no puede significar únicamente aprender sintaxis.

**Segunda.** Usar inteligencia artificial va a ser parte normal del trabajo del ingeniero. La ventaja no está en ignorarla, y tampoco está simplemente en saber escribir prompts. Está en saber usarla con criterio de ingeniería.

**Tercera.** El código ya no será la parte más difícil de construir software. El problema, los requisitos, la arquitectura, la seguridad, la operación, el costo y las decisiones siguen siendo difíciles.

Y ahí sigue haciendo falta un ingeniero.

---

## 6.4 · Última frase

**TIEMPO** · 38:48 → 39:58 · 1m 10s

**PANTALLA** — Negro. Sin texto, hasta la pantalla final.

**GUION**

Quizás dentro de algunos años escribamos mucho menos código a mano.

Pero eso no significa que necesitemos menos ingeniería.

Probablemente necesitemos más.

Porque cuando cualquiera puede producir software, la diferencia entre producir código y construir un buen sistema se vuelve todavía más importante.

**NOTA** — Pausa. Última línea, más lento, mirando al público.

Así que no tengan miedo de que la inteligencia artificial aprenda a programar.

**Preocúpense por aprender ustedes a hacer ingeniería.**

**PANTALLA FINAL**

> # Don't compete with AI at writing code.
> # Learn to build what matters.
>
> **Ingeniería + Cloud + IA + criterio.**

---
---

# Anexo A · Fuentes verificadas

Todas verificadas el 13 de agosto de 2026. Los enlaces del guion v1 traían parámetros de rastreo (`utm_source=chatgpt.com`); están limpios aquí.

| Afirmación en el guion | Fuente |
|---|---|
| AWS Educate es gratuito, abierto a cualquier persona sin importar nivel educativo, sin tarjeta de crédito, desde los 13 años; laboratorios de S3, EC2, VPC, RDS y Cloud Operations; insignias digitales; bolsa de empleo para 18+ | [AWS Educate](https://aws.amazon.com/education/awseducate/) |
| Skill Builder: gratis los Practice Question Sets (20 preguntas), cursos Exam Prep de 2h y Cloud Quest. Suscripción individual desde 29 USD/mes para exámenes de práctica oficiales, labs y cursos extendidos de 6–8h | [AWS Certification exam preparation](https://aws.amazon.com/certification/certification-prep/) · [skillbuilder.aws](https://skillbuilder.aws/) |
| Kiro convierte prompts en requisitos, diseños arquitectónicos y tareas ordenadas; revisa los requisitos buscando contradicciones y vacíos antes de escribir código; IDE, CLI y web; capa gratuita; no requiere cuenta AWS | [kiro.dev](https://kiro.dev/) |
| Plan de estudiantes de Kiro: 1.000 créditos/mes gratis por un año, **solo para universidades elegibles** (lista actual: EE.UU. y Canadá). Formulario para solicitar inclusión de tu universidad | [kiro.dev/students](https://kiro.dev/students/) |
| Cuatro niveles de certificación (Foundational, Associate, Professional, Specialty); AWS Certified Generative AI Developer – Professional abierta para registro; microcredenciales evaluadas en entorno real de AWS con temas como serverless y agentic AI, sin necesidad de suscripción | [AWS Certification](https://aws.amazon.com/certification/) |

**Reemplazo de cita:** el guion v1 citaba el anuncio de lanzamiento de Kiro en AWS GovCloud como fuente de qué es Kiro. Es una fuente débil para esa afirmación — se reemplazó por el sitio del producto, que además aporta el detalle de la validación de contradicciones en los requisitos. También se retiró la referencia al post del blog de marzo de 2026 sobre laboratorios de Agentic AI: la afirmación equivalente ahora se apoya en la página de microcredenciales, que es contenido permanente y no un anuncio puntual.

---

# Anexo B · Bitácora de cambios frente al guion v1

**Reducción:** 10 actos → 5 actos + cierre. Sin pérdida de ideas únicas.

### Duplicados eliminados

| Qué estaba repetido | Dónde estaba | Qué se hizo |
|---|---|---|
| La lista de lo que la IA puede hacer (escribir código, pruebas, infra, documentar…) | Acto 0 y Acto I §2 "Cuarta etapa" | Se conserva una sola vez, en 0.2, donde tiene más fuerza dramática |
| La historia de las abstracciones | Acto 0 (transición), Acto I §2, Acto III §10 (analogía) | Consolidada en el Acto I (1.2 y 1.3). La analogía de la calculadora se movió aquí porque pertenece al contexto histórico, no a la respuesta |
| Kiro presentado desde cero | §12 y §17, ambos con la misma cita y el mismo contraste prompt → spec | Una sola presentación conceptual en 4.2; en 5.2 aparece solo como recurso accionable |
| "¿Vale la pena aprender a programar?" | §1, §9, §20, §21-Primera | Se pregunta en 1.1, se responde en 4.1, se cierra como bookend en 6.1 y queda como takeaway breve en 6.3 sin volver a explicarse |
| La ruta de 10 pasos vs. las 5 capas | §13 y §19 se solapaban casi por completo | Las capas responden *qué* aprender (4.3); los pasos responden *en qué orden* (5.1), reducidos de 10 a 7. Los pasos 7 y 8 del v1 (arquitectura, fundamentos de IA) ya estaban en las capas 2 y 4 |
| Cloud descrito dos veces | Capa 3 (§13) y paso 4 (§19) | Capa 3 conserva el temario; el paso 4 conserva la acción ("desplegar") |
| AWS Educate y certification-prep citados dos veces cada uno | §15/§19 y §16/§18 | Una cita por afirmación, todas en el Anexo A |
| "No compitas con la IA" | Acto VI §14 y pantalla final | Fundido en el cierre (6.2), donde el mensaje remata en lugar de anticiparse |

### Reordenamientos

- **La analogía de la calculadora subió** del Acto III al Acto I. Antes llegaba después de la respuesta; ahora prepara el terreno para ella.
- **"El código se volvió barato" ahora cierra el Acto I** en lugar de abrir el II. Es la conclusión de la historia de las abstracciones, no una premisa nueva.
- **La provocación de las tres horas se movió al inicio del Acto I** y se cierra explícitamente en 6.1. Antes se abría y nunca se marcaba el retorno.
- **Vibe coding y la paradoja de la IA quedaron juntos** en un solo acto (III). Antes estaban separados por la sección de "qué quieren las empresas", que rompía la tensión.
- **Las 7 preguntas del roadmap se redujeron a 5** y ahora corresponden exactamente, una a una y en orden, a los actos I a V. (Las dos que salieron — "qué buscan las empresas" y "cómo prepararnos" — no se perdieron: son los actos II y V.)
- **"De programador a ingeniero aumentado" (§11 del v1) bajó al Acto II**, como 2.3. En el v1 estaba en un acto propio, después de la respuesta sobre si vale la pena programar; ahora cierra la argumentación sobre qué cambió en el trabajo y prepara directamente el spec-driven del Acto IV. Su remate — *"demuestra que cumple con ellas"* — quedó marcado como la bisagra de la charla.

### Verificación de cobertura

Se comparó el v2 contra el v1 sección por sección. Se detectaron siete pérdidas de contenido único y las siete se restauraron: la progresión Ayer/Hoy/Mañana, el ingeniero como coordinador de agentes, la reformulación del encargo de trabajo ("demuestra que cumple"), "modifica repositorios completos" en 0.2, "comprender algoritmos" en 4.1, la pregunta "¿se va a acabar el trabajo para los programadores?" en 0.4, la ruta de conocimiento *fundamentos → arquitectura/cloud → especialización → IA* en 5.2, el marco de la *economía* de producir software en 1.4, y la aclaración de que la IA participa en todas las etapas del flujo spec-driven en 4.2.

### Correcciones de forma

- Jerarquía de encabezados arreglada: en el v1 los actos y sus secciones usaban ambos `#`, así que no había jerarquía real. Ahora `#` para actos, `##` para secciones numeradas.
- Numeración continua y consistente (`0.1`, `1.2`, `4.3`) en lugar de una serie global de 21 secciones desalineada de los actos.
- Notas de autor ("aquí introduciría", "una posible apertura") convertidas en guion hablado o en bloques `NOTA` explícitos.
- Párrafos de una línea agrupados donde la separación no aportaba ritmo de habla.

### Tema original

El hueco de 0.1 quedó lleno: la charla original iba a ser sobre **las microVMs detrás de AWS Lambda**.

En lugar de dejarlo como anécdota de apertura, se convirtió en un hilo de tres puntos:

1. **0.1** — se presenta con entusiasmo real (el giro solo funciona si el público cree que el tema valía la pena).
2. **1.2** — callback: Lambda es la abstracción; la microVM es el trabajo que la abstracción movió de lugar, no el que eliminó.
3. **4.3, Capa 1** — cierre del hilo: el ejemplo del arranque en frío demuestra por qué hay que entender la capa de abajo aunque no se escriba.

Si necesitas recortar tiempo, los puntos 2 y 3 son opcionales por separado — pero si eliminas uno, elimina los dos, o el hilo queda abierto.

### Pendiente

- Nada. El guion está completo.
