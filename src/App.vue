<template>
  <div id="app">
    <div class="brand"><img src="./assets/imgs/logo.png" /></div>
    <div class="title">
      O AVANÇO REVOLUCIONÁRIO DO PROCESSO DE LIMPEZA DE PELE
    </div>
    <div class="subtitle">
      O melhor aparelho da atualidade para remoção de cravos e espinhas por
      sucção!
    </div>
    <div class="btn" v-on:click="onPress">PEÇA agora</div>
    <div class="video-wrapper">
      <video autoplay loop muted>
        <source ref="videoRef" src="./assets/video.mp4" type="video/mp4" />
      </video>
    </div>

    <div class="title">
      Remova cravos e espinhas com facilidade deixando sua pele limpa e macia.
    </div>
    <div class="text">
      Aumenta a circulação sanguínea da pele do rosto estimulando a renovação
      celular.
    </div>
    <div class="btn" v-on:click="onPress">comprar agora</div>
    <img src="./assets/imgs/1.webp" />
    <div class="title">Satisfação 100% garantida</div>

    <div class="text">
      A função de vácuo limpa os poros sujos através da sucção e aumenta a
      circulação sanguínea na pele
    </div>
    <img src="./assets/imgs/3.webp" />

    <div class="title">Cabeça de diamante</div>
    <div class="text">
      Com mais de 100 mil partículas microcristalinas minerais naturais de alta
      absorção, pode esfregar e esfoliar a pele morta e sugá-la, para reparar a
      pele e remover as rugas e acnes sem prejudicar a pele.
    </div>
    <div class="sub-text">
      * Área de uso: Qualquer área do rosto, exceto ao redor dos olhos. Adequado
      para áreas com rugas como cotovelo, joelho e tornozelo.
    </div>

    <div class="title">Cabeça circular grande</div>
    <div class="text">
      Com forte sucção, pode remover a cravos de forma eficaz, promovendo o
      sangue e a circulação linfática, deixando a pele rejuvenescer novamente.
    </div>
    <div class="sub-text">
      * Área de uso: Qualquer área do rosto, exceto em torno dos olhos.
    </div>

    <div class="title">Cabeça circular pequeno</div>
    <div class="text">
      A sucção é fraca, que pode ser usada para remover cravos em áreas
      sensíveis.
    </div>
    <div class="sub-text">
      * Área de uso: Pode ser usado em áreas sensíveis com o redor dos olhos.
    </div>

    <div class="title">Cabeça oval</div>
    <div class="text">
      Pele reafirmante, removendo rugas finas, aumentando a elasticidade da
      pele. Adequado para o canto da boca e outras áreas onde é fácil ter linhas
      finas para evitar o crescimento de rugas.
    </div>
    <div class="sub-text">
      * Área de uso: Pode ser usado em áreas sensíveis como ao redor dos olhos e
      o canto da boca.
    </div>

    <div class="video-wrapper">
      <video controls>
        <source ref="videoRef" src="./assets/youtube.mp4" type="video/mp4" />
      </video>
    </div>
    <div style="margin-bottom: 10px" />
    <div class="sale">
      <div class="title" style="font-weigth: bold">
        PEÇA AGORA O SEU DERMA SUCTION
      </div>
      <div class="old-price">R$ 139,00</div>
      <div>por apenas</div>
      <div class="new-price">12x R$ 8,44</div>
      <img src="./assets/imgs/4.webp" class="img-product" />
      <div
        class="btn"
        onclick="window.open('https://bugibra.pay.yampi.com.br/r/7MNC2NRBBK','mywindow');"
      >
        comprar já
      </div>
      <div style="color: grey; margin-top: -10px">ENVIO IMEDIATO</div>
      <div class="container-selos">
        <img src="./assets/imgs/selo_garantia.png" class="selos" />
        <img src="./assets/imgs/seguro.png" class="selos" />
      </div>
    </div>
    <div class="footer">BugiBra © 2021</div>
  </div>
</template>

<script>
export default {
  name: "App",
  components: {},
  methods: {
    onPress: function () {
      var el = this.$el.getElementsByClassName("sale")[0];
      el.scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>

<style>
/* roboto-slab-regular - latin */
@font-face {
  font-family: "Roboto Slab";
  font-style: normal;
  font-weight: 400;
  src: local(""),
    url("./assets/fonts/roboto-slab-v12-latin-regular.woff2") format("woff2"),
    /* Chrome 26+, Opera 23+, Firefox 39+ */
      url("./assets/fonts/roboto-slab-v12-latin-regular.woff") format("woff"); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}
/* roboto-slab-800 - latin */
@font-face {
  font-family: "Roboto Slab";
  font-style: normal;
  font-weight: 800;
  src: local(""),
    url("./assets/fonts/roboto-slab-v12-latin-800.woff2") format("woff2"),
    /* Chrome 26+, Opera 23+, Firefox 39+ */
      url("./assets/fonts/roboto-slab-v12-latin-800.woff") format("woff"); /* Chrome 6+, Firefox 3.6+, IE 9+, Safari 5.1+ */
}
#app {
  font-family: "Roboto Slab";
  text-align: center;
  color: #2c3e50;
  margin-bottom: 20px;
  margin-top: 100px;
}

.container-selos {
  display: flex;
  justify-content: center;
  align-self: center;
  margin-left: -20px;
  margin-bottom: 20px;
  margin-top: 20px;
}

.footer {
  position: absolute;
  bottom: 20;
  width: 100%;
  left: 0;
  height: 30px;
  background: #4a6eca;
  color: white;
  display: flex;
  justify-content: center;
  align-self: center;
  padding-top: 5px;
}

.title {
  color: #4a6eca;
  font-size: 20px;
  margin-bottom: 20px;
}

.selos {
  height: 100px;
  width: auto;
}

.subtitle {
  margin-bottom: 20px;
}

.brand {
  color: #4a6eca;
  font-size: 26px;
  font-weight: 800;
  margin-bottom: 10px;
  z-index: 99;
  position: fixed;
  width: 100%;
  background: white;

  top: 0;
}

.btn {
  background-color: #75d237;
  border-bottom: 3px solid #5daf27 !important;
  text-transform: uppercase;
  color: white;
  font-weight: 800;
  padding: 20px;
  margin-bottom: 20px;
}

.video-wrapper {
  width: 100%;
  height: 100%;
  margin-bottom: 10px;
}

.video-wrapper video {
  object-fit: cover;
  width: 100%;
}

img {
  max-width: 100%;
  height: auto;
}

.text {
  text-align: justify;
  margin-bottom: 20px;
}

.old-price {
  text-decoration: line-through;
  color: grey;
  font-size: 34px;
}

.new-price {
  color: #5daf27;
  font-size: 34px;
}

.img-product {
  height: 235px;
}

.logo {
  height: 50px;
}

.sub-text {
  color: grey;
  font-size: 14px;
  text-align: justify;
  margin-bottom: 30px;
  padding-bottom: 10px;
}
</style>
