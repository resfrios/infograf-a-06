# Infografía Interactiva: Top 5 Barreras del Estudiante Introvertido

## Descripción

Proyecto de diseño de información gráfica orientada a entornos educativos digitales. El objetivo es presentar un ranking de tipo "Top 5" sobre los principales obstáculos que enfrentan los estudiantes introvertidos en el aprendizaje colaborativo, transformando una lista de texto tradicional en una experiencia visual dinámica, atractiva y fácil de comprender.

## Tecnologías

El proyecto está desarrollado en un archivo único, sin dependencias externas ni procesos de compilación:

* HTML5: Estructura semántica (\<ul\>, \<li\>, \<header\>, \<main\>, \<footer\>) para garantizar accesibilidad y correcta interpretación por lectores de pantalla.  
* CSS3: Toda la presentación visual, layout y lógica de interacción.  
* Restricción estricta: No se utilizó JavaScript. Toda la interactividad se logra exclusivamente mediante selectores de estado (:hover) y pseudoelementos (::before, ::after).

## Características

* Interactividad sin JavaScript: Los elementos reaccionan al pasar el cursor del mouse sobre ellos, revelando información y activando animaciones de forma nativa con CSS.  
* Animación de íconos circulares: Cada viñeta utiliza un border-radius: 50% que inicialmente muestra solo la mitad de un fondo acento. Al hacer hover, la mitad oculta se revela mediante una animación de rotación 3D (rotateY con perspective).  
* Línea ondulada animada: Bajo cada título, un SVG codificado en base64 como background-image se anima desplazándose horizontalmente durante el estado hover.  
* Diseño Responsivo (Mobile First): Construido desde la versión móvil hacia el escritorio, utilizando @media (min-width) para adaptar espaciados, tipografía y proporciones en tres puntos de quiebre.  
* Accesibilidad: Respeta la preferencia del usuario por movimiento reducido mediante @media (prefers-reduced-motion: reduce), desactivando las transiciones cuando es necesario.

## Contenido

El contenido de la infografía está extraído y adaptado del artículo científico:

*Unveiling barriers of introverts to collaborative learning*  
DOI: [10.1186/s40359-025-03282-y](https://doi.org/10.1186/s40359-025-03282-y)

El Top 5 abordado es el siguiente:

1. Miedo al liderazgo y a la responsabilidad  
2. Dificultad para expresar ideas  
3. Problemas de comunicación en grupos  
4. Inseguridad y dudas en sí mismos  
5. Alto desgaste de energía al participar

## Proceso de construcción

1. Maquetación HTML: Se definió una lista semántica \<ul\> donde cada \<li\> actúa como una tarjeta de dos columnas (ícono a la izquierda, texto a la derecha) utilizando Flexbox.  
2. Diseño visual base: Se aplicó la paleta de colores oscura y elegante (\#1A1A2E, \#16213E, \#E94560) con tipografía *Poppins* para establecer un ritmo visual limpio y educativo.  
3. Integración de efectos CSS: Se construyó la lógica de los pseudoelementos para dividir el círculo en dos mitades controlables por separado, y se generó/dimensionó el SVG en base64 para lograr la curva precisa bajo los títulos.  
4. Responsive Testing: Se ajustaron los valores de gap, padding y font-size progresivamente para asegurar la legibilidad tanto en pantallas pequeñas como en monitores grandes.

## Autor

Dariana Cornejo Dávila

