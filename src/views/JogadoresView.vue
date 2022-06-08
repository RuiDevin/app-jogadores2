<script>
export default {
  data() {
    return {
      jogadores: [
        { id: 1, name: "Jogador 1" },
        { id: 2, name: "Jogador 2" },
        { id: 3, name: "Jogador 3" },
        { id: 4, name: "Jogador 4" },
      ],
    };
  },
};
</script>

<template>
  <main id="main">BEM VINDO TIME</main>
  <div class="container">
    <h2>Gerenciamento de jogadores</h2>
  </div>
  <div class="form-input">
    <input type="text" />
    <button>Salvar</button>
  </div>
  {{ jogadores }}
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
          <td>1</td>
          <td>Time 1</td>
          <td>???</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<style scoped></style>
