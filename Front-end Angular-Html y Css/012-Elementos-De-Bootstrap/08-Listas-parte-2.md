
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Listas 2</title>
    <link
      href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css"
      rel="stylesheet"
      integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3"
      crossorigin="anonymous"
    />
  </head>
  <body>
    <div class="container py-4">
      <div class="row">
        <div class="col-4">
          <div class="list-group" id="list-tab" role="tablist">
            <a
              class="list-group-item list-group-item-action active"
              id="list-home-list"
              data-bs-toggle="list"
              href="#list-home"
              role="tab"
              aria-controls="list-home"
              >Inicio</a
            >
            <a
              class="list-group-item list-group-item-action"
              id="list-profile-list"
              data-bs-toggle="list"
              href="#list-profile"
              role="tab"
              aria-controls="list-profile"
              >Perfil</a
            >
            <a
              class="list-group-item list-group-item-action"
              id="list-messages-list"
              data-bs-toggle="list"
              href="#list-messages"
              role="tab"
              aria-controls="list-messages"
              >Messages</a
            >
            <a
              class="list-group-item list-group-item-action"
              id="list-settings-list"
              data-bs-toggle="list"
              href="#list-settings"
              role="tab"
              aria-controls="list-settings"
              >Settings</a
            >
          </div>
        </div>
        <div class="col-8">
          <div class="tab-content" id="nav-tabContent">
            <div
              class="tab-pane fade show active"
              id="list-home"
              role="tabpanel"
              aria-labelledby="list-home-list"
            >
              Esta es la home
            </div>
            <div
              class="tab-pane fade"
              id="list-profile"
              role="tabpanel"
              aria-labelledby="list-profile-list"
            >
              Este es tu perfil - personalizado
            </div>
            <div
              class="tab-pane fade"
              id="list-messages"
              role="tabpanel"
              aria-labelledby="list-messages-list"
            >
              Estos son tus mensajes
            </div>
            <div
              class="tab-pane fade"
              id="list-settings"
              role="tabpanel"
              aria-labelledby="list-settings-list"
            >
              Aquí tienes los ajustes
            </div>
          </div>
        </div>
      </div>
    </div>
  </body>
  <script
    src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js"
    integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p"
    crossorigin="anonymous"
  ></script>
</html>