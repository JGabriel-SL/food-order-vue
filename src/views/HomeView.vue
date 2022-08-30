<script lang="ts">
  import CardExamples from '@/components/CardExamples.vue'

  export default {
    name: 'HomeView',
    components: {
      CardExamples
    }
  }
</script>

<template>
  <div>
    <!-- <div class="principal-section ">
      <img src="../assets/wallpaper1.png" />
    </div> -->

    <div class="principal-section ">
      <div class="title-container">
        <h1>GABS<img src="@/assets/newlogo.svg"/>FOOD</h1>
        <p class="text-center">Monte do jeitinho que você gosta!</p>
        <button class="btn-ordernow">Faça ja o seu pedido!</button>
      </div>
      <img src="../assets/hamburgers.png" />

    </div>  
    <h1 class="title-section">APROVEITE JÁ</h1>
    <div class="examples-section"> 
      <CardExamples />     
      <CardExamples />     
      <CardExamples />     
    </div>
    <div class="transition-section"></div>
    <div class="principal-section"></div>
  </div>
</template>

<style scoped>

.principal-section {
  margin-top: 50px;
  width: 100%;
  height: 80vh;

  display: flex;
  justify-content: center;
  align-items: center;
  scroll-behavior: hidden;

  padding: 0 20px;
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

.title-container h1 img {
  width: 10%;
  margin: 0 10px;
}

.principal-section img {
  width: 60%;
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

.examples-section {
  display: flex;
  justify-content: space-around;
  flex-wrap: wrap;
  margin-bottom: 100px;
  padding: 0 30px;

}

.title-section {
  color: #CCC;
  text-align: center;
  margin-bottom: 30px;
}

.title-section::after {
  width: 10px;
  height: 5px;
  background-color: #fff;
  
}

.transition-section {
  width: 100%;
  height: 500px;
  background-image: url("https://img.freepik.com/fotos-gratis/vista-lateral-duplo-cheeseburger-com-rissois-de-carne-grelhada-queijo-e-folha-de-alface-entre-bolos-de-hamburguer_141793-4883.jpg?w=2000");
  background-size: cover;
  background-attachment: fixed;
  background-position: center center;
}

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

</style>
