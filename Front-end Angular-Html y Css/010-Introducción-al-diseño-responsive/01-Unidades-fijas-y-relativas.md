
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unidades</title>
    <link rel="stylesheet" href="unidades.css">
</head>
<body>
    <h1>Unidades fijas y relativas</h1>
    <div class="escenario-1 escenario">
        <div class="px">200px</div>
        <div class="porcentaje">50%</div>
        <div class="view">50vw</div>
    </div>
    <div class="escenario-2 escenario">
        <div class="px">200px</div>
        <div class="porcentaje">50%</div>
        <div class="view">50vw</div>
    </div>
</body>
</html>


CSS
-------
body {
    padding: 20px;
    margin: 0;
}
.escenario {
    margin: 10px 0px;
    border: 1px solid #ccc;
    padding: 10px;
}

.escenario-1 {
    width: 100%;
}
.escenario-2 {
    width: 50%;
}

.px {
    background-color: green;
    width: 200px;
}

.porcentaje {
    background-color: red;
    width: 50%;
}

.view {
    background-color: yellow;
    width: 50vw;
}