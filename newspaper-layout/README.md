Historias de usuario:

    Tu página debe contener un elemento main con la clase newspaper-layout.
    La .newspaper-layout debe incluir un header con la clase title que contenga un h1 para mostrar el nombre del periódico.
    La .newspaper-layout debe incluir un article con la clase feature-article para el artículo principal de noticias.
    El .feature-article debe incluir un elemento h2 para el título del artículo seguido de un elemento p para el contenido del artículo.
    Debes agregar tres elementos article más para artículos más pequeños, con las clases small-article1, small-article2 y small-article3.
    Cada uno de los artículos más pequeños debe incluir un elemento h3 para el título del artículo seguido de un elemento p para el contenido del artículo.

    La .newspaper-layout debe incluir un elemento article con la clase secondary-article para una sección adicional de noticias.
    El .secondary-article debe incluir un elemento h2 para el título del artículo seguido de un elemento p para el contenido del artículo.

    La .newspaper-layout debe incluir un figure con la clase cover-image para mostrar una imagen que represente el contenido del periódico.
    Los elementos con las clases title, feature-article, secondary-article, cover-image, small-article1, small-article2 y small-article3 deben tener una propiedad grid-area establecida con el mismo nombre de clase.
    Tu .newspaper-layout debe usar CSS Grid con una propiedad grid-template-areas para definir la disposición de las secciones:
        El .title debe abarcar toda la fila superior.
        La .feature-article debe abarcar dos columnas en la segunda fila, con la .cover-image en la tercera columna.
        La .secondary-article debe abarcar dos columnas en la tercera fila, con la .cover-image en la tercera columna.
        Los tres artículos pequeños deberían aparecer en la cuarta fila.
    La .newspaper-layout debe tener una propiedad grid-template-columns que divida el espacio en tres columnas iguales.
    Debes establecer la propiedad grid-template-rows de .newspaper-layout en auto para la primera fila y dividir el espacio restante en partes iguales para las otras filas.
    Debes agregar un espacio entre los elementos de la cuadrícula.
    Asegúrate de que la imagen dentro de .cover-image quepa en el espacio designado estableciendo su max-width en 100%.

Nota: Asegúrate de vincular tu hoja de estilos en tu HTML y aplica tu CSS.
