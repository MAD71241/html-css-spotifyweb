<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="icon" href="./assets/img/favicon.ico" type="image/x-icon" />
    <link
      rel="stylesheet"
      href="https://use.fontawesome.com/releases/v5.1.1/css/all.css"
      integrity="sha384-O8whS3fhG2OnA5Kas0Y9l3cfpmYjapjI0E4theH4iuMD+pLhbf6JI0jIMfYcK3yZ"
      crossorigin="anonymous"
    />
    <link
      rel="stylesheet"
      href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css"
      integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T"
      crossorigin="anonymous"
    />
    <link rel="stylesheet" href="./assets/css/style.css" />
    <link rel="stylesheet" href="./assets/css/media.css" />
    <title>Spotify WebApp</title>
  </head>

  <body class="background-main">
    <!-- Header -->
    <section class="header">
      <h6 class="text-uppercase">Effettua l'upgrade</h6>
    </section>
    <!-- /Header -->

    <!-- Sidebar -->
    <section class="sidebar">
      <!-- Header - Logo -->
      <div class="sidebar-header">
        <img src="./assets/img/logo.svg" alt="spotify logo large" />
        <img
          src="./assets/img/logo-small.svg"
          class="mobile-logo"
          alt="spotify logo small"
        />
      </div>
      <!-- /Header - Logo -->

      <!-- Sezione Top Sidebar -->
      <div class="top-sidebar font-spotifygrey">
        <span class="active-selector"></span>
        <ul class="nav flex-column align-content-center">
          <li class="nav-item">
            <a
              class="nav-link py-1 font-spotifygrey font-weight-bold active"
              href="#"
              ><img src="./assets/img/home.svg" alt="" /><span class="pl-2"
                >Home</span
              ></a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link py-1 font-spotifygrey font-weight-bold" href="#"
              ><img src="./assets/img/search.svg" alt="" /><span class="pl-2"
                >Cerca</span
              ></a
            >
          </li>
          <li class="nav-item">
            <a class="nav-link py-1 font-spotifygrey font-weight-bold" href="#"
              ><img src="./assets/img/libreria.svg" alt="" /><span class="pl-2"
                >La tua libreria</span
              ></a
            >
          </li>
        </ul>
      </div>
      <!-- /Sezione Top Sidebar -->

      <!-- Sezione Playlist Sidebar -->
      <div class="add-playlist">
        <i class="fas fa-plus"></i>
        <span class="font-spotifygrey">Crea Playlist</span>
      </div>

      <div class="playlist">
        <ul class="font-spotifygrey">
          <li>Aggiungi Playlist</li>
          <li>Aggiungi Playlist</li>
          <li>Aggiungi Playlist</li>
          <li>Aggiungi Playlist</li>
          <li>Aggiungi Playlist</li>
          <li>Aggiungi Playlist</li>
        </ul>
      </div>
      <!-- /Sezione Playlist Sidebar -->

      <!-- Sezione Utente Sidebar -->
      <div class="bottom-sidebar">
        <div class="user">
          <div>
            <img
              src="./assets/img/download.svg"
              id="download"
              alt="Download Icon"
            />
            <span class="font-spotifygrey font-weight-bold">Installa app</span>
          </div>
          <hr />
          <div>
            <img
              src="./assets/img/profile.svg"
              id="profile"
              alt="Profile Icon"
            />
            <span class="font-spotifygrey font-weight-bold active"
              >John Doe</span
            >
          </div>
        </div>
      </div>
      <!-- /Sezione Utente Sidebar -->
    </section>
    <!-- /Sidebar -->

    <!-- Sezione Player -->
    <section class="player">
      <!-- Sezione sinistra del player -->
      <div class="player-left">
        <img
          src="./assets/img/sinister.jpeg"
          alt="album in play"
          class="player-thumbnail"
        />
        <div class="row ml-1">
          <h5 class="p-0 mb-0 text-white">Artista</h5>
          <h6 class="font-spotifygrey p-0 mb-0" id="song-name">Nome Brano</h6>
        </div>
        <div class="row ml-1">
          <div class="col-12 col-sm-6" id="heart">
            <i class="far fa-heart"></i>
          </div>
          <div class="col-12 col-sm-6" id="bookmark">
            <i class="far fa-folder"></i>
          </div>
        </div>
      </div>
      <!-- /Sezione sinistra del player -->

      <!-- Sezione centrale del player -->
      <div class="music-player">
        <i class="fas fa-random"></i>
        <i class="fas fa-step-backward"></i>
        <i class="far fa-play-circle"></i>
        <i class="fas fa-step-forward"></i>
        <i class="fas fa-redo-alt"></i>
        <div class="progress-bar">
          <div class="actual-progress">
            <div class="progress-slider"></div>
          </div>
          <h6 id="time-passed">1:20</h6>
          <h6 id="time-left">4:30</h6>
        </div>
      </div>

      <div class="player-right text-white">
        <i class="fas fa-list-ul p-1"></i>
        <i class="fas fa-desktop p-1"></i>
        <i class="fas fa-volume-up p-1">
          <div class="volume-bar-mobile">
            <div class="volume-bar-slide">
              <div class="volume-bar-slider"></div>
            </div>
          </div>
        </i>
        <div class="volume-bar">
          <div class="volume-bar-slide">
            <div class="volume-bar-slider"></div>
          </div>
        </div>
      </div>
    </section>
    <!-- /Sezione Player -->

    <!-- MACRO-SEZIONE MAIN -->
    <main class="background-main">
      <div class="container-fluid">
        <div class="row">
          <div class="col-12 text-white" id="main">
            <!-- Navbar centrale -->
            <div class="row">
              <div class="col-2"></div>
              <div class="col-8">
                <div class="row">
                  <div class="col-lg-2 col-md-3 col-4 text-uppercase">
                    <h6>in evidenza</h6>
                    <div class="divider"></div>
                  </div>
                  <div class="col-lg-2 col-md-3 col-4 text-uppercase">
                    <h6>podcast</h6>
                  </div>
                  <div class="col-lg-2 col-md-3 col-4 text-uppercase">
                    <h6>classifiche</h6>
                  </div>
                  <div class="col-lg-2 col-md-3 col-4 text-uppercase">
                    <h6>generi e mood</h6>
                  </div>
                  <div class="col-lg-2 col-md-3 col-4 text-uppercase">
                    <h6>nuove uscite</h6>
                  </div>
                  <div class="col-lg-2 col-md-3 col-4 text-uppercase">
                    <h6>scopri</h6>
                  </div>
                </div>
              </div>
              <div class="col-2"></div>
            </div>
            <!-- /Navbar centrale -->

            <h2>Recently Played</h2>
            <!-- prima row, recently played -->
            <div class="row pb-5">
              <div class="album-thumbnail text-center col-6 col-md-3 col-lg-2">
                <div class="image-container">
                  <img
                    src="./assets/img/metal_lifting.jpg"
                    alt="metal albums"
                    class="album-thumbnail"
                  />
                  <div class="overlay">
                    <i class="far fa-play-circle"></i>
                  </div>
                </div>
                <h5 id="metal">title</h5>
                <h6 class="font-spotifygrey">subtitle</h6>
              </div>
              <div class="album-thumbnail text-center col-6 col-md-3 col-lg-2">
                <div class="image-container">
                  <img
                    src="./assets/img/stranger.jpeg"
                    alt="stranger things ost"
                    class="album-thumbnail"
                  />
                  <div class="overlay">
                    <i class="far fa-play-circle"></i>
                  </div>
                </div>
                <h5>title</h5>
                <h6 class="font-spotifygrey">subtitle</h6>
              </div>
              <div class="album-thumbnail text-center col-6 col-md-3 col-lg-2">
                <div class="image-container">
                  <img
                    src="./assets/img/aquietplace.jpeg"
                    alt="a quiet place album cover"
                    class="album-thumbnail"
                  />
                  <div class="overlay">
                    <i class="far fa-play-circle"></i>
                  </div>
                </div>
                <h5>title</h5>
                <h6 class="font-spotifygrey">subtitle</h6>
              </div>
              <div class="album-thumbnail text-center col-6 col-md-3 col-lg-2">
                <div class="image-container">
                  <img
                    src="./assets/img/split.jpeg"
                    alt="split album cover"
                    class="album-thumbnail"
                  />
                  <div class="overlay">
                    <i class="far fa-play-circle"></i>
                  </div>
                </div>
                <h5>title</h5>
                <h6 class="font-spotifygrey">subtitle</h6>
              </div>
              <div class="album-thumbnail text-center col-6 col-md-3 col-lg-2">
                <div class="image-container">
                  <img
                    src="./assets/img/cure.jpeg"
                    alt="a cure for welness album cover"
                    class="album-thumbnail"
                  />
                  <div class="overlay">
                    <i class="far fa-play-circle"></i>
                  </div>
                </div>
                <h5>title</h5>
                <h6 class="font-spotifygrey">subtitle</h6>
              </div>
              <div class="album-thumbnail text-center col-6 col-md-3 col-lg-2">
                <div class="image-container">
                  <img
                    src="./assets/img/sinister.jpeg"
                    alt="sinister album cover"
                    class="album-thumbnail"
                  />
                  <div class="overlay">
                    <i class="far fa-play-circle"></i>
                  </div>
                </div>
                <h5>title</h5>
                <h6 class="font-spotifygrey">subtitle</h6>
              </div>
            </div>
            <!-- /prima row -->

            <!-- seconda row, suggerimenti -->
            <h2>Creato per John Doe</h2>
            <h6 class="font-spotifygrey">
              Pi?? ascolti, pi?? accurati saranno i suggerimenti.
            </h6>
            <div class="row pb-5">
              <div class="album-thumbnail text-center col-6 col-md-3 col-lg-2">
                <div class="image-container">
                  <img
                    src="./assets/img/radar.jpeg"
                    alt="release radar thumbnail"
                    class="album-thumbnail"
                  />
                  <div class="overlay">
                    <i class="far fa-play-circle"></i>
                  </div>
                </div>
                <h5>title</h5>
              </div>
              <div class="album-thumbnail text-center col-6 col-md-3 col-lg-2">
                <div class="image-container">
                  <img
                    src="./assets/img/mixdaily.jpeg"
                    alt="daily mix thumbnail"
                    class="album-thumbnail"
                  />
                  <div class="overlay">
                    <i class="far fa-play-circle"></i>
                  </div>
                </div>
                <h5>title</h5>
              </div>
            </div>
            <!-- /seconda row -->

            <!-- Terza row, Artisti popolari -->
            <h2>Artisti pi?? popolari</h2>
            <h6 class="font-spotifygrey">
              Pi?? ascolti, pi?? accurati saranno i suggerimenti.
            </h6>
            <div class="row pb-5">
              <div class="album-thumbnail text-center col-6 col-md-3 col-lg-2">
                <div class="image-container">
                  <img
                    src="./assets/img/youg.jpeg"
                    alt="release radar thumbnail"
                    class="album-thumbnail circle"
                  />
                  <div class="overlay circle">
                    <i class="far fa-play-circle"></i>
                  </div>
                </div>
                <h5>title</h5>
                <h6 class="font-spotifygrey">subtitle</h6>
              </div>
              <div class="album-thumbnail text-center col-6 col-md-3 col-lg-2">
                <div class="image-container">
                  <img
                    src="./assets/img/einaudi.jpeg"
                    alt="ludovico einaudi portrait"
                    class="album-thumbnail circle"
                  />
                  <div class="overlay circle">
                    <i class="far fa-play-circle"></i>
                  </div>
                </div>
                <h5 id="einaudi">title</h5>
                <h6 class="font-spotifygrey">subtitle</h6>
              </div>
            </div>
            <!-- /Terza row -->
          </div>
        </div>
      </div>
    </main>
    <!-- /MACRO-SEZIONE MAIN -->

    <script src="./assets/main.js"></script>
  </body>
</html>
