<template>
  <v-app>
    <v-main class="mb-4">
      <vue-particles
              class="particles"
              color="#A9A9A9"
              :particleOpacity="0.7"
              :particlesNumber="80"
              shapeType="circle"
              :particleSize="4"
              linesColor="#A9A9A9"
              :linesWidth="1"
              :lineLinked="true"
              :lineOpacity="0.4"
              :linesDistance="150"
              :moveSpeed="3"
              :hoverEffect="false"
              :clickEffect="false"
      >
      </vue-particles>
      <v-container
              class="fill-height"
              fluid
      >
        <v-row
                align="center"
                justify="center"
                class="mb-3"
        >
          <Posts/>
        </v-row>
      </v-container>
    </v-main>
    <v-footer
            absolute
            padless
    >
      <v-card
              class="flex"
              flat
              tile
      >

        <v-card-text class="grey darken-4 white--text text-right fnt-vaz">
          به خودت ایمان بیار، تو میتونی
          <p class="float-left">میم</p>
        </v-card-text>
      </v-card>
    </v-footer>
  </v-app>
</template>

<script>
  import Posts from './components/Posts'

  export default {
    name: 'App',

    components: {
      Posts,
    },

    data: () => ({
      //
    }),
  };
</script>
<style>
  @font-face {
    font-family: Vazir;
    src: url('/fonts/vazir/Vazir.eot');
    src: url( '/fonts/vazir/Vazir.eot?#iefix') format('embedded-opentype'),
    url( '/fonts/vazir/Vazir.woff2') format('woff2'),
    url( '/fonts/vazir/Vazir.woff') format('woff'),
    url( '/fonts/vazir/Vazir.ttf') format('truetype');
    font-weight: normal;
    font-style: normal;
  }
  @font-face {
    font-family: Vazir;
    src: url( '/fonts/vazir/Vazir-Bold.eot');
    src: url( '/fonts/vazir/Vazir-Bold.eot?#iefix') format('embedded-opentype'),
    url( '/fonts/vazir/Vazir-Bold.woff2') format('woff2'),
    url( '/fonts/vazir/Vazir-Bold.woff') format('woff'),
    url( '/fonts/vazir/Vazir-Bold.ttf') format('truetype');
    font-weight: bold;
    font-style: normal;
  }
  @font-face {
    font-family: Vazir;
    src: url( '/fonts/vazir/Vazir-Black.eot');
    src: url( '/fonts/vazir/Vazir-Black.eot?#iefix') format('embedded-opentype'),
    url( '/fonts/vazir/Vazir-Black.woff2') format('woff2'),
    url( '/fonts/vazir/Vazir-Black.woff') format('woff'),
    url( '/fonts/vazir/Vazir-Black.ttf') format('truetype');
    font-weight: 900;
    font-style: normal;
  }
  @font-face {
    font-family: Vazir;
    src: url( '/fonts/vazir/Vazir-Medium.eot');
    src: url( '/fonts/vazir/Vazir-Medium.eot?#iefix') format('embedded-opentype'),
    url( '/fonts/vazir/Vazir-Medium.woff2') format('woff2'),
    url( '/fonts/vazir/Vazir-Medium.woff') format('woff'),
    url( '/fonts/vazir/Vazir-Medium.ttf') format('truetype');
    font-weight: 500;
    font-style: normal;
  }
  @font-face {
    font-family: Vazir;
    src: url( '/fonts/vazir/Vazir-Light.eot');
    src: url( '/fonts/vazir/Vazir-Light.eot?#iefix') format('embedded-opentype'),
    url( '/fonts/vazir/Vazir-Light.woff2') format('woff2'),
    url( '/fonts/vazir/Vazir-Light.woff') format('woff'),
    url( '/fonts/vazir/Vazir-Light.ttf') format('truetype');
    font-weight: 300;
    font-style: normal;
  }
  @font-face {
    font-family: Vazir;
    src: url( '/fonts/vazir/Vazir-Thin.eot');
    src: url( '/fonts/vazir/Vazir-Thin.eot?#iefix') format('embedded-opentype'),
    url( '/fonts/vazir/Vazir-Thin.woff2') format('woff2'),
    url( '/fonts/vazir/Vazir-Thin.woff') format('woff'),
    url( '/fonts/vazir/Vazir-Thin.ttf') format('truetype');
    font-weight: 100;
    font-style: normal;
  }
  .fnt-vaz{
    font-family: Vazir,sans-serif;
  }
  .particles {
    position: absolute;
    left: 0;
    right: 0;
    top: 0;
    bottom: 0;
  }
</style>
