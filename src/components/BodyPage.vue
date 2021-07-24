<template>
    <main class="main">
      <div class="box" id="1"></div>
      <div class="box" id="2"></div>
      <div class="box" id="3"></div>
      <div class="box" id="4"></div>
      <div class="box" id="5"></div>
      <div class="box" id="6"></div>
      <div class="box" id="7"></div>
      <div class="box" id="8"></div>
      <div class="box" id="9"></div>
      <div class="box" id="10"></div>
      <div class="box" id="11"></div>
      <div class="box" id="12"></div>
      <div class="box" id="13"></div>
      <div class="box" id="14"></div>
      <div class="box" id="15"></div>
      <div class="box" id="16"></div>
      <div class="box" id="17"></div>
      <div class="box" id="18"></div>
      <div class="box" id="19"></div>
      <div class="box" id="20"></div>
      <div class="box" id="21"></div>
      <div class="box" id="22"></div>
      <div class="box" id="23"></div>
      <div class="box" id="24"></div>
      <div class="box" id="25"></div>
      <div class="box" id="26"></div>
      <div class="box" id="27"></div>
      <div class="box" id="28"></div>
      <div class="box" id="29"></div>
      <div class="box" id="30"></div>
      <div class="box" id="31"></div>
      <div class="box" id="32"></div>
      <div class="box" id="33"></div>
      <div class="box" id="34"></div>
      <div class="box" id="35"></div>
    </main>
    <button class="btn__send">Enviar Datos</button>
    <button class="btn__clear">
      <p>Limpiar</p>
     <!--  <img src="../assets/trash-icon.png" alt="Resetear valores"/> -->
    </button>
</template>

<script>
/* aqui van weas de javascript */
</script>


<style>
:root {
  --text-color: #f4f4f4;
  --title-color: #dfdfdf;
  --dark-color: #121212;
  --border-color: #242424;
  --white-color: #dedede;

  --border-color-h: #242424e0;
  --white-color-h: #dededee0;
  --opacity-color: #000000d0;
}

body {
  display: flex;
  flex-direction: column;
  justify-content: center;
  background: rgb(100, 149, 209);
  background: linear-gradient(90deg, rgba(100, 149, 209, 1) 0%, rgba(35, 35, 140, 1) 50%, rgba(255, 204, 0, 1) 100%);
  font-family: 'Roboto', sans-serif;
}
main {
  margin: 20px;
  min-height: 70vh;
  display: grid;
  justify-content: center;
  align-content: center;
  grid-template: repeat(7, minmax(48px, 88px))/ repeat(5, minmax(48px, 88px));
  font-family: 'Roboto', sans-serif;
}
.box {
  box-shadow: rgba(0, 0, 0, 0.25) 0px 54px 55px, rgba(0, 0, 0, 0.12) 0px -12px 30px, rgba(0, 0, 0, 0.12) 0px 4px 6px, rgba(0, 0, 0, 0.17) 0px 12px 13px, rgba(0, 0, 0, 0.09) 0px -3px 5px;
  border-color: var(--border-color);
  border-style: solid;
  background: var(--text-color);
  cursor: pointer;
}

.box.active {
  background: var(--border-color);
}

.box:hover {
  opacity: 0.8;
}

.title {
  width: 100%;
  color: var(--title-color);
  margin-top: 20px;
  font-size: calc(1.725vw + 2.725vh);
  font-weight: bold;
  text-align: center;
}

.btn__send {
  cursor: pointer;
  margin: 2rem;
  padding: 1rem;
  align-self: center;
  border-style: none;
  border-radius: 8px;
  box-shadow: rgba(50, 50, 93, 0.25) 0px 2px 5px -1px, rgba(0, 0, 0, 0.3) 0px 1px 3px -1px;
  max-width: 80vw;
  width: 80%;
  min-height: 48px;
  background: 4px 8px rgb(100, 149, 209);
  font-size: calc(1.2vw + 2.8vh);
  letter-spacing: 3px;
  color: var(--text-color);
  font-weight: bold;
}

.btn__send:hover {
  opacity: 0.8;
}

.btn__clear {
  cursor: pointer;
  margin: 2rem;
  border-style: none;
  color: var(--text-color);
  padding: 0.5rem;
  align-items: center;
  align-self: center;
  border-radius: 20px;
  box-shadow: rgba(50, 50, 93, 0.25) 0px 2px 5px -1px, rgba(0, 0, 0, 0.3) 0px 1px 3px -1px;
  width: calc(14vw + 2vmax);
  height: calc(7vw + 2vmax);
  min-width: 120px;
  min-height: 40px;
  max-width: 240px;
  max-height: 100px;
  text-align: center;
  background: 4px 8px rgb(100, 149, 209);

}

.btn__clear p {
  font-size: calc(1.2vw + 1.8vh);
}

.btn__clear img {
  width: calc(3vw + 1.5vh);
  height: calc(3vw + 1.5vh);
}

.btn__clear > * {
  padding: 0.5rem;
}

.btn__clear:hover {
  opacity: 0.8;
}

</style>
