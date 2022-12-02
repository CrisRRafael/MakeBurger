<template>
  <div id="main-burger">
    <h1>Make Your Burger</h1>
  </div>
</template>

<script>
export default {
  name: "Banner",
};
</script>

<style scoped>
#main-burger {
  background-image: url("../assets/burger.jpg");

  background-position: 0 -280px;
  background-size: cover;
  height: 580px;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}

#main-burger h1 {
  color: #fff;
  text-align: center;
  font-size: 60px;
  background-color: #222;
  padding: 20px 40px;

  border-radius: 0 25px 25px 0;
}
</style>
