# Taller: Reconstrucción Semántica de una Página Web

## Página Utilizada
[Naruto Wiki (Fandom ES)](https://naruto.fandom.com/es/wiki/Naruto_Wiki)

## Identificación semántica

Para identificar la estructura semántica, realicé primero una inspección visual que me permitió distinguir los componentes principales, tales como la navegación (nav), el contenido central (main) y las distintas secciones. Posteriormente, intenté validar esta estructura con las herramientas de desarrollo del navegador; sin embargo, este proceso fue complicado ya que la falta de semántica en el código no es muy buena, por lo que la observación directa fue el método más eficaz para definir la nueva organización.

# Explicación de la Estructura Semántica: Naruto Wiki

### 1. `<header>`: La Identidad
Utilicé el `header` en la parte superior porque es el contenedor natural de la **identidad del sitio**. Aquí es donde vive el logo de Naruto y el título principal (`h1`). Al usar esta etiqueta, le indico al navegador: "Este es el encabezado global, lo primero que el usuario debe reconocer".

### 2. `<nav>`: El Mapa del Sitio
Para el menú de navegación con enlaces a la serie, manga y anime, usé `nav`. No es solo una lista de enlaces; es la **estructura principal de navegación**. Esto ayuda a los motores de búsqueda a indexar las secciones más importantes de la wiki de forma prioritaria.

### 3. `<main>`: El Corazón del Contenido
Encapsulé la bienvenida y la información principal dentro de `main`. Esto es vital para la accesibilidad, ya que le dice a los lectores de pantalla: "Ignora el resto por un momento, aquí empieza el **contenido único** de esta página".

### 4. `<section>`: Organización por Temas
Dividí el sitio en diferentes `section` (Contenido Destacado, Series, Sabías que...). La razón es que cada una representa un **bloque temático distinto**. Es como separar los capítulos de un libro; ayuda a que el código sea legible y organizado.

### 5. `<article>`: Piezas Independientes
Dentro de las secciones, usé `article` para elementos como la ficha de Kawaki o las noticias.
* **¿Por qué?** Porque un `article` representa contenido que tiene sentido por sí mismo. Si yo tomara ese bloque de Kawaki y lo pusiera en otra página, se seguiría entendiendo perfectamente sin necesidad del resto del sitio.

### 6. `<aside>`: Información Complementaria
Puse la barra lateral (Lo más reciente, Administración, Blogs) dentro de un `aside`. Esta etiqueta se usa para contenido que está **relacionado de forma indirecta**. Es información útil, pero no es el foco principal que el usuario busca leer de inmediato.

### 7. `<figure>` y `<figcaption>`: Semántica Visual
Para las imágenes de las aldeas y categorías, no usé solo `img`. Usé `figure` para agrupar la imagen y su título (`figcaption`). Esto crea una **relación explícita** entre la foto y el texto, algo que el HTML básico no logra por sí solo.

### 8. `<footer>`: El Cierre Profesional
Finalmente, el `footer` contiene los enlaces de Fandom y avisos legales. Es el lugar estándar donde los usuarios buscan información de contacto o enlaces corporativos una vez que terminan de leer.

### 9. `<strong>` y `<em>`: Énfasis con Significado
* Usé `<strong>` para nombres importantes (como **Amaterasu**), indicando que tienen **mucha importancia**.
* Usé `<em>` para términos en japonés o títulos (como *Kesshō*), indicando un **énfasis de lectura** o cambio de idioma.



He reestructurado el sitio eliminando elementos secundarios como redes sociales y comentarios para centrar la atención en el contenido real de la enciclopedia. Mi objetivo no fue recortar información, sino reorganizar cada parte utilizando una semántica más precisa; de esta manera, el sitio no solo es más limpio visualmente, sino que ahora es mucho más fácil de entender tanto para los usuarios como para los motores de búsqueda.
