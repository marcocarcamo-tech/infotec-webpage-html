# infotec-webpage-html

Esta página corresponde con la tarea de infotec para el curso de html, la cual consiste en crear una página empleando los elementos enseñados en la unidad 1.

1. El proyecto pide emplear al menos 3 etiquetas que no se hayan visto a lo largo de las lecciones.

En mi caso utilicé las siguientes etiquetas:

- <ul>: sirve para abrir una lista no ordenada.
- <li>: esta etiqueta se usa para cada uno de los elementos dentro de nuestra lista.
- <label>: sirve para poner texto a nuestros campos de input y los unimos con estos a través de la propiedad for.

1. Exposición del proyecto

La página creada es sobre los mejores videojuegos de terror según las críticas. Acontinuación describiré los elementos empleados en la misma.

 

### Hipervínculos y anclas

En el sitio hay enlaces a sitios externos como en el siguiente caso

```html
el sitio de <a href="https://www.metacritic.com/">Metacritic</a> y buscar las puntuaciones.
```

El sitio también contiene anclas para encontrar rápidamente cada elemento del listado presentado:

```html
<!-- Ancla -->
<li><a href="#resident_2">5. Resident Evil 2</a></li>

<!-- Elemento anclado -->
<center><h2><a id="resident_2"></a>5. Resident Evil 2</h2></center>
```

### Tablas

Al igual que en el video de repaso presentado, esta página presenta la información haciendo uso de tablas, de forma que en una columna se encuentra la información y en otra una imagen. 

```html
<table>
        <td class="texto">
            <p>Resident Evil 2, la segunda entrega de la que posiblemente sea la mejor franquicia de videojuegos de terror de todos los tiempos, es un ejemplo de survival horror. Presenta mejoras generales respecto a su predecesor en casi todos los aspectos, con un claro enfoque en la exploración, los puzles y el combate.

            Cuenta con personajes para dos jugadores, con caminos ramificados y argumentos únicos para cada uno. Quizá el mayor logro de este juego sea el de consolidar a Resident Evil no como un éxito puntual, sino como una franquicia continua que seguiría siendo de gran calidad durante décadas.</p>
        </td>
        <td>
            <img src="../assets/resident_2.webp" alt="resident2_img">
        </td>
    </table>
```

### Formularios

En el proyecto se un incluye un breve formulario que además hace uso de los elementos

- fieldset
- legend
- labels
- botón de submit

```html
<form action="registrar_datos.php" method="post">
        <form action="registrardatos.php" method="post">
            <fieldset>
                <legend>Datos de contacto</legend>
    
                <label for="nombre">Nombre: </label>
                <input type="text" id="nombre" name="nombre" size="30"><br>
                <label for="E-mail">E-mail: </label>
                <input type="text" name="dni" size="8"><br> 
            </fieldset>
    
            <fieldset>
                <legend>Déjanos saber tu opinión</legend>
                <label for="comentarios">Comentarios</label>
                <textarea name="comentarios" id="comentarios" cols="30" rows="10"></textarea>
            </fieldset>

            <input class="submit" type="submit" value="Enviar">
    </form>
```