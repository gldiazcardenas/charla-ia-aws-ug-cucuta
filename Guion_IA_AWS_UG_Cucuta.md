# El futuro del desarrollo de software luego de la Inteligencia Artificial

### AWS User Group Cúcuta

## Idea central de la charla

> **La inteligencia artificial no está acabando con los ingenieros de software. Está acabando con una definición demasiado pequeña de lo que significa ser ingeniero de software.**

Durante muchos años asociamos el trabajo del programador con escribir código.

Hoy una máquina puede producir código en segundos.

Entonces aparece una pregunta incómoda:

**Si escribir código deja de ser nuestra principal ventaja competitiva, ¿cuál será nuestro valor?**

Toda la charla debería conducir hacia una respuesta:

**Nuestro valor estará cada vez menos en producir líneas de código y cada vez más en entender problemas, diseñar sistemas, tomar decisiones, evaluar alternativas y garantizar que lo que construimos realmente funcione.**

---



# ACTO 0 — ESTA NO ERA LA CHARLA QUE IBA A DAR

## 0. Romper el hielo: la historia detrás de esta charla

Quiero comenzar contándoles algo.

**Esta no era la charla que originalmente iba a dar.**

Cuando comenzamos a pensar en este evento, la idea inicial era hablar de [AQUÍ CUENTAS LA TEMÁTICA ORIGINAL].

Y tenía sentido.

Era un tema interesante, podíamos hablar de tecnología, mostrar algunas herramientas, probablemente hacer alguna demo y terminar con algunas recomendaciones.

Pero mientras preparábamos la charla apareció una pregunta.

Una pregunta mucho más incómoda.

> **¿Tiene sentido hablar solamente de nuevas tecnologías cuando está cambiando la manera misma en la que construimos tecnología?**

Porque algo extraño está pasando en nuestra industria.

---

## El momento en que cambia la pregunta

Durante años, quienes trabajamos en tecnología nos hemos acostumbrado al cambio.

Cada cierto tiempo aparece:

- un nuevo lenguaje;
- un nuevo framework;
- una nueva arquitectura;
- una nueva herramienta;
- una nueva plataforma cloud;
- una nueva forma de desplegar software.

Y normalmente nuestra reacción como ingenieros es bastante sencilla:

> “Bueno... toca aprenderlo.”

Aprendimos Git.

Aprendimos contenedores.

Aprendimos cloud.

Aprendimos CI/CD.

Aprendimos nuevos frameworks.

Y seguimos adelante.

Pero con inteligencia artificial empecé a pensar que estaba ocurriendo algo diferente.

Porque esta vez la nueva herramienta no solamente nos ayuda a hacer nuestro trabajo.

**La nueva herramienta puede hacer una parte del trabajo que durante años utilizamos para definir nuestra profesión.**

Puede escribir código.

Puede crear pruebas.

Puede explicar un repositorio.

Puede encontrar errores.

Puede crear infraestructura.

Puede proponer arquitecturas.

Puede documentar.

Puede tomar una tarea y comenzar a implementarla.

Entonces la pregunta dejó de ser:

> **“¿Qué nueva tecnología debería aprender un ingeniero?”**

Y pasó a ser:

> **“¿Qué significa ser ingeniero cuando una máquina también puede programar?”**

---

# Una conversación que probablemente todos hemos tenido

Seguramente muchos de los estudiantes que están aquí han pensado alguna vez:

> “¿Será que escogí la carrera correcta?”

O quizá:

> “Estoy aprendiendo Java/Python/JavaScript mientras ChatGPT, Claude, Kiro, Copilot y otras herramientas ya pueden generar todo esto.”

Y entonces aparece inevitablemente la pregunta:

> **¿Para qué estoy aprendiendo a programar?**

Pero esta pregunta no es solamente de los estudiantes.

Los que llevamos algunos años trabajando también tenemos nuestra propia versión:

> **¿Lo que sé hacer hoy seguirá siendo valioso dentro de cinco años?**

Y las empresas tienen otra:

> **¿Qué debería esperar ahora de un ingeniero de software si tiene inteligencia artificial disponible todo el tiempo?**

Son tres perspectivas diferentes sobre el mismo cambio.

---

# Ahí nació realmente esta charla

Entonces decidimos cambiar el tema.

Porque quizá lo más útil que podemos hacer hoy no sea enseñarles simplemente **otra herramienta**.

