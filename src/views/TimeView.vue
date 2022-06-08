<script>
 export default {
 data(){
     return {
       times: [
         {id: 1, name: "Time 1"},
         {id: 2, name: "Time 2"},
         {id: 3, name: "Time 3"},
         {id: 4, name: "Time 4"},
         
       ],
     };
   },
 };
</script>

<template>
  <main id="main">BEM VINDO TIME</main>
  <div class = "container">
  <h2>Gerenciamento de time</h2>
  </div>
  <div class="form-input">
    <input type="text" placeholder="Nome">
    <input type="text" placeholder="Time">
    <button>Salvar</button>
  </div>
  {{times}} 
  <div class="list-times">
    <table>
      <thead>
      <tr>
      <th>ID</th>
      <th>Nome</th>
      <th>Açoẽs</th>
      </tr>
      </thead>
      <tbody>
        <tr v-for="time in times" :key="time.id">
        <td>{{time.id}}</td>
        <td>{{time.name}}</td>
        <td>???</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>


