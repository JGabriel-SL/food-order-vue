<script setup lang="ts">
import TheWelcome from '@/components/TheWelcome.vue'
</script>

<template>
  <div>
    <!-- <div class="principal-section ">
      <img src="../assets/wallpaper1.png" />
    </div> -->

    <div class="principal-section ">
      <div class="title-container">
        <h1>GABSFOOD</h1>
        <p class="text-center">Monte do jeitinho que você gosta!</p>
        <button class="btn-ordernow">Faça ja o seu pedido!</button>
      </div>
      <img src="../assets/hamburger.png" />
      <img class="duplicated-image" src="../assets/hamburger.png" />
    </div>  

  </div>
</template>

<style scoped>


@media (max-width: 1024px) {
  .principal-section {
    flex-direction: column;
  }

  .duplicated-image {
    display: none;
  }

  .title-container h1 {
    font-size: 2.5rem !important;
  }

  .title-container {
    padding: 0px !important;
  }

  .principal-section button {
    margin-bottom: 40px;
  }
  .principal-section img {
    width: 80% !important;
    display: none;
  } 
}

.principal-section {
  width: 100%;
  height: 80vh;

  display: flex;
  justify-content: center;
  align-items: center;

}

.title-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 0px 5rem;
}

.title-container h1{
  font-size: 50px;
  letter-spacing: 10px;
  color: #FFF;
}

.principal-section img {
  width: 40%;
  margin: 0 auto;
}

.principal-section .duplicated-image {
  margin-left: -40%;
  margin-top: 5%;
}

.btn-ordernow {
  margin-top: 20px;
  border: 0;
  border-radius: 10px;
  
  padding: 10px 20px;

  color: #FFF;
  background-color: #c90a00e1;
  font-weight: bold;
  transition: 0.5s;

  cursor: pointer;
}

.btn-ordernow:hover {
  background-color: #910902e0;
  background-color: #FFF;
  color:#c90a00e1;
}

</style>
