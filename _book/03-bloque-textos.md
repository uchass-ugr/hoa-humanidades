# Bloque A · Las palabras cuentan {#textos}

::: tiempo
15 minutos
:::

## Qué es la minería de textos

Cuando tenemos **muchos** textos, leerlos uno a uno es imposible. La minería de textos convierte el texto en datos: qué palabras aparecen, cuántas veces, en qué contextos, con qué otras palabras.

Es el motor silencioso detrás de: buscadores, traductores, filtros antispam, sistemas de recomendación, chatbots, y por supuesto, ChatGPT.

## Ejemplo 1 · Reseñas de La Casa de Papel

**Pregunta:** ¿Qué sienten los espectadores internacionales cuando hablan de la serie?

**Datos:** reseñas públicas en IMDb (≈ unos miles).

**Técnica:** nube de palabras con frecuencias.

**Qué aparece en pantalla:**

- Una nube de palabras tipo *wordcloud* clásica (llamativa pero mala para comparar).
- Luego la misma información como gráfico de barras (aburrida pero honesta).

**Mensaje didáctico:** la nube de palabras es *marketing* visual; el gráfico de barras es *análisis*. Conviene enseñar las dos.

> **Material reutilizable** de Wences: diapositivas 19–20.

## Ejemplo 2 · Subtítulos de YouTube

**Pregunta:** ¿Cómo habla un personaje público? ¿Qué palabras usa más? ¿Cuál es su tono dominante?

**Datos:** subtítulos automáticos descargados con `youtube-transcript-api` (Python) o `pytube`.

**Candidato sugerido:** un youtuber que el aula reconozca (Ibai, Illojuan, AuronPlay) frente a una figura política (Pedro Sánchez, Feijóo). Contraste evidente y didáctico.

**Qué analizamos:**

- Vocabulario más frecuente (sin *stopwords*).
- Muletillas.
- Análisis de sentimiento básico (positivo / negativo / neutro).

**Mensaje didáctico:** el lenguaje es un fingerprint. Quien habla elige palabras, incluso sin darse cuenta.

## Ejemplo 3 (opcional, si sobra tiempo) · Emoticonos y emojis

Una diapositiva sobre cómo un emoji es también un dato: se cuentan, se contextualizan, y cuentan una historia emocional que las palabras no capturan.

## Advertencia honesta: los horrores de la visualización

Dedicamos 60 segundos a recordar que **una visualización mal hecha miente mejor que cualquier texto**. Ejemplo clásico: elegir los colores de un mapa político a conveniencia hace que Madrid cambie de signo.

> **Material reutilizable** de Wences: diapositivas 22–25.

## Transición

> *"Hasta aquí hemos contado palabras. Pero las palabras no existen solas: están conectadas. Y sus hablantes también."*
