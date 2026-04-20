# Bloque B · Todo está conectado {#redes}

::: tiempo
15 minutos
:::

## Qué es una red

Una **red** (o grafo) es simplemente un conjunto de cosas (nodos) conectadas entre sí (aristas).

- Personas y amistades → red social.
- Actores y películas → red de colaboración.
- Webs y enlaces → la World Wide Web.
- Aeropuertos y vuelos → red de transporte.

## Los seis grados de Kevin Bacon

**La idea:** cualquier actor de Hollywood está a menos de seis películas de distancia de Kevin Bacon. De un juego de bar salió una página web (*Oracle of Bacon*) y, años después, el mismo Kevin Bacon montó una ONG (*SixDegrees.org*) para "usar su red" para causas benéficas.

**Lo que mostramos:**

1. Grafo visual de Kevin Bacon con actores a distancia 1, 2, 3.
2. Misma idea aplicada a otros actores (El Rubius → Keanu Reeves en 3 saltos, diapo de Wences).
3. Stanley Milgram y el experimento original de 1967: seis grados de separación entre cualquier par de personas del planeta.
4. Edunov et al. (2016): Facebook midió la distancia real y le salió **3.57** grados. Internet nos acercó.

> **Material reutilizable** de Wences: diapositivas 5–9, 32–33.

## Aplicación a series: Stranger Things

**Pregunta:** ¿Qué personajes son el "centro" de la serie? ¿Hay grupos que casi no interactúan?

**Datos:** co-aparición de personajes por episodio. Se puede sacar de subtítulos (quién habla en qué escena) o de *fan wikis*.

**Técnica:** grafo con tamaño de nodo = número de apariciones; grosor de arista = número de interacciones.

**Qué veremos:**

- Eleven y Mike como nodos centrales.
- Comunidades claras: el grupo de los niños, el instituto, el grupo adulto (Hopper, Joyce), los nuevos personajes de cada temporada.
- Cómo cambia la red entre temporadas.

::: aviso
**Si no hay dataset de Stranger Things listo:** Wences ya tiene una red de Los Simpson perfectamente usable (diapositivas 28–29). Menos moderna, pero funciona y los chavales conocen la serie.
:::

## Aplicación a redes sociales reales

Cerrar el bloque volviendo al caso Elena Cañizares: quién retuitea a quién dibuja comunidades. De "mil usuarios retuitean a tres cuentas" salen los clústers: unos apoyan a Elena, otros a las compañeras de piso.

> **Material reutilizable** de Wences: diapositivas 34–40.

## Transición

> *"Hemos contado palabras y hemos trazado conexiones. Falta una pregunta muy literaria: ¿quién escribió esto?"*
