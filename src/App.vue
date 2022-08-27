<template>
  <div id="app" class="container">
    <router-view />
  </div>
</template>

<style lang="scss">
@import "../node_modules/bootstrap/scss/bootstrap.scss";

#app {
  text-align: center;
  margin-top: 16px;
}

// dark theme colors
@media (prefers-color-scheme: dark) {
  // global app colors
  body {
    background-color: black;
  }
  #app {
    color: #dedad6;
  }

  // navbar colors
  .navbar.bg-light {
    background-color: rgb(33, 37, 41) !important;
    border-bottom: 1px solid #8a8a8a !important;
  }
  .navbar .navbar-brand {
    color: #fff;
  }
  .navbar .navbar-nav .nav-link {
    color: rgba(255, 255, 255, 0.55);
  }
  .navbar .navbar-nav .nav-link:focus,
  .navbar .navbar-nav .nav-link:hover {
    color: rgba(255, 255, 255, 0.75);
  }
  .navbar .navbar-nav .nav-link.active {
    color: #fff;
  }
  .navbar-light .navbar-brand:hover {
    color: #fff;
  }
  .dropdown-menu {
    color: #dee2e6;
    background-color: #343a40;
    border-color: rgba(0, 0, 0, 0.15);
  }
  .dropdown-menu .dropdown-item {
    color: #dee2e6;
  }
  .dropdown-menu .dropdown-item:focus:not(.active),
  .dropdown-menu .dropdown-item:hover:not(.active) {
    color: #fff;
    background-color: rgba(255, 255, 255, 0.15);
  }

  // button colors
  .btn-primary {
    background-color: #004dbf;
    border-color: #125cc8;
  }
  .btn-secondary {
    background-color: #484e53;
    border-color: #555d64;
  }
  .btn-outline-secondary {
    color: #909ca6;
    border-color: #909ca6;
  }

  // table colors
  .table {
    border-color: #75787b;
  }
  .table-striped > tbody > tr:nth-of-type(2n + 1) {
    background-color: #222;
  }

  // form control colors
  .form-control {
    background-color: rgba(0, 0, 0, 0);
    border-color: #83888c;
    color: #dedad6;

    &::placeholder {
      color: #8e8e8e;
    }
  }
  .form-control:focus {
    background-color: rgba(0, 0, 0, 0);
    color: #dedad6;
    border-color: #125cc8;
  }
}
</style>
