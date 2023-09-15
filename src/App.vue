<script setup>
</script>

<template>
<main>
  <div class="titulo">
    <h1>Lista de afazeres</h1>
  </div>
  <div class="formulario">
    <input 
    type="text" 
    class="texto"
    placeholder="Insira sua nova tarefa...">
    <button type="submit">Enviar</button>
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
  width: 400px;
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
  width: 400px;
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

.formulario > button {
  width: 60px;
  height:  30px;
  border-radius: 10px;
  background-color: var(--laranja-fab);
  border: none;
  color: var(--branco-fab);
  font-weight: bold;
}
.formulario > button:hover {
  background-color: var(--laranja-escuro)
}

</style>
