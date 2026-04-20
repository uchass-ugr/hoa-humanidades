# Ni de letras ni de ciencias: el maravilloso mundo de las Humanidades Computacionales

Materiales de una charla divulgativa de 60 minutos para alumnado de bachillerato.

## Autores

- Nicolás Robinson-García — [U^CHASS](https://uchass.ugr.es), Universidad de Granada
- Benamí Barros García — [U^CHASS](https://uchass.ugr.es), Universidad de Granada

## Cómo compilar

Este proyecto usa [bookdown](https://bookdown.org/). Desde R:

```r
install.packages(c("bookdown", "rmarkdown"))
bookdown::render_book("index.Rmd", "bookdown::gitbook")
```

O desde RStudio: abrir el proyecto y pulsar `Build Book`.

## Estructura

- `index.Rmd` — Portada y presentación del curso.
- `01-gancho.Rmd` — Apertura con el caso Elena Cañizares.
- `02-que-son-hc.Rmd` — ¿Qué son las Humanidades Computacionales?
- `03-bloque-textos.Rmd` — Bloque A · Minería de textos.
- `04-bloque-redes.Rmd` — Bloque B · Análisis de redes.
- `05-bloque-estilometria.Rmd` — Bloque C · Estilometría.
- `06-cierre.Rmd` — Cierre y salidas profesionales.
- `07-referencias.Rmd` — Referencias y recursos.
- `anexo-a-canciones.Rmd` — Anexo: análisis de letras de canciones.
- `anexo-b-guion-docente.Rmd` — Anexo: guion completo con tiempos.

## Licencia

CC BY-SA 4.0.