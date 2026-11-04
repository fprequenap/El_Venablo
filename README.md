# El Venablo

**Las pruebas del oficio de caballero, según el *Libro de la Orden de Caballería* de Ramon Llull.**

© 2026 Francisco de Paula Requena Paredes · A.M.D.G.

> «Correr a caballo bien guarnecido, blandir la lanza en las lizas, andar con armas, los torneos, las tablas redondas, la esgrima, cazar ciervos, osos, jabalíes y leones, y otros ejercicios semejantes, pertenecen al oficio de caballero, pues con ellos se habitúa a los hechos de armas y al sostén de la Orden.» (II, §10)

Juego para móvil dirigido a adolescentes y jóvenes. El jugador empieza de escudero y va superando las pruebas del oficio. Cada prueba se mide por dos ejes, como en el Código: **destreza** y **virtud**. Ninguna prueba se supera sin las dos.

> «Así como todos esos ejercicios pertenecen al caballero en cuanto al cuerpo, le tocan en cuanto al alma la justicia, la sabiduría, la caridad, la lealtad, la verdad, la humildad, la fortaleza, la esperanza, la cautela y otras virtudes semejantes.» (II, §11)

**Versión actual: 0.12, de valoración.** Todas las pruebas están abiertas y no hay límite diario de jornadas.

---

## Cómo jugar

- **iPhone, Android u ordenador:** abre la página de este repositorio en GitHub Pages con el navegador. En el iPhone, desde Safari, usa **Compartir › Añadir a pantalla de inicio** para que quede como una app.
- **Android, instalado:** abre el archivo `El_Venablo_*.apk` y permite instalar apps de origen desconocido.

---

## Las pruebas

### Escudero

**El venablo: el jabalí.** Tres jabalíes por jornada.
- **El acecho:** toca donde quieras clavar el venablo, tensa y suelta cuando la barra marque «¡ahora!». Cuenta con el viento y con el paso del animal. Al codillo vale el doble.
- **La carga:** mantén pulsado para afirmar el venablo y apunta la punta a su pecho. La cruceta lo detiene a un palmo. Si sueltas, flaqueas.

**El ciervo: arco y misericordia.** Tres ciervos por jornada, con tres flechas cada uno.
- **El tiro:** el ciervo camina, se para, pasta y vigila. Se tira cuando está parado y con la cabeza baja. Si tiras mientras vigila, te oye y salta. La mira se pone roja sobre el codillo.
- **Codillo o vientre:** al codillo cae enseguida. Al vientre huye herido y hay que pararlo con otra flecha. Dejarlo escapar herido es falta.
- **El remate:** en tierra todavía respira y patea. Hay que esperar a que se calme y rematarlo con la misericordia en la nuca, como la puntilla. Dejarlo agonizar es falta.

### Caballero

**El oso: lanza o espada.** Dos osos por jornada. El segundo es más fuerte, para más golpes y amaga la zarpa para embestir.
- **El arma:** antes de cada oso se elige lanza o espada.
- **La lanza:** toca para la lanzada. Mantén pulsado para afirmarla, y si el oso embiste se clava él solo. La lanza puede quebrarse, y entonces se sigue con la espada.
- **La espada:** toca para el tajo a la cabeza. Mantén y suelta para la estocada.
- **Escudo y Atrás:** mantén el escudo para parar cualquier ataque. Atrás sirve para esquivar.
- **Golpes decisivos:** con el círculo rojo, cuando el oso se alza, la estocada o la lanzada al corazón lo mata en el acto. Con el oso malherido y descubierto, el tajo le parte la cabeza.
- **La misericordia:** si cae malherido, se remata con el puñal (V, §10). Dejarlo agonizar es falta.
- **Aguante:** atacar, esquivar y cubrirse cansan, y esperar en guardia lo recupera.

### Pendientes

Correr a caballo, la esgrima, la justa en las lizas, el torneo, las tablas redondas y el león.

---

## La virtud

