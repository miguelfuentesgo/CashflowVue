<template>
  <div class="splashscreen">
    <img src="../../assets/cashflow-icon.svg" alt="logo" />
    <h1>Cash<span>flow</span></h1>
    <h2>Loading...</h2>
  </div>
</template>

<style scoped>
.splashscreen {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 100vh;
  font-family: Arial, Helvetica, sans-serif;
}
h1 {
  color: green;
}

h1 span {
  color: blue;
}

.loading {
  background-color: red;
}
</style>
