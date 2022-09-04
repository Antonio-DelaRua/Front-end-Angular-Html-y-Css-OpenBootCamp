
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Estilos Formularios</title>
    <link rel="stylesheet" href="../css/estilosformularios.css" />
  </head>
  <body>
    <form action="" method="">
      <input class="input" type="text" name="name" />
      <input class="input" type="password" name="password" />

      <input
        class="input-moderno"
        type="text"
        name="name"
        placeholder="Tu nombre"
      />

      <input
        class="input-background"
        type="text"
        name="name"
        placeholder="Tu nombre"
      />

      <input
        class="input-search"
        type="text"
        name="name"
        placeholder="Tu nombre"
      />

      <textarea name="descripcion"></textarea>

      <select>
          <option>Opción 1</option>
          <option>Opción 2</option>
          <option>Opción 3</option>
      </select>
    </form>
  </body>
</html>

css
-----

.input {
    width: 100%;
    padding: 5px 10px;
    border: 2px solid green;
    border-radius: 10px;
    margin-bottom: 10px;
}

.input[type="password"] {
    color: red;
}

.input-moderno {
    border: none;
    border-bottom: 1px solid #c2c2c2;
    outline: none;
    padding: 5px;
    color: #5f5f5f;
}

.input-moderno::placeholder {
    color: #c2c2c2;
}

.input-moderno:focus {
    border-bottom: 1px solid #5f5f5f;
}

.input-background {
    background-color: aquamarine;
    border: none;
    border-radius: 5px;
    padding: 5px 10px;
    outline: none;
    color: white;
    box-shadow: 0 0 10px #ccc;
}

.input-background::placeholder {
    color: #ccc;
}

.input-search {
    padding: 10px;
    padding-left: 30px;
    /* border: none; */
    background-color: #fff;
    border-radius: 8px;
    margin: 10px;
    background-image: url('../img/searchicon.png');
    background-repeat: no-repeat;
    background-position: 5px;
}

textarea {
    resize: none;
}

select {
    width: 100%;
    padding: 15px;
    background-color: #ccc;
}