Quizá primero tenemos que entender:

**qué está pasando con nuestra profesión.**

Y por eso hoy quiero que conversemos sobre algunas preguntas que probablemente muchos tenemos:

- ¿Qué cambió realmente con la inteligencia artificial?
- ¿Qué están buscando ahora las empresas?
- ¿Se va a acabar el trabajo para los programadores?
- ¿Vale la pena aprender a programar?
- ¿Qué pasa cuando dejamos que la IA escriba software que nosotros mismos no entendemos?
- ¿Qué deberíamos aprender ahora?
- ¿Y cómo podemos prepararnos para lo que viene?

No pretendo tener una bola de cristal.

Pero sí podemos observar lo que está ocurriendo hoy y tratar de entender hacia dónde se está moviendo nuestra profesión.

---

# La transición al Acto I

Y para entender hacia dónde vamos...

primero tenemos que recordar **de dónde venimos**.

Porque hay algo importante que solemos olvidar:

**esta no es la primera vez que una tecnología hace que programar sea más fácil.**

De hecho, prácticamente toda la historia de nuestra industria consiste en eso.

Cada generación de ingenieros ha construido herramientas para que la siguiente tenga que hacer menos trabajo manual.

La diferencia es que esta vez...

**la abstracción está empezando a escribir el código por nosotros.**

---

# ACTO I — EL MUNDO CAMBIÓ

## 1. Abrir con una provocación

Una posible apertura:

> Quiero comenzar con una pregunta para los estudiantes que están aquí.
>
> ¿Cuántos están aprendiendo actualmente Java, Python, JavaScript, C#, Go o algún otro lenguaje?
>
> Ahora imaginen que mañana aparece una herramienta capaz de escribir en 30 segundos el código que ustedes tardaron tres horas en aprender a construir.
>
> ¿Perdieron esas tres horas?
>
> ¿O estaban aprendiendo algo mucho más importante que simplemente escribir código?

Pausa.

> Esa es probablemente una de las preguntas más importantes para cualquier persona que esté estudiando ingeniería de sistemas en este momento.

Y ahí introduces el problema:

**La IA cambió radicalmente la economía de producir software.**

---

# 2. ¿De dónde venimos?

Contar rápidamente la evolución.

### Primera etapa: programar era hablar con la máquina

El desarrollador debía conocer profundamente:

- memoria;
- estructuras de datos;
- sistemas operativos;
- compiladores;
- lenguajes;
- infraestructura.

Construir software era costoso.

El código era escaso.

---

### Segunda etapa: aparecen las abstracciones

Llegaron:

- frameworks;
- bibliotecas;
- cloud computing;
- servicios administrados;
- APIs;
- Infrastructure as Code;
- CI/CD;
- contenedores.

Cada generación permitió hacer más con menos esfuerzo.

Antes alguien configuraba servidores físicamente.

Después escribíamos scripts.

Después aparecieron Terraform, CloudFormation, CDK.

Después aparecieron plataformas administradas.

**La industria siempre ha avanzado eliminando trabajo manual.**

---

### Tercera etapa: Stack Overflow, Google y GitHub

El desarrollador dejó de memorizar todo.

Aprendimos a buscar.

Una habilidad fundamental pasó a ser:

> **Saber encontrar la respuesta correcta.**

---

### Cuarta etapa: IA generativa

Ahora sucede algo diferente.

Ya no solamente buscamos la respuesta.

Podemos decir:

> Construye esta funcionalidad.

Y la máquina:

- propone una arquitectura;
- escribe código;
- genera pruebas;
- documenta;
- encuentra errores;
- crea infraestructura;
- modifica repositorios completos.

Por primera vez estamos automatizando parcialmente **la producción del código mismo**.

Ahí está el verdadero cambio.

---

# 3. Lo que se volvió barato

Hay una frase que puede convertirse en uno de los mensajes principales:

> **El código se está volviendo barato. El criterio sigue siendo caro.**

Generar 300 líneas de código puede tomar segundos.

Pero siguen siendo difíciles preguntas como:

- ¿Son las 300 líneas correctas?
- ¿Resuelven el problema?
- ¿Son seguras?
- ¿Escalan?
- ¿Cuánto costarán en producción?
- ¿Qué ocurrirá cuando falle un servicio?
- ¿Estamos almacenando correctamente los datos?
- ¿Cumplimos con privacidad y regulación?
- ¿Es esta realmente la arquitectura que necesitamos?

