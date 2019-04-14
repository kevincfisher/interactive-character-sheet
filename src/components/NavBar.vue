<template>
    <nav role="navigation" class="navbar is-primary">
        <div class="navbar-brand">
            <a class="navbar-item" href="/">
                <img src="../assets/logo.png">
            </a>

            <a role="button" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navBar">
              <span aria-hidden="true"></span>
              <span aria-hidden="true"></span>
              <span aria-hidden="true"></span>
            </a>
        </div>
        <div id="navBar" class="navbar-menu">
            <div class="navbar-start">
                <a class="navbar-item">
                    Stats
                </a>
                <a class="navbar-item">
                    Background
                </a>
                <a class="navbar-item">
                    Notes
                </a>
            </div>
        </div>
    </nav>
</template>

<script>
    export default {
        name: 'NavBar',
        mounted() {
            // Get all "navbar-burger" elements
          const $navbarBurgers = Array.prototype.slice.call(document.querySelectorAll('.navbar-burger'), 0);

           // Check if there are any navbar burgers
          if ($navbarBurgers.length > 0) {

          // Add a click event on each of them
          $navbarBurgers.forEach( el => {
          el.addEventListener('click', () => {

          // Get the target from the "data-target" attribute
          const target = el.dataset.target;
          const $target = document.getElementById(target);

          // Toggle the "is-active" class on both the "navbar-burger" and the "navbar-menu"
          el.classList.toggle('is-active');
          $target.classList.toggle('is-active');
      });
    });
  }

        }
    }
</script>

<style>
    .navbar {
        margin-bottom: 1em;
    }
</style>