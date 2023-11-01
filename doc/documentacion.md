# Documentación de la Página Pecora Pizza

La página web de la pizzería está diseñada utilizando HTML y Bootstrap 5. Se han agregado algunos estilos personalizados utilizando CSS, principalmente para ajustes de color y efectos de hover en ciertos elementos.

Antes de adentrarnos en la análisis del código, es crucial destacar que la elección de utilizar únicamente HTML y Bootstrap implica que no solamente se tiene que ver bien y ser responsive, también tiene que ser semánticamente correcta. La utilización de una semántica adecuada en el código no solo mejora la legibilidad y el mantenimiento, sino que también facilita a los motores de búsqueda en el proceso de indexar y comprender el contenido de la página. Estos usan arañas o crawlers que son programas automatizados utilizados por los motores de búsqueda para recorrer la web de forma sistemática, recopilando información sobre el contenido de las páginas. Un código bien estructurado y semántico ayuda a estas arañas a interpretar y clasificar el contenido de manera más efectiva, lo que puede contribuir a mejorar el posicionamiento y la visibilidad de la página en los resultados de búsqueda.

# Estructura de la Página Web

La web consta de cuatro páginas principales, cada una con su propósito específico: la página principal, la página de la carta, la página del blog y la página de contacto.

Todas estas páginas comparten estilos que se encuentran en el archivo `custom.css`. Además, el diseño del `footer` y `navbar` es consistente en la mayoría de las páginas, a excepción de las páginas de la carta y el blog, que presentan una variación del `navbar` para adaptarse mejor al contenido específico de cada sección.

# Elementos Comunes

## Barra de Navegación (Nav)

El elemento de navegación (Nav) es consistente en todas las páginas. Incluye los siguientes elementos:

- **Logo:** El logo sirve como enlace a la página principal.
- **Enlaces de Páginas:** Proporciona enlaces a las diferentes páginas de la web.
- **Modo Claro/Oscuro:** Un desplegable con iconos permite al usuario cambiar entre el modo claro y oscuro.
- **Barra de Búsqueda:** Permite a los usuarios buscar información específica en la página.
- **Botón de Búsqueda:** Activa la barra de búsqueda para facilitar la interacción.
- **Responsive Design:** Es completamente responsive, adaptándose a diferentes tamaños de pantalla. En pantallas más pequeñas, se muestra una hamburguesa (botón) para plegar y desplegar la navegación. Todos los elementos se agrupan a la izquierda en lugar de en el centro.
- **Acción de Plegar y Desplegar:** La acción de plegar y desplegar utiliza JavaScript, utilizando las bibliotecas de Bootstrap por defecto.

### Implementación Navbar

- Se utiliza la clase `navbar` de Bootstrap para garantizar un diseño responsivo y adaptable.
- La clase `navbar-expand-lg` permite que la barra de navegación se expanda en pantallas más grandes y se pliegue en pantallas más pequeñas.
- Se utiliza una imagen como logotipo, que sirve como enlace a la página principal.
- El botón con la clase `navbar-toggler` controla la visualización de la navegación en pantallas más pequeñas, como dispositivos móviles, utilizando el atributo `data-bs-toggle` para cambiar entre plegado y desplegado.
- La clase `navbar-collapse` se utiliza para agrupar los elementos de navegación y asegurar que se alineen correctamente en diferentes tamaños de pantalla.
- Los elementos de la lista `navbar-nav` se presentan a la derecha, y cada uno de ellos se ha estilizado utilizando las clases proporcionadas por Bootstrap.

La estructura del `nav` se ha implementado de manera limpia y efectiva, lo que facilita la navegación del usuario y asegura una experiencia consistente en una variedad de dispositivos.

## Footer

El `footer` del sitio web ha sido diseñado para proporcionar información esencial y opciones de contacto a los visitantes. Se compone de varias secciones que se distribuyen de manera efectiva en diferentes tamaños de pantalla, asegurando una experiencia amigable.

- **VISÍTANOS:** Esta sección destaca la filosofía de la pizzería, enfocada en la frescura y la calidad. Proporciona una breve descripción de la hospitalidad y la variedad de platos disponibles.

- **HORARIO:** Aquí, los usuarios pueden consultar el horario de funcionamiento de la pizzería durante la semana y los fines de semana.

- **CONTACTO:** Ofrece información de contacto, incluyendo la dirección, número de teléfono y un enlace de correo electrónico para consultas directas.

- **BOLETÍN:** Los visitantes pueden suscribirse al boletín informativo de la pizzería ingresando su correo electrónico en el campo proporcionado y haciendo clic en el botón "Suscribirse".

- **Redes Sociales:** Se incluyen enlaces a las redes sociales de la pizzería para mantener a los usuarios actualizados sobre noticias y eventos.

