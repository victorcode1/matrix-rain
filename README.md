# Matrix Rain

Un tema oscuro verde para T3 Code, con lluvia digital detrás del chat y paneles que mantienen legibles las conversaciones. La escena funciona sin conexión, reacciona al puntero y respeta la opción de reducir movimiento.

## Instalación

La escena animada requiere [mi rama `feat/theme-scene` de T3 Code](https://github.com/victorcode1/t3code/tree/feat/theme-scene). En la versión oficial se aplican los colores, pero no la escena.

```sh
git clone https://github.com/victorcode1/matrix-rain.git
cd matrix-rain
t3 theme set ./matrix-rain.json --id matrix-rain
cp matrix-rain.html ~/.t3/userdata/themes/
```

Activa el modo oscuro. Si usas `--base-dir`, añade esa misma opción al comando `t3` y copia el HTML a `<carpeta>/userdata/themes/`. Para instalar únicamente los colores, importa el JSON desde Ajustes → Apariencia → Añadir tema.

La escena se ejecuta en un marco aislado y recibe la posición del puntero. Una versión compilada de una rama alternativa requiere revisar su código y mantenerla actualizada; instala temas de fuentes de confianza.

## Desarrollo

Edita `src/colors.json`, `src/theme.css` y `src/scene.html`; después ejecuta `npm run build` para generar los archivos instalables y `npm run check` para validar contraste y sincronización.

## Licencia

MIT. Proyecto independiente de T3 Code.
