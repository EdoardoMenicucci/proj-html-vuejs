<!-- COMPONENTE SINGOLO -->
<script>
// SCRIPT
export default {
  data() {
    return {
      logo: 'img/theme_eduprime_logo.png',
      bgHeader: 'img/hero.png',
      jumboDesc: 'EduPrime is the most versatile WordPress theme for educational purposes, showcasing universities, courses, secondary schools etc.',
      wave: '/img/Wave-1.png'
    }
  },
  methods: {

  },
  mounted() {

  },
}
</script>

<template>
  <!-- TEMPLATE html-->
  <div class="gradient-header"></div>
  <div class="container-header">
    <!-- SEZIONE HEADER -->
    <header class="p-4 d-flex justify-content-between align-items-center round-font">
      <div>
        <img class="logo" :src="logo" alt="">
      </div>
      <div class="left">
        <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
          <div class="container-fluid">

            <div class="collapse navbar-collapse" id="navbarNavDarkDropdown">
              <ul class="navbar-nav">
                <li class="nav-item dropdown">
                  <button class="btn btn-dark dropdown-toggle round-font" data-bs-toggle="dropdown"
                    aria-expanded="false">
                    Home
                  </button>
                  <ul class="dropdown-menu dropdown-menu-dark">
                    <li><a class="dropdown-item" href="#">Action</a></li>
                    <li><a class="dropdown-item" href="#">Another action</a></li>
                    <li><a class="dropdown-item" href="#">Something else here</a></li>
                  </ul>
                </li>
              </ul>
            </div>

            <div class="collapse navbar-collapse" id="navbarNavDarkDropdown">
              <ul class="navbar-nav">
                <li class="nav-item dropdown">
                  <button class="btn btn-dark dropdown-toggle round-font" data-bs-toggle="dropdown"
                    aria-expanded="false">
                    Courses
                  </button>
                  <ul class="dropdown-menu dropdown-menu-dark">
                    <li><a class="dropdown-item" href="#">Action</a></li>
                    <li><a class="dropdown-item" href="#">Another action</a></li>
                    <li><a class="dropdown-item" href="#">Something else here</a></li>
                  </ul>
                </li>
              </ul>
            </div>

            <a class="navbar-brand" href="#">About Us</a>

            <div class="collapse navbar-collapse" id="navbarNavDarkDropdown">
              <ul class="navbar-nav">
                <li class="nav-item dropdown">
                  <button class="btn btn-dark dropdown-toggle round-font" data-bs-toggle="dropdown"
                    aria-expanded="false">
                    News
                  </button>
                  <ul class="dropdown-menu dropdown-menu-dark">
                    <li><a class="dropdown-item" href="#">Action</a></li>
                    <li><a class="dropdown-item" href="#">Another action</a></li>
                    <li><a class="dropdown-item" href="#">Something else here</a></li>
                  </ul>
                </li>
              </ul>
            </div>

            <div class="collapse navbar-collapse" id="navbarNavDarkDropdown">
              <ul class="navbar-nav">
                <li class="nav-item dropdown">
                  <button class="btn btn-dark dropdown-toggle round-font" data-bs-toggle="dropdown"
                    aria-expanded="false">
                    Pages
                  </button>
                  <ul class="dropdown-menu dropdown-menu-dark">
                    <li><a class="dropdown-item" href="#">Action</a></li>
                    <li><a class="dropdown-item" href="#">Another action</a></li>
                    <li><a class="dropdown-item" href="#">Something else here</a></li>
                  </ul>
                </li>
              </ul>
            </div>

            <a class="navbar-brand" href="#">Contact</a>

            <a class="navbar-brand" href="#">Purchase</a>

            <button class="button ms-3">VIEW COURSES</button>

          </div>
        </nav>
      </div>
    </header>
    <!-- FINE NAVBAR -->
    <!-- INIZIO JUMBOTRON -->
    <div class="jumbo d-flex flex-columns align-items-center ">
      <h1 class="round-font pb-5 pt-5">Showcase your courses</h1>
      <p>{{ jumboDesc }}</p>
      <div>
        <button class="button round-font"><i class="fa-solid fa-magnifying-glass"></i> Search courses</button>
        <button class="button-white round-font ms-4">Apply for university</button>
      </div>
    </div>
  </div>
  <div class="bg-red">
    <img class="wave" :src="wave" alt="">
  </div>

</template>

<!-- CON SCOPED DICHIARO CSS SOLO AL ATTUALE COMPONENTE/file -->
<style scoped>
/* STILE */


* {
  font-size: 1.2rem;
}

.gradient-header {
  height: 40rem;
  width: 100%;
  position: absolute;
  top: 0;
  left: 0;
  background: rgb(2, 0, 36);
  background: linear-gradient(180deg, rgba(2, 0, 36, 0) 78%, rgba(209, 94, 94, 1) 98%);
}

.container-header {
  height: 40rem;
  background-image: url(../../img/hero.png);
  background-size: cover;
  background-position: bottom;
}

.logo {
  height: 4rem;
}

button {
  font-size: 1.2rem !important;
}

button:hover {
  color: #e9d758;
}

h1 {
  font-size: 4rem;
}

.bg-red {
  background-color: #d15e5e;
}

.button {
  padding: 16px 43px !important;
  background-color: #e9d758;
  color: #fff;
  border-radius: 32px;
  border: transparent;
  font-weight: 600;
  transition: 0.3s ease;
}

.button-white {
  padding: 16px 43px !important;
  background-color: transparent;
  color: #fff;
  border-radius: 32px;
  border: 1px solid white;
  font-weight: 600;
  transition: 0.3s ease;
}

.button-white:hover {
  padding: 16px 43px !important;
  background-color: #e9d758;
  color: #fff;
  border-radius: 32px;
  border: transparent;
  font-weight: 600;
}

.button:hover {
  padding: 16px 43px !important;
  background-color: transparent;
  color: #fff;
  border-radius: 32px;
  border: 1px solid white;
  font-weight: 600;
}

.navbar {
  background-color: rgba(0, 0, 0, 0) !important;
}

.btn {
  background-color: rgba(0, 0, 0, 0);
  border: transparent;
}

.wave {
  object-fit: cover;
  width: 100%;
  height: 3rem;
  opacity: 1;
}

.jumbo {
  height: 100%;
  width: 30%;
  margin: 0 auto;
  text-align: center;
}

.flex-columns {
  flex-direction: column;
}
</style>
