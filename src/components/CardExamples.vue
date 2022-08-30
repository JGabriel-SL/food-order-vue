<template>
  <div class="container">
    <h1>Combo 1</h1>
    <img src="@/assets/burger.png" />
    <p>burguerX1</p>
  </div>
</template>

<script>
export default {
    name: 'CardExamples'
}
</script>

<style scoped>
    .container {
        min-height: 40vh;

        display: flex;
        flex-direction: column;
        align-items: center;

        background-color: #fff;
        width: 300px;
        color: #333;
        padding: 20px 10px;

        border-radius: 20px;
        border: 4px rgb(245, 3, 3) solid;
        margin-bottom: 30px;
    }
    .container img {
      width: 60%;
    }


</style>