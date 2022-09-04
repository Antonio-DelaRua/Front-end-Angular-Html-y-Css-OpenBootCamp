
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Grid</title>
    <link rel="stylesheet" href="grid.css">
</head>
<body>
    <div class="contenedor">
        <div class="item item1">1</div>
        <div class="item item2">2</div>
        <div class="item item3">3</div>
        <div class="item item4">4</div>
        <div class="item item5">5</div>
        <div class="item item6">6</div>
        <div class="item item7">7</div>
        <div class="item item8">8</div>
        <div class="item item9">9</div>
    </div>
</body>
</html>

CSS
------
.contenedor {
    display: grid;
    gap: 0.5rem;
    /* column-gap: 0.1rem; */
    /* row-gap: 1rem; */
    /* grid-template-columns: auto auto auto; */
    /* grid-template-columns: repeat(3, auto); */
    /* grid-template-columns: 20px 3rem 25vw; */
    grid-template-columns: 1fr 1fr 3fr;
    grid-template-rows: 200px 5rem 100px;
    /* grid-template-areas: 'head head head' 'main main aside' 'footer footer footer'; */
}

.item {
    background-color: aquamarine;
    padding: 0.25rem;
    font-size: 2rem;
    border: solid 1px blue;
}

.item1 {
    /* grid-column: 1 / 3; */
    grid-column: 2 / span 2;
    /* grid-area: head; */
}

.item9 {
    /* grid-area: footer; */
    grid-area: 2 / 1 / 4 / 3;
    /* grid-area: filainicio / colinicio / filafin / colfin */
}