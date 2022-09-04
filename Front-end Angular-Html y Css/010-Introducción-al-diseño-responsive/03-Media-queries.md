
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Media Queries</title>
    <link rel="stylesheet" href="mediaqueries.css">
</head>
<body>
    <h1>Título</h1>
    <p>Este es un párrafo</p>
</body>
</html>

CSS
--------h1 {
    color: red;
    font-size: 4rem;
}

p {
    color: black;
    font-size: 2rem;
}

/* @media all and (max-width: 576px) { */
/* @media (max-width: 576px) {
    h1 {
        color: blue;
    }
} */

@media (min-width: 576px) {
    h1 {
        color: green;
    }
}

@media (min-width: 995px) {
    h1 {
        color: blue;
    }
}

@media (orientation: landscape) and (min-height: 400px) {
    p {
        color: brown;
    }
}

@media (min-height: 300px), (min-width: 1100px) {
    h1 {
        color: darksalmon;
    }
}