### Implementación Footer

El `footer` del sitio web hace uso de varias clases de Bootstrap para una presentación adecuada y una experiencia de usuario consistente:

- Las clases `col-md-3` se utilizan para la distribución en columnas de tamaño medio, asegurando una disposición adecuada de los elementos en pantallas de tamaño mediano.
- La clase `d-none` se implementa para ocultar ciertas secciones del footer en dispositivos más pequeños, evitando la sobrecarga de información y mejorando la legibilidad.
- La clase `d-md-block` se utiliza para asegurar que los elementos ocultos en dispositivos más pequeños sean visibles en pantallas de tamaño mediano, permitiendo que la información importante esté disponible cuando sea necesario.
- Los iconos utilizados, como `bi-geo-alt-fill`, `bi-clock`, `bi-sign-intersection-fill`, y `bi-envelope`, son de la biblioteca Bootstrap Icons, lo que asegura una presentación visual coherente y atractiva.
- Se hace uso de la clase `input-group` para el formulario de suscripción, mejorando la presentación y usabilidad del campo de correo electrónico y el botón de suscripción.
- Los iconos de redes sociales, como `bi-twitter`, `bi-facebook`, `bi-google`, y `bi-linkedin`, se utilizan como enlaces a las respectivas redes sociales de la pizzería, todos los iconos vienen de la biblioteca oficial de bootstrap icons.

El `footer` ha sido diseñado teniendo en cuenta la experiencia del usuario, garantizando que la información importante sea accesible y que la distribución de elementos sea adecuada en diferentes dispositivos.

# Página Principal

En la parte superior de la página principal, el `navbar` se mantiene fijo en la parte superior en todo momento, garantizando una navegación fácil y accesible para los usuarios. La sección inicial se compone de una impresionante "landing page" con un encabezado atractivo.

- La imagen de fondo se presenta con un efecto profesional utilizando un degradado de opacidad del 0.5, lo que aporta una sensación visual agradable y atractiva para los usuarios.
- El título prominente de la página web se destaca en la parte central de la landing page, asegurando que los visitantes tengan una comprensión clara del propósito y la identidad de la pizzería desde el primer momento.
- Se incorpora un botón de llamada a la acción (call to action) estratégicamente ubicado, que dirige a los usuarios hacia el menú. Esta llamada a la acción está diseñada con la intención de guiar a los visitantes hacia el área de la web donde se llevan a cabo las conversiones, facilitando así el proceso de generación de ventas y pedidos.

## Sección de Servicios

A continuación, se presenta una sección de servicios que resalta las diversas ventajas asociadas con el negocio de la pizzería. La implementación de esta sección se ha realizado de la siguiente manera:

- Se han utilizado iconos de la biblioteca `Bootstrap Icons` para representar visualmente cada servicio, proporcionando una presentación clara y concisa de las características clave.
- La distribución de los elementos se adapta dinámicamente según el tamaño de la pantalla utilizando las clases `col-md-6` y `col-lg-3`, lo que garantiza una presentación óptima y una experiencia consistente en una variedad de dispositivos.
- La clase `fs` se emplea para controlar el tamaño de las fuentes, asegurando una presentación visual equilibrada y legible en todos los dispositivos.

Esta sección se ha diseñado estratégicamente para comunicar eficazmente las ventajas competitivas de la pizzería, lo que contribuye a atraer y retener a los clientes.

## Sección de Recomendaciones

En esta sección se destacan los cuatro platos más populares de la carta, seleccionados estratégicamente para impulsar las ventas y satisfacer las preferencias de los clientes. La implementación de esta sección se ha llevado a cabo de la siguiente manera:

- Se presentan cuatro tarjetas con imágenes y descripciones detalladas de los platos destacados, así como información relevante sobre alérgenos.
- En pantallas más grandes, las tarjetas se distribuyen en dos filas utilizando la clase `col-lg-6`, mostrando dos tarjetas en cada fila. Además, se ajusta el orden de las tarjetas utilizando las clases `order-first`, `order-last` y `order-md-last`, lo que permite una presentación dinámica y diferente según el dispositivo usado para ver la web.
- La distribución de las tarjetas se adapta en pantallas medianas utilizando la clase `col-md-6`. En dispositivos móviles, las tarjetas se presentan en una sola columna con un orden alterado por `order-first` y `order-last`, lo que mejora la legibilidad y la experiencia de usuario en pantallas más pequeñas.
- También es importante destacar que todas las tarjetas incluyen una animación al pasar el cursor creada con CSS. Esta animación de hover se ha implementado para mejorar la interactividad y la experiencia de usuario en el sitio web. Cabe mencionar que esta misma animación se aplicará a varios elementos adicionales en diferentes secciones del proyecto, lo que asegura una coherencia visual y una sensación uniforme en todo el sitio web. Además evitamos crear más css de lo estríctamente necesario.

