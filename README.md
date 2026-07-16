# Ciclo del Cielo 🌅

Fondo de pantalla animado e interactivo que simula el ciclo día/noche completo — amanecer, mediodía, atardecer y noche — construido solo con HTML, CSS y JS (sin video, sin imágenes).

🔗 **[Ver demo en vivo](https://yamidgt.github.io/Fondo-de-pantalla-ciclo-del-cielo/)**

## Archivos incluidos

- **`index.html`** — el wallpaper autocontenido (sin dependencias externas): cielo, aviones y hora/fase en la esquina. Sincronizada en vivo con la hora real del dispositivo. Optimizada para consumo mínimo de recursos.
- **`Minimalist and interactive sky cycle.zip`** — paquete listo para importar directamente en **Lively Wallpaper** (incluye el mismo `.html`, el `LivelyInfo.json` con los metadatos del wallpaper, y las capturas de preview). Es la forma más rápida de instalarlo si ya usas Lively: solo arrastra el `.zip` a la app o usa "Agregar wallpaper" → seleccionar archivo.

## Características

- **Cielo dinámico**: interpolación de color entre 11 fotogramas clave según la hora — transiciones suaves sin saltos.
- **Sol y luna**: se mueven en arco según la hora, con fade-in/fade-out en los bordes de su turno.
- **Estrellas**: campo de 60 puntos con parpadeo individual, visibles solo de noche.
- **Modo en vivo**: se sincroniza con la hora real del dispositivo cada 15s.
- **Aviones**: aparecen solos cada 25–60s; también se pueden lanzar tocando la pantalla o con una "resortera" (arrastra para apuntar, suelta para disparar — más estiras, más rápido vuela).

## Uso

Abre `index.html` en cualquier navegador — funciona offline, sin instalar nada.

Para usarlo como fondo de pantalla animado en Windows:

- **Lively Wallpaper**: importa directamente el `.zip` (recomendado, ya trae metadatos y preview), o carga `index.html` como "aplicación web".
- **[Wallpaper Engine](https://store.steampowered.com/app/431960/Wallpaper_Engine/)**: cárgalo como "aplicación web" apuntando a `index.html`.

## Cómo funciona

Un reloj interno (0–1440 minutos) controla todo el color y movimiento en cada fotograma: cielo interpolado, arcos de sol/luna, opacidad de estrellas, y trayectorias de aviones (lineales o balísticas, según el modo de lanzamiento). Nada es video ni imagen — todo se recalcula en tiempo real.

## Licencia

Uso personal libre.
