
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Animaciones</title>
    <link rel="stylesheet" href="animaciones.css">
</head>
<body>
    <div class="padre">
        <div class="hijo"></div>
    </div>
</body>
</html>

CSS
-----
.padre {
    width: 400px;
    height: 400px;
    background-color: blue;
}

.hijo {
    width: 50%;
    height: 50%;
    background-color: beige;
    /* transition: transform 1s ease-in 2s; */
    animation: traslacion 4s ease-in-out infinite forwards alternate;
}

.padre:hover .hijo {
    /* transform: translateX(100%);
    background-color: blueviolet; */
    animation-play-state: paused;
}

@keyframes traslacion {
    0% {
        background-color: beige;
        transform: translateX(0%) translateY(0%);
    }
    25% {
        transform: translateX(100%) translateY(0%);
    }
    50% {
        transform: translateX(100%) translateY(100%);
    }
    75% {
        transform: translateX(0%) translateY(100%);
    }
    100% {
        background-color: darkorange;
        transform: translateX(0%) translateY(0%);
    }
}