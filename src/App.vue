<template>
  <header class="menu-superior">
    <div class="Menu Esquerdo">
      <span><RouterLink to="/players">jogadores</RouterLink> </span>
      <span><RouterLink to="/times">times</RouterLink> </span>
      <span><RouterLink to="/">Home</RouterLink> </span>
    </div>

    <div class="Menu Direito">
      <span>Sair</span>
    </div>
  </header>

  <RouterView />

  <footer id="footer">footer</footer>
</template>

<style>
@import "@/assets/base.css";

#app {
  font-size: 16px;
  height: 100vh;
  width: 100vw;

  font-weight: normal;
}

header,
footer {
  background-color: rgb(59, 59, 127);
  color: white;
  height: 15%;
  font-size: 1.3rem;
  display: flex;
  align-items: center;
  padding-left: 2rem;
}

header span {
  padding: 0 20px;
}

header.menu-superior {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

main {
  height: 70%;
}
</style>
