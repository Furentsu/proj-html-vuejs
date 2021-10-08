<template>
  <header>

    <!-- Logo -->
    <div class="logo-container">
      <img src="../assets/images/construction_logo_retina.png" alt="Avada Construction's logo">
    </div>

    <!-- Navbar -->
    <nav>
      <ul>
        <li v-for="(element,index) in headerNav" :key="index">
          <a href="#">{{headerNav[index].text}}</a>
        </li>
      </ul>
    </nav>

    <!-- Get quote button -->
    <div class="call-to-action">
      <button>Get quote</button>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data() {
    return {
      headerNav: [
        {
            text: "home",
        },
        {
            text: "about",
        },
        {
            text: "services",
        },
        {
            text: "work",
        },
        {
            text: "articles",
        }
      ]
    }
  }
}
</script>


<style lang="scss" scoped>
@import "../style/variables.scss";

header {
      display: flex;
      align-items: center;
      height: 100px;

// LOGO CONTAINER
    .logo-container {
      display: flex;
      justify-content: center;
      align-items: center;
      width: 20%;
      height: 100%;

      img {
        width: 150px;
      }
    }

// NAVIGATION MENU
    nav {
      width: 60%;
      height: 100%;

      ul {
        display: flex;
        justify-content: right;
        height: 100%;
        align-items: center;
        list-style: none;

          li {
            text-transform: uppercase;
            font-size: .8rem;

              a {
                text-decoration: none;
                color: $doveGrey;
                margin: 0 0 0 25px;

                &:hover {
                  color: $brightSun;
                }
              }
          }
      }
    }

// QUOTE BUTTON

.call-to-action {
  display: flex;
  flex-grow: 1;
  justify-content: center;

  button {
      border: none;
      padding: 8px 30px;
      text-transform: uppercase;
      font-size: .8rem;
      background-color: $brightSun;
      color: $doveGrey;

      &:hover {
        color: $primaryWhite;
        background-color: $codGrey;

      }
    }
}
}
</style>
