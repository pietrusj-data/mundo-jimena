# 🦄 El Mundo de Jimena

App de números y letras para una niña de infantil que **todavía no sabe leer**:
todo funciona por voz. Hecha por su padre para acompañarla en el aprendizaje a
distancia.

🌐 **https://pietrusj-data.github.io/mundo-jimena/**

Es una app personal, y a la vez el **laboratorio del motor de infantil** de
[PequeMisiones](https://github.com/pietrusj-data/pequemisiones).

## Qué hace

- **Todo se oye**: la portada desbloquea la voz del dispositivo y cada consigna se
  puede repetir con el botón 🔊. No hace falta leer nada.
- Números del 1 al 99: contar, buscar, series a saltos y cuenta atrás.
- **Amigos del 5, del 10 y del 20** en marco ABN, **familias** y **vecinos** de
  decena, tabla del 100.
- **Subitización** (¿cuántos ves de un vistazo?) y **palillos** para las decenas.
- **Sílabas** con grabadora ("la ele con la a suena *la*") y **trazado** de letras
  y números con rastro de arcoíris.
- **Misiones de papá** con su mensaje leído en voz alta.
- **Sin fallo posible**: a los dos errores, la respuesta buena parpadea y ella la
  toca; en los resultados aparece "la ayudó Nube 🌸", y puntúa igual.
- Estrellas, tesoros, fuegos artificiales en cada acierto y minijuegos de premio.

Principio que no se toca: en esta app **todo logro se celebra y nada se penaliza**.

## Notas técnicas

Un solo `index.html` (HTML, CSS y JS dentro), instalable como PWA, con Supabase
detrás y cola offline en `localStorage`.

El trazado usa canvas con `touch-action:none` y da por buena la letra al cubrir
≥78 % del recorrido; los trazos están en `LETRAS_TRAZO`.

Sin datos personales en el servidor.

Para trabajar en local: `python -m http.server 8795`.

## Licencia

Código propietario, ver [LICENSE](LICENSE). Público solo para que GitHub Pages
pueda servirlo.
