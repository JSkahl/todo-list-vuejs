<script>

export default {
  data() {
    return {
      mostrarTarefa: false
    };
  },
  methods: {
    adicionarTarefa() {
      this.mostrarTarefa = true;
    }
  }
};

</script>

<template>
<main>
  <div class="titulo">
    <h1>Lista de tarefas</h1>
  </div>
  <div class="formulario">
    <input 
    type="text" 
    class="texto"
    placeholder="Insira sua nova tarefa...">
    <button @click="adicionarTarefa">Enviar</button>
    
  </div>

  <div class="adicionarTarefa">
    <input type="checkbox">

    <div class="textoTarefa">
      <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit.</p>
    </div>

    <div class="botoesTarefa">
      <button class="apagarTarefa">Apagar</button>
      <button class="editarTarefa">Editar</button>
    </div>

  </div>

</main>
</template>

<style scoped>

main {
  width: 400px;
  height: 500px;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: auto;
  margin-top: 100px;
}

.titulo {
  background-color: var(--cinza-fab);
  width: 500px;
  height: 40px;
  display: flex;
  border-radius: 15px 15px 0px 0px;
  box-shadow: 0px 0px 10px 3px rgba(0,0,0,0.75);
}

.titulo > h1 {
  margin: auto;
  font-size: x-large;
}

.formulario {
  width: 500px;
  height: 70px;
  background-color: var(--branco-fab);
  display: flex;
  justify-content: space-evenly;
  border-radius: 0px 0px 15px 15px;
  align-items: center;
  box-shadow: 0px 8px 10px 3px rgba(0,0,0,0.75);
}

.formulario > input {
  border: 2px var(--laranja-fab) solid;
  border-radius: 10px;
  width: 250px;
  height: 30px;
  outline: none;
  padding: 0px 10px 0px 10px
}

.formulario > input:hover {
  background-color: var(--branco-fab);
}

button {
  width: 60px;
  height:  30px;
  border-radius: 10px;
  background-color: var(--laranja-fab);
  border: none;
  color: var(--branco-fab);
  font-weight: bold;
}

button:hover {
  background-color: var(--laranja-escuro)
}

.adicionarTarefa {
  width: 500px;
  height: 80px;
  background-color: var(--branco-fab);
  margin-top: 10px;
  border-radius: 15px;
  display: flex;
  flex-direction: col;
  font-size: 15px;
  box-shadow: 0px 0px 20px 0px rgba(0,0,0,0.75);
}

.textoTarefa {

  width: 400px;
  height: 74px;
  margin: auto;
  margin: auto 10px auto 10px;
}

.botoesTarefa {
  display: flex;
  margin: auto;
  margin-right: 10px;
  flex-direction: column;
}

.botoesTarefa > button {
  margin: 5px;
}

.editarTarefa {
  background-color: var(--ciano-fab);
}

.editarTarefa:hover {
  background-color: var(--ciano-escuro);
}

.apagarTarefa {
  background-color: var(--vermelho-fab);
}

.apagarTarefa:hover {
  background-color: var(--vermelho-escuro);
}

.adicionarTarefa > input {
  width: 20px;
  margin-left: 10px;
}

</style>