La IA puede producir una respuesta.

**El ingeniero sigue siendo responsable de determinar si es una buena respuesta.**

Transición:

> Y esto cambia completamente lo que las empresas deberían esperar de nosotros.

---

# ACTO II — EL NUEVO INGENIERO

## 4. ¿Qué quieren ahora las empresas?

Durante muchos años una entrevista podía estar dominada por preguntas como:

- ¿Conoces Java?
- ¿Sabes React?
- ¿Has trabajado con Spring?
- ¿Sabes hacer una API REST?

Eso sigue teniendo valor.

Pero cada vez es menos suficiente.

La empresa no contrata realmente a alguien porque sabe escribir Java.

La empresa tiene:

- clientes;
- procesos;
- restricciones;
- riesgos;
- dinero;
- infraestructura;
- datos;
- problemas.

Y necesita personas capaces de transformar todo eso en sistemas confiables.

Por eso el perfil valioso se está moviendo de:

> **“Sé programar en X.”**

hacia:

> **“Sé resolver problemas utilizando software.”**

---

# 5. La nueva unidad de productividad

Antes podíamos pensar:

**Problema → desarrollador → código**

Ahora tenemos:

**Problema → ingeniero → IA/agentes/herramientas → software**

Esto significa que una persona puede producir mucho más.

Pero también significa algo importante:

> **Una mala decisión también puede producirse muchísimo más rápido.**

Con IA podemos acelerar buenas decisiones.

Pero también podemos acelerar:

- deuda técnica;
- vulnerabilidades;
- arquitecturas deficientes;
- código innecesario;
- complejidad;
- costos cloud;
- errores.

La velocidad no reemplaza al conocimiento.

**La velocidad multiplica aquello que ya sabemos hacer.**

---

# 6. Vibe coding

Aquí introduciría el concepto de forma equilibrada.

Vibe coding puede ser extraordinariamente útil.

Una persona describe lo que quiere, la IA genera algo, lo prueba superficialmente y continúa iterando:

> “Haz que este botón funcione.”

> “Ahora agrega autenticación.”

> “Ahora conecta una base de datos.”

> “Corrige este error.”

Y rápidamente tenemos una aplicación funcionando.

Para:

- prototipos;
- experimentos;
- hackathons;
- aprendizaje;
- validación de ideas;

esto puede ser increíble.

El problema comienza cuando confundimos:

> **“Funciona en mi computador.”**

con:

> **“Está listo para producción.”**

---

# 7. La trampa del vibe coding

Imaginemos que le pedimos a una IA crear una aplicación.

Después de veinte prompts tenemos:

- frontend;
- backend;
- login;
- base de datos;
- API;
- despliegue.

Todo parece funcionar.

Entonces alguien pregunta:

**¿Cómo funciona la autenticación?**

No sabemos.

**¿Por qué elegimos esta base de datos?**

No sabemos.

**¿Qué sucede si tenemos diez mil usuarios concurrentes?**

No sabemos.

**¿Dónde están almacenados los secretos?**

No sabemos.

**¿Cuánto cuesta operar esto?**

No sabemos.

Y aparece el problema fundamental:

> **Somos propietarios de un sistema que no entendemos.**

Ese es uno de los riesgos más importantes de desarrollar software solamente mediante prompts.

---

# 8. La paradoja de la IA

Aquí introduciría una de las ideas más fuertes de la conferencia:

> **Mientras más código pueda escribir la IA, más importantes se vuelven los fundamentos de ingeniería.**

¿Por qué?

Porque alguien tiene que reconocer cuando la IA propone algo incorrecto.

Para detectar una mala arquitectura necesitas conocer arquitectura.

Para detectar una vulnerabilidad necesitas conocer seguridad.

Para detectar una consulta ineficiente necesitas entender bases de datos.

Para evaluar código concurrente necesitas comprender concurrencia.

Para diseñar un sistema distribuido necesitas comprender sistemas distribuidos.

La IA puede reducir la necesidad de recordar sintaxis.

Pero puede aumentar la necesidad de **comprender conceptos**.

---

# ACTO III — ¿ENTONCES TODAVÍA VALE LA PENA APRENDER A PROGRAMAR?

## 9. La pregunta que muchos estudiantes realmente tienen

> ¿Vale la pena pasar años aprendiendo programación si una IA puede escribir código?

