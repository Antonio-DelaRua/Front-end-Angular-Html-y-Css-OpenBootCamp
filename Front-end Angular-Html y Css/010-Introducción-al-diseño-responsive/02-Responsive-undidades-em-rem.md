
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unidades EM y REM</title>
    <link rel="stylesheet" href="unidades-em.css">
</head>
<body>
    <div class="escenario-1 escenario">
        <div class="em">2em</div>
        <div class="rem">2rem</div>
    </div>
    <div class="escenario-2 escenario">
        <div class="em">2em</div>
        <div class="rem">2rem</div>
    </div>
</body>
</html>

CSS
------
.escenario {
    border: 1px solid #333;
    padding: 10px;
}

.escenario-1 {
    font-size: 32px;
}

.escenario-2 {
    font-size: 16px;
}

.em {
    font-size: 2em;
}

.rem {
    font-size: 2rem;
}