Tras cada pieza llega una prueba de virtud: una decisión con su consecuencia y la cita literal del Libro. Una sola falta impide superar la jornada.

| Prueba | Virtudes y vicios | Citas |
|---|---|---|
| Venablo | Caridad, humildad, templanza en el ardimiento, devoción, bien común, contra la envidia | II §19 · III §19 · VI §16 · VI §17 · VI §20 · VI §14 |
| Ciervo | Verdad, justicia, templanza, contra la acidia, humildad, contra la ira | V §3 · II §9 · VI §16 · VI §12 · III §19 · VI §15 |
| Oso | Contra la ira, defensa de los labradores, contra la avaricia, prudencia, contra la acidia, piedad | VI §15 · II §22 · VI §11 · VI §7 · VI §12 · II §20 |

Si la destreza alcanza el mínimo pero hay falta de virtud, el juego responde con la Parte II, §11: diestro, pero no digno.

## Reglas de la jornada

- **Destreza mínima:** 150 en el venablo, 130 en el ciervo y 150 en el oso.
- **Sin falta de virtud y sin caer malherido:** tres heridas terminan la jornada.
- **Para ganar cada prueba,** hay que superar tres jornadas.
- **Templanza:** la versión definitiva limitará el juego a cinco jornadas al día; la de valoración no tiene límite.
- **Sin pagos ni anuncios.** El enganche está en la maestría, no en la compulsión.

## Dar tu opinión

El botón **Dar mi opinión**, en la portada y al final de cada jornada, abre un correo con cuatro preguntas y un resumen de la última jornada. Las opiniones llegan a **fprequenap@gmail.com**.

---

## Archivos de este repositorio

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La página del juego |
| `index.js` | Arranque del motor |
| `index.wasm.1`, `index.wasm.2` | El motor del juego, partido en dos trozos de menos de 25 MB; la página los vuelve a unir al cargar |
| `index.pck` | El juego: dibujo, lógica, textos y citas |
| `index.audio.worklet.js`, `index.audio.position.worklet.js` | Sonido |
| `index.png`, `index.icon.png`, `index.apple-touch-icon.png` | Pantalla de carga e iconos |

Para actualizar el juego, se suben los archivos nuevos encima de los anteriores.

## Técnica

- **Motor:** Godot 4.7.2, renderizador de compatibilidad, exportación web sin hilos para que funcione en Safari.
- **Arte y sonido:** dibujados y sintetizados por el propio programa. No hay imágenes ni grabaciones externas.
- **Datos guardados:** se guardan en el dispositivo y no se envían a ningún sitio.
- **El APK de Android:** se firma con una clave propia, que debe guardarse para poder publicar actualizaciones.

---

## Créditos

El juego nace de la edición impresa del **Libro de la Orden de Caballería** de Ramon Llull: edición bilingüe lemosín-español, con traducción, advertencia y edición de Francisco de Paula Requena Paredes (primera edición, 2026). Todas las citas del juego proceden de esa edición.

El fin de la Orden es el del Libro: que el caballero conozca, ame, sirva y adore a Dios, y por ese camino alcance la vida eterna.

> «Todo caballero debe conocer las siete virtudes, raíz y principio de todas las buenas costumbres y camino de la gloria celestial y perdurable.» (VI, §2)

Libro impreso: [https://amzn.eu/d/0c8yaSr1](https://amzn.eu/d/0c8yaSr1)

Aplicación compañera: *Código de Llull*, en [https://fprequenap.github.io/Llull/](https://fprequenap.github.io/Llull/)

## Derechos

El texto de Ramon Llull es de dominio público.

Son obra protegida, © 2026 Francisco de Paula Requena Paredes:
- la traducción al español contemporáneo y la edición del Libro;
- el juego: diseño, programa, dibujo y textos.

Reservados todos los derechos.

Tipografías UnifrakturMaguntia y EB Garamond, bajo licencia SIL Open Font License.

**AMDG**
