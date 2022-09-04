
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="flexbox.css">
    <title>FlexBox</title>
</head>
<body>
    <div class="contenedor">
        <div class="item item1">Item 1</div>
        <div class="item item2">Item 2</div>
        <div class="item item3">Item 3</div>
        <div class="item item4">Item 4</div>
    </div>
</body>
</html>

CSS
-----
/* https://codepen.io/enxaneta/full/adLPwv */

.contenedor {
    background-color: yellow;
    padding: 0.5rem;
    display: flex;
    gap: 0.5rem;
    min-height: 5rem;
    /* Eje principal */
    justify-content: space-around;

    /* Eje secundario */
    align-items: center;

    /* flex-direction: column; */

    flex-wrap: wrap;
}

.item {
    background-color: salmon;
    padding: 0.25rem;
    width: 10rem;
}

.item2 {
    align-self: stretch;
}