**Sí.**

Pero tenemos que ser mucho más precisos sobre qué significa aprender programación.

Aprender programación no consiste solamente en recordar cómo escribir:

```text
for
if
while
class
function
```

Programar enseña a:

- dividir problemas grandes en problemas pequeños;
- construir abstracciones;
- modelar información;
- pensar en estados;
- manejar errores;
- comprender algoritmos;
- razonar sobre eficiencia;
- diseñar interfaces;
- depurar sistemas;
- pensar sistemáticamente.

Eso sigue teniendo muchísimo valor.

---

# 10. Una analogía

Las calculadoras no hicieron innecesario aprender matemáticas.

Hicieron innecesario realizar manualmente ciertos cálculos.

Las hojas de cálculo no eliminaron a los financieros.

Los hicieron capaces de trabajar con problemas más grandes.

Los compiladores no eliminaron a los programadores porque ya no escribíamos ensamblador.

Los lenguajes de alto nivel tampoco.

Cloud no eliminó a los ingenieros porque ya no instalábamos físicamente servidores.

**La abstracción mueve el nivel en el que resolvemos los problemas.**

La IA está haciendo exactamente eso.

Nos está obligando a subir un nivel.

---

# ACTO IV — ¿QUÉ SERÁ DEL INGENIERO DE SISTEMAS?

## 11. De programador a ingeniero aumentado

Una posible evolución:

### Ayer

El desarrollador escribía gran parte del código manualmente.

### Hoy

El desarrollador escribe código junto con asistentes de IA.

### Mañana

El ingeniero probablemente coordinará múltiples agentes y herramientas capaces de:

- implementar funcionalidades;
- escribir pruebas;
- revisar código;
- desplegar infraestructura;
- analizar vulnerabilidades;
- generar documentación;
- investigar incidentes.

El trabajo se parecerá progresivamente menos a:

> “escribe esta función”.

Y más a:

> “este es el sistema que necesitamos; estas son sus restricciones; estas son las condiciones bajo las cuales debe funcionar; demuestra que cumple con ellas.”

---

# 12. Del código a la especificación

Esto permite introducir Kiro de manera natural.

Hay algo particularmente interesante:

Si la IA es capaz de escribir código, entonces una de las habilidades más importantes pasa a ser **explicar con precisión qué queremos construir**.

Eso nos lleva de:

**prompt-driven development**

a:

**spec-driven development.**

No decir simplemente:

> “Créame una aplicación para reservas.”

Sino definir:

- qué problema resuelve;
- cuáles son sus requisitos;
- cuáles son sus restricciones;
- qué comportamientos esperamos;
- cuáles son sus criterios de aceptación;
- cómo debería probarse.

