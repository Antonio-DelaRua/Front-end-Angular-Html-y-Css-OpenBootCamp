
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Variables</title>
    <link rel="stylesheet" href="variables.css">
</head>
<body>
    <div class="contenedor">
        <h1 class="titulo">Título</h1>
        <p class="parrafo">Este es el párrafo</p>
        <p class="footer">Este es el pie de página</p>
    </div>
</body>
</html>

CSS
-----
:root {
    --color-principal: rgb(195, 0, 255);
    --ancho-principal: 350px;
}

.titulo {
    color: var(--color-principal);
}

.footer {
    color: var(--color-principal);
}

.contenedor {
    background-color: antiquewhite;
    padding: 1rem;
    max-width: var(--ancho-principal);
}