Esta sección ha sido diseñada para resaltar los platos más populares y fomentar la participación de los clientes, ya que serán ellos los que decidan de forma indirecta decidan que platos hay en esta sección.

## Sección de Entrega a Domicilio

Una sección adicional recuerda a los clientes que se ofrece servicio de entrega a domicilio a través de diferentes plataformas de reparto, como Uber Eats, Just Eat y Deliveroo. La implementación de esta sección se destaca por lo siguiente:

- Se utiliza un fondo con degradado (bg-gradient) para resaltar esta sección y diferenciarla visualmente del resto del contenido, atrayendo la atención del usuario de manera efectiva.
- Se integra un mapa interactivo utilizando la API de Google Maps, que permite a los clientes ubicar fácilmente el local y tener una referencia clara para realizar pedidos o recoger los productos en persona.
- Se incluyen enlaces a las diferentes plataformas de reparto, lo que facilita que los usuarios accedan rápidamente a la página correspondiente y realicen pedidos de manera conveniente.

Esta sección está diseñada con el objetivo de resaltar la conveniencia y accesibilidad de los servicios de entrega a domicilio, lo que contribuye a aumentar la comodidad y la satisfacción del cliente.

## Sección de Opiniones

La sección de opiniones presenta comentarios de clientes famosos, que se acompañan de un icono de avatar representativo de la persona, su nombre y su valoración en forma de estrellas de la biblioteca `Bootstrap Icons`.

- Se utiliza la clase `bg-light` para aplicar un fondo claro a la sección, lo que mejora la legibilidad y la presentación de las opiniones de los clientes.
- La sección está diseñada con márgenes superiores (`mt-3`) y un relleno interno (`py-5`), lo que asegura un espaciado adecuado y una presentación visual equilibrada en la página.
- Se ha aplicado la clase `row-cols-1 row-cols-md-3` para ajustar el número de columnas en función del tamaño de la pantalla, permitiendo que las tarjetas de opinión se muestren en una sola columna en dispositivos móviles y en tres columnas en pantallas medianas.
- Se han utilizado imágenes de avatares de diferentes clientes, lo que agrega un toque personal y humano a las opiniones.

Esta sección se ha diseñado con el propósito de generar confianza y credibilidad entre los visitantes, al destacar las experiencias positivas de clientes notables y reconocidos.

## Horario de Atención

La inclusión de un horario de atención en la página principal tiene como objetivo principal proporcionar a los clientes información clara y accesible sobre cuándo pueden disfrutar de los servicios del restaurante. Esto facilita la planificación de visitas y pedidos, mejorando la experiencia del cliente y evitando posibles contratiempos.

La implementación de esta tabla de horarios de atención se destaca por los siguientes aspectos:

- Se utiliza la clase `table-responsive` para asegurar que la tabla se adapte de manera efectiva a diferentes tamaños de pantalla.
- El ancho de la tabla se controla con la clase `w-75`, lo que garantiza un tamaño adecuado en la página.
- La tabla se presenta con un borde redondeado (`rounded-2`) y un relleno interno (`py-5`), lo que mejora la presentación visual y la legibilidad de la información.
- Se ha aplicado un diseño limpio y claro utilizando las clases `table-bordered`, `table-striped`, y `table-hover`, lo que contribuye a una presentación atractiva y una experiencia de usuario fluida al interactuar con la tabla.
- El texto se centra visualmente utilizando la clase `text-center`.

## Novedades y Eventos

La sección de "Novedades y Eventos" en la página web proporciona a los visitantes información actualizada sobre las últimas noticias y actividades especiales del restaurante. Esta sección está estructurada de la siguiente manera:

- Se utiliza un contenedor principal (`container`) para mantener y organizar el contenido de la sección.
- El encabezado destacado en la sección se logra mediante el uso de la clase `page-header`, que centra y resalta el título principal "Novedades y Eventos".
- La estructura de la sección se compone de una fila (`row`) que alberga dos columnas: una columna más grande (`col-md-8`) y una columna más pequeña (`col-md-4`).
- La columna más grande contiene un componente de acordeón (`accordion`), que se implementa utilizando la clase correspondiente de Bootstrap. Este componente permite desplegar información detallada sobre cada evento, lo que permite a los visitantes obtener más detalles con solo un clic.
- La columna más pequeña presenta un código QR que permite a los clientes acceder de manera rápida y sencilla al menú especial del restaurante. El código QR se visualiza de manera atractiva utilizando la clase `img-fluid` y un estilo específico de altura para mantener una presentación equilibrada.
- Aunque pueda parecer que no, realmente el QR si que está centrado.