Este enfoque conecta directamente con herramientas modernas como **Kiro**, que AWS describe como un entorno de desarrollo con IA orientado precisamente a pasar de prompts a especificaciones, código, documentación y pruebas. ([Amazon Web Services, Inc.](https://aws.amazon.com/about-aws/whats-new/2026/02/kiro-launch-aws-govcloud-us/?utm_source=chatgpt.com))

---

# ACTO V — LAS HABILIDADES QUE SOBREVIVEN A LA IA

## 13. ¿Qué debería aprender hoy un estudiante?

Yo lo agruparía en cinco capas.

### Capa 1 — Fundamentos

No abandonen:

- programación;
- estructuras de datos;
- algoritmos;
- bases de datos;
- redes;
- sistemas operativos;
- concurrencia;
- Git.

No porque necesariamente vayamos a escribirlo todo manualmente.

Sino porque necesitamos saber **qué está haciendo la máquina por nosotros**.

---

### Capa 2 — Ingeniería de software

Aprender:

- diseño de software;
- testing;
- patrones;
- APIs;
- observabilidad;
- seguridad;
- mantenibilidad;
- refactoring;
- documentación;
- arquitectura.

Cuando generar código es barato, distinguir **buen software de software que simplemente funciona** se vuelve mucho más importante.

---

### Capa 3 — Cloud

Un ingeniero moderno debería comprender:

- cómputo;
- redes;
- almacenamiento;
- bases de datos;
- identidad;
- seguridad;
- serverless;
- observabilidad;
- infraestructura como código.

Porque escribir una aplicación es solamente una parte del problema.

La aplicación después tiene que existir en el mundo real.

---

### Capa 4 — Inteligencia artificial

No necesariamente todos deben convertirse en investigadores de machine learning.

Pero sí deberían comprender:

- modelos fundacionales;
- contexto;
- tokens;
- embeddings;
- RAG;
- agentes;
- tool use;
- MCP;
- evaluación;
- seguridad de aplicaciones con IA;
- costos y límites de los modelos.

La IA debe convertirse en parte normal del toolbox del ingeniero.

---

### Capa 5 — Habilidades humanas

Aquí posiblemente esté una de las ventajas competitivas más grandes:

- pensamiento crítico;
- comunicación;
- entendimiento del negocio;
- capacidad de hacer buenas preguntas;
- capacidad de trabajar con ambigüedad;
- criterio técnico;
- liderazgo;
- responsabilidad.

Porque una IA puede producir veinte alternativas.

**Alguien todavía tiene que escoger una.**

---

# ACTO VI — CÓMO APRENDER EN ESTE NUEVO MUNDO

## 14. No competir contra la IA

Un mensaje importante para los estudiantes:

> No intenten convertirse en la persona que escribe código más rápido que una IA.

Esa carrera probablemente está perdida.

Conviértanse en la persona que sabe:

- qué código debe existir;
- qué arquitectura utilizar;
- qué riesgos hay;
- cómo verificar la solución;
- cuándo la IA está equivocada;
- cómo llevar algo desde una idea hasta producción.

La habilidad no es simplemente **usar IA**.

La habilidad es:

> **hacer ingeniería con IA.**

---

# ACTO VII — EL ECOSISTEMA AWS COMO RUTA DE APRENDIZAJE

Aquí la charla deja de ser conceptual y pasa a ser accionable.

## 15. AWS Educate — empezar

Para estudiantes que todavía están construyendo bases, AWS Educate puede ser una excelente puerta de entrada.

Actualmente AWS lo presenta como una plataforma gratuita y abierta a personas independientemente de su nivel educativo o experiencia, con rutas para aprender cloud e IA y ejercicios prácticos sobre servicios como Amazon S3 y EC2. ([Amazon Web Services, Inc.](https://aws.amazon.com/education/awseducate/?nc2=h_ql_exm_edu&utm_source=chatgpt.com))

Mensaje:

> No necesitan esperar a conseguir su primer empleo para empezar a trabajar con tecnologías cloud.

---

# 16. AWS Skill Builder — aprender sistemáticamente

Después está **AWS Skill Builder**.

Aquí pueden avanzar hacia rutas estructuradas de aprendizaje sobre:

- cloud;
- arquitectura;
- seguridad;
- datos;
- inteligencia artificial;
- preparación para certificaciones.

AWS ofrece contenido gratuito de preparación, incluidos cursos de Exam Prep y sets oficiales de preguntas; las suscripciones agregan recursos como laboratorios y exámenes de práctica completos. ([Amazon Web Services, Inc.](https://aws.amazon.com/certification/certification-prep/?utm_source=chatgpt.com))

Además, AWS continúa incorporando contenido específicamente relacionado con IA generativa y sistemas agentic. En 2026, por ejemplo, Skill Builder incorporó laboratorios de Agentic AI y rutas asociadas a nuevas certificaciones de IA generativa. ([Amazon Web Services, Inc.](https://aws.amazon.com/blogs/training-and-certification/march-2026-new-offerings/?utm_source=chatgpt.com))

---

# 17. Kiro — aprender a desarrollar con IA de otra manera

Después pueden experimentar con **Kiro**.

El mensaje aquí no debería ser simplemente:

> “Aquí hay otro editor que escribe código con IA.”

La idea interesante es otra.

Kiro introduce un flujo orientado a especificaciones.

En vez de:

**Prompt → código → prompt → más código**

podemos movernos hacia algo como:

**Idea → requisitos → diseño → tareas → implementación → pruebas**

con IA participando durante todo el proceso.

AWS posiciona Kiro precisamente como una herramienta para llevar proyectos desde prototipos hacia producción usando desarrollo basado en especificaciones, generando y manteniendo código, documentación y tests. ([Amazon Web Services, Inc.](https://aws.amazon.com/about-aws/whats-new/2026/02/kiro-launch-aws-govcloud-us/?utm_source=chatgpt.com))

Y eso conecta con todo lo que discutimos anteriormente:

> **La IA no elimina la ingeniería. Puede ayudarnos a hacerla más explícita.**

---

# 18. AWS Certifications — demostrar fundamentos

Luego aparecen las certificaciones.

Aquí evitaría venderlas como:

> “Consigue este certificado y tendrás trabajo.”

Presentaría una certificación como:

**una estructura para aprender + una forma de validar conocimiento.**

Una persona podría construir progresivamente conocimientos de:

**fundamentos → arquitectura/cloud → especialización → IA**

dependiendo de su carrera.

AWS mantiene rutas oficiales de preparación mediante Skill Builder y actualmente también cuenta con formación y certificaciones vinculadas específicamente con IA generativa. ([Amazon Web Services, Inc.](https://aws.amazon.com/certification/certification-prep/?utm_source=chatgpt.com))

El mensaje importante:

> La certificación no reemplaza la experiencia.
>
> El proyecto no reemplaza los fundamentos.
>
> La IA no reemplaza ninguna de las dos.
>
> **Las tres cosas se complementan.**

---

# ACTO VIII — UNA RUTA CONCRETA PARA LOS ESTUDIANTES

## 19. Si hoy estuviera comenzando ingeniería...

Yo propondría al público esta ruta:

### 1. Aprendería a programar.

Un lenguaje suficientemente bien.

Python, Java, JavaScript, C#, Go...

El lenguaje concreto importa menos que aprender correctamente los fundamentos.

### 2. Aprendería Git.

Porque el software real se construye colaborativamente.

### 3. Construiría proyectos.

No veinte tutoriales.

Dos o tres sistemas que realmente pueda explicar.

### 4. Aprendería cloud.

Desplegaría esos sistemas.

Configurar infraestructura.

Base de datos.

Logs.

Seguridad.

Monitoreo.

### 5. Utilizaría IA desde el principio.

Pero preguntándome siempre:

> ¿Entiendo lo que acaba de generar?

### 6. Aprendería a escribir especificaciones.

No solamente prompts.

### 7. Estudiaría arquitectura y system design.

Porque allí se están desplazando muchas de las decisiones más valiosas.

### 8. Aprendería fundamentos de IA generativa.

Para entender las herramientas con las que voy a trabajar.

### 9. Utilizaría rutas como AWS Educate y AWS Skill Builder.

Para estructurar el aprendizaje. ([Amazon Web Services, Inc.](https://aws.amazon.com/education/awseducate/?nc2=h_ql_exm_edu&utm_source=chatgpt.com))

### 10. Construiría evidencia de que sé hacer cosas.

GitHub.

Proyectos.

Arquitecturas.

Experimentos.

Contribuciones.

Certificaciones.

Experiencia.

---

# ACTO IX — EL MENSAJE FINAL

## 20. Volver a la pregunta inicial

Al principio preguntamos:

> Si una IA puede escribir en segundos el código que tardamos horas en aprender, ¿perdimos nuestro tiempo aprendiendo programación?

La respuesta es no.

Porque el objetivo nunca debió ser solamente aprender a escribir código.

El objetivo era aprender a construir sistemas.

---

## 21. Tres ideas para llevarse a casa

### Primera

**Sí, vale la pena aprender a programar.**

Pero aprender programación ya no puede significar únicamente aprender sintaxis.

---

### Segunda

**Usar inteligencia artificial será parte normal del trabajo del ingeniero.**

La ventaja no estará en ignorarla.

Tampoco estará simplemente en saber escribir prompts.

Estará en saber utilizarla con criterio de ingeniería.

---

### Tercera

**El código ya no será necesariamente la parte más difícil de construir software.**

El problema, los requisitos, la arquitectura, la seguridad, la operación, el costo y las decisiones seguirán siendo difíciles.

Y allí seguirá haciendo falta un ingeniero.

---

# CIERRE

Una posible última frase:

> Quizás dentro de algunos años escribamos mucho menos código manualmente.
>
> Pero eso no significa que necesitaremos menos ingeniería.
>
> Probablemente necesitaremos más.
>
> Porque cuando cualquiera puede producir software, la diferencia entre simplemente producir código y construir un buen sistema se vuelve todavía más importante.
>
> Así que no tengan miedo de que la inteligencia artificial aprenda a programar.
>
> **Preocúpense por aprender ustedes a hacer ingeniería.**

Pantalla final:

# Don't compete with AI at writing code.
# Learn to build what matters.

**Ingeniería + Cloud + IA + criterio.**