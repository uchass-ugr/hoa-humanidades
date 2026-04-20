# (APPENDIX) Anexos {-}

# Anexo A · Análisis de letras de canciones {#anexo-canciones}

::: tip
Este anexo **no forma parte de la charla de 60 minutos**. Se reserva como material de profundización para el alumnado interesado o para un taller más largo.
:::

## Pregunta de investigación

¿Cómo ha cambiado el vocabulario de un artista entre sus primeros discos y los más recientes?

**Candidatos interesantes** por tener discografía amplia y que los chavales reconocen:

- Bad Bunny (de *X 100PRE* a *Nadie Sabe Lo Que Va A Pasar Mañana*).
- Rosalía (de *Los Ángeles* a *Motomami*).
- Taylor Swift (de *Taylor Swift* a *Midnights*).
- C. Tangana (de *Avida Dollars* a *El Madrileño*).

## Pipeline de trabajo

### 1. Obtención de datos

Dos opciones principales:

- **Genius API** (vía el paquete `geniusr` de R) con un token gratuito.
- **Scraping directo** con `rvest` si la API da problemas.

### 2. Limpieza

```r
library(tidyverse)
library(tidytext)

# Ejemplo esquemático
letras |>
  unnest_tokens(palabra, letra) |>
  anti_join(stopwords_es) |>
  filter(str_length(palabra) > 2)
```

### 3. Análisis

- Palabras más frecuentes por disco.
- TF-IDF para detectar palabras características de cada álbum.
- Análisis de sentimiento con léxicos en español (`lexiconsp`, `iSAD`).
- Evolución temporal: ¿cambia la positividad/negatividad del artista a lo largo de los años?

### 4. Visualización

- Gráficos de barras por disco (no nubes de palabras, para no caer en el mismo error didáctico del bloque A).
- Mapa de calor de sentimiento a lo largo del tiempo.
- Diagrama de "palabras que desaparecen" y "palabras que aparecen" entre el primer y el último disco.

## Consideraciones legales

Las letras de canciones están protegidas por copyright. Los análisis agregados (frecuencias, vocabulario) se pueden publicar sin problema, pero **reproducir letras completas** no. Citar fragmentos bajo *fair use* en un contexto educativo es defendible.

## Para ir más allá

- Comparar discos **antes y después** de un hecho biográfico del artista.
- Redes de colaboraciones entre artistas usando los créditos de cada tema.
- Análisis de rimas (fonético) además de análisis de palabras (léxico).
