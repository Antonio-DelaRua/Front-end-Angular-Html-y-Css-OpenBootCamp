
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pseudo-Elementos</title>
    <link rel="stylesheet" href="../css/pseudoelementos.css">
    <!-- https://www.w3schools.com/css/css_pseudo_elements.asp -->
</head>
<body>
    <div class="contenedor">
        <p><span class="frase">En medio de la dificultad reside la oportunidad</span> - Albert Einstein</p>
    </div>
    <div class="libro">
        <p>
            Laboris sunt in reprehenderit adipisicing consequat id est laboris Lorem ea fugiat irure fugiat. Fugiat non consectetur do enim quis nisi culpa velit ipsum quis cillum pariatur. Esse aliquip cillum consectetur commodo irure tempor cupidatat et. Exercitation veniam voluptate non enim aute irure ut ipsum adipisicing. Aute quis mollit pariatur ad adipisicing nostrud aute velit do qui. Reprehenderit nulla exercitation nulla elit adipisicing nulla enim sint officia anim fugiat veniam ea deserunt.
        </p>
    </div>
    <div class="listado">
        <ul>
            <li>Elemento 1</li>
            <li>Elemento 2</li>
            <li>Elemento 3</li>
        </ul>
        <ol>
            <li>Elemento 1</li>
            <li>Elemento 2</li>
            <li>Elemento 3</li>
        </ol>
    </div>
</body>
</html>

CSS
-----
.contenedor {
    width: 300px;
    height: 100px;
    background-color: aquamarine;
}

div {
    background-color: blue;
}

span.frase {
    font-style: italic;
}

span.frase::before {
    content: '<< ';
    font-size: xx-small;
}
span.frase::after {
    content: ' >>';
    font-size: xx-small;
}

.libro {
    background-color: bisque;
    padding: 15px;
    font-family: Arial;
}

.libro p::first-letter {
    font-size: xx-large;
}

.libro p::first-line {
    color: white;
}

.libro p::selection {
    background-color: chocolate;
    color: lime;
}

.listado li::marker {
    color: red;
}