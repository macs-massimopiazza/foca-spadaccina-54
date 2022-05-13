<template>
  <div id="app">
    <h1 style="color: aqua;">🥰Viva Classe 54🥰</h1>
    <h3>🐳Che la foca sia sempre con voi🐳</h3>
    <p style="color: blue;">💕I vostri insegnanti e coordinatori: Luca, Gianluca, Alessio e Massimo 💕</p>
    <img src="https://rivistanatura.com/wp-content/uploads/2017/05/narvalo-770x381.jpg" alt="la foca spadaccina">
    <img src="https://www.osservatorioartico.it/wp-content/uploads/2019/01/narvalo-1280x720.jpg" alt="la foca spadaccina">
    <img src="https://www.ilgiornaledeimarinai.it/wp-content/uploads/2013/12/Il-Narvalo.jpg" alt="la foca spadaccina">
    <h3 style="color: greenyellow;">🪐 Qualche parola 🪐</h3>
    <ul>
      <li v-for="(frase, index) in frasi" :key="index">{{ frase.testo}}  <span style="font-style: italic;">  -{{ frase.nome}}</span></li> <span style="font-style: italic;"></span>
    </ul>

    <h3 style="color: blue;">🎼 Colonna sonora offerta da noi sappiamo chi 🎼</h3>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/c-UNbjm0Wyo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      frasi: [
        { testo: "Grazie ragazzi per non aver usato linux durante il corso ✨", nome: "Massimo" },
        { testo: "Manuel, hai pestato i piedi alla persona sbagliata", nome: "Anonimo" },
        { testo: "Apparte i tutor tutto bene", nome: "Michelangelo" },
        { testo: "Mac ha più problemi", nome: "Gisueppe" },
        { testo: "grazie a boolean ho imparato a fare le ricerche su google", nome: "Micaela" },
        { testo: "Aiutooo ho iniziato a programmare qualke gg fa ke mio cuggino mi a insegnato col il blokko note ma come si mettono i stili x favore haiuto", nome: "Marco" },
        { testo: "vogliamo un ad block per boolean", nome: "Angelo" },
        { testo: "Ho avuto un contrattempo, sono entrato per salutare, non posso connettermi… un saluto Massimo e Alessio", nome: "Andrea" },
        { testo: "✨SCUSA GIANLUCAH, POSSO FARTI UNA DOMANDAA_A_A?✨", nome: "Noi sappiamo chi" },
        { testo: "✨ vi vogliamo bene, dai che è venerdì, stasera si sboccia, progetto finale senza di noi è come mangiare la minestra con la forchetta. 130 martin garrix ✨", nome: "Giusteppe Michelangelo Marco Alberto" },
      ]
    }
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}

body {
  background-color: #ff00a6;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
 
}

img {
  width: 600px;
}

li {
  font-size: 20px;
  margin-bottom: 5px
}

h1, h3, img, p, ul {
  margin-bottom: 20px;
}
</style>
