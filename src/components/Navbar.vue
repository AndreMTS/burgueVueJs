<template>
  <header>
    <div class="wrapper">
      <nav>
         <RouterLink to="/" id="logo-url">
          <img v-bind:src="logo" v-bind:alt="alt" id="logo">
         </RouterLink>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/pedidos">Pedidos</RouterLink>
      </nav>
    </div>
  </header>
</template>

<script>

export default {
  name: "Navbar",
  props:['logo','alt']
};
</script>

<style scoped>
nav{
  background-color: #222;
  border-bottom:4px solid #111;
  padding:15px 50px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}
nav #logo-url{
  margin: auto;
  margin-left: 0;
}
#logo{
  width: 40%;
  height: 40%;
}
nav a {
  color:rgb(153, 87, 0);
  text-decoration: none;
  margin: 12px;
  transition: .5s;
}
nav a:hover {
  color:rgb(255, 255, 255);
}
</style>