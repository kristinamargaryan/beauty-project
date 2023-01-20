<template>
  <nav class="navbar navbar-expand-lg custom-navbar-styles">
    <div class="navbar-container">
      <div>
        <img src="@/assets/logo.svg" alt="" />
      </div>
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav me-auto mb-2 mb-lg-0">
          <li class="nav-item">
            <div
              class="nav-link navbar-pages"
              aria-current="page"
              @click="showHomePage"
            >
              Home
            </div>
          </li>
          <li class="nav-item">
            <div
              class="nav-link navbar-pages"
              aria-current="page"
              @click="showAboutPage"
            >
              About
            </div>
          </li>
          <li class="nav-item">
            <div class="nav-link navbar-pages" @click="showServicesPage">
              Services
            </div>
          </li>
          <li class="nav-item">
            <div class="nav-link navbar-pages" @click="showProductPage">
              Product
            </div>
          </li>
          <li class="nav-item">
            <div class="nav-link navbar-pages" @click="showContactPage">
              Contact
            </div>
          </li>
          <!-- <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
            Dropdown
          </a>
          <ul class="dropdown-menu">
            <li><a class="dropdown-item" href="#">Action</a></li>
            <li><a class="dropdown-item" href="#">Another action</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="#">Something else here</a></li>
          </ul>
        </li> -->
          <!-- <li class="nav-item">
          <a class="nav-link disabled">Disabled</a>
        </li> -->
        </ul>
      </div>
      <div>
        <form class="d-flex" role="search">
          <!-- <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search"> -->
          <button class="btn" type="submit">
            <img src="@/assets/search.svg" alt="search" class="navbar-icons" />
          </button>
          <button class="btn more-btn" type="submit">
            <img src="@/assets/menu.svg" alt="manu" class="navbar-icons" />
          </button>
        </form>
      </div>
    </div>
  </nav>
</template>
<script>
export default {
  name: "NavManu",
  methods: {
    showAboutPage() {
      this.$router.push({ path: "/about" });
    },
    showHomePage() {
      this.$router.push({ path: "/" });
    },
    showServicesPage() {
      this.$router.push({ path: "/services" });
    },
    showProductPage() {
      this.$router.push({ path: "/products" });
    },
    showContactPage() {
      this.$router.push({ path: "/contact" });
    },
  },
};
</script>
<style>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@100&display=swap");
.navbar-container {
  z-index: 9999;
  max-width: 1920px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 80px;
}
nav {
  padding: 0px !important;
}
.navbar-collapse {
  padding: 0 200px 0 350px;
}
.navbar {
  height: 80px;
  overflow: hidden;
  position: fixed;
  top: 0;
  width: 100%;
}
.navbar-expand-lg {
  padding: 0 207px !important;
}
.navbar-pages {
  cursor: pointer;
  font-style: normal;
  font-weight: 500;
  font-size: 20px;
  line-height: 24px;
  color: #ffffff;
  font-family: "Montserrat";
  padding-right: 35px !important;
  padding-left: 35px !important;
}
.nav-link:hover {
  font-weight: 900 !important;
  color: #ffffff;
}
.nav-link:visited {
  font-weight: 900 !important;
  color: #ffffff;
}
.custom-navbar-styles {
  background-color: #469597;
  padding: 0 200px;
}
/* .navbar-collapse{
 flex-grow: 0 !important;
} */
.more-btn {
  margin-bottom: 5px;
}

@media (max-width: 1760px) {
  .navbar-container {
    max-width: 1760px;
  }
  .navbar-pages {
    padding-right: 25px !important;
    padding-left: 25px !important;
  }
  .navbar-expand-lg {
    padding: 0 150px !important;
  }
  .navbar-icons {
    width: 20px;
  }
  .navbar-pages {
    padding-right: 35px !important;
  }
  .navbar-collapse {
    padding: 0 200px 0 200px;
  }
}

@media (max-width: 1501px) {
  .navbar-container {
    max-width: 1501px;
  }
  .navbar-pages {
    padding-right: 25px !important;
    padding-left: 25px !important;
  }
  .navbar-expand-lg {
    padding: 0 110px !important;
  }
  .navbar-icons {
    width: 20px;
  }
  .navbar-pages {
    padding: 0 40px !important;
  }
  .navbar-collapse {
    padding: 0 100px 0 100px;
  }
}

@media (max-width: 1201px) {
  .navbar-container {
    max-width: 1201px;
  }
  .navbar-pages {
    padding-right: 17px !important;
    padding-left: 17px !important;
  }
  .navbar-icons {
    width: 20px;
  }
}

@media (max-width: 1024px) {
  .navbar-container {
    max-width: 1024px;
    max-height: 500px;
    padding-left: 0;
  }
  .navbar-pages {
    font-size: 16px;
    padding-right: 25px !important;
    padding-left: 25px !important;
  }
  .navbar-expand-lg {
    padding: 0 65px !important;
  }
  .navbar-icons {
    width: 20px;
  }
  .navbar-pages {
    padding: 0 20px !important;
  }
  .navbar-collapse {
    padding: 0 90px 0 90px;
  }
}

@media (max-width: 991px) {
  .navbar-container {
    width: 600px;
  }
  .navbar-icons {
    width: 20px;
  }
}

@media (max-width: 768px) {
  .custom-navbar-styles {
    padding: 0 100px;
  }
  .navbar-icons {
    width: 20px;
  }
  .navbar-expand-lg {
    padding: 0 45px !important;
  }
}

@media (max-width: 320px) {
  .navbar-container {
    width: 320px;
  }
  .navbar-expand-lg {
    padding: 10px !important;;
  }
}
</style>
