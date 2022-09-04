
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tooltip</title>
    <link rel="stylesheet" href="tooltip.css">
</head>
<body>
    <button class="btn-tooltip">Buscar
        <span class="tooltip">Hace una búsqueda de tu crush</span>
    </button>
    <div class="triangulo"></div>
</body>
</html>

CSS
-----
body {
    padding: 0;
    margin: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
}

.btn-tooltip {
    position: relative;
    padding: 10px 20px;
    border-radius: 5px;
    border: none;
    background-color: green;
    color: white;
    border-bottom: 2px solid darkgreen;
    cursor: pointer;
    transition: background-color 150ms;
}

/* .btn-tooltip:hover::before {
    content: "Esto es un tooltip";
} */

.tooltip {
    position: absolute;
    /* visibility: hidden; */
    opacity: 0;
    top: -50px;
    left: -100%;
    transform: translateX(25%);
    color: #ddd;
    background-color: #333;
    padding: 5px 10px;
    border-radius: 5px;
    transition: opacity 150ms;
}

.btn-tooltip:hover {
    background-color: rgb(0, 100, 0);
}

.btn-tooltip:hover .tooltip {
    /* visibility: visible; */
    opacity: 1;
}

.tooltip::before {
    content: '';
    border: solid 10px transparent;
    border-top-color: #333;
    position: absolute;
    top: 40px;
    left: 50%;
    transform: translateX(-50%);
}

/* .triangulo {
    border: solid 10px transparent;
    border-top-color: #333;
} */