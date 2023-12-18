<script setup>
  import {ref} from 'vue'
  import Title from "./components/Title.vue"
  const text = ref("The Spy")
  </script>
<template>
 <Title :num = 60>
 <template #text>
    The Spy  
</template>
 </Title>
 <div class="container">
  <!-- Content here -->
  <div class= "card text-center w-60 mx-auto">
    <div class = "card-body">
      <div class = "card-text">
        <Title :num = 10>
        <template #text>
          Welcome to The Spy  
        </template>
 </Title>
      </div>
    </div>
  </div>
  
</div>
</template>

<style>
body{
  margin: 0;
  padding:0;
  background-color: beige;
}
.mainbody{
  display: flex;
  align-self: center;
  margin-left: 20%;
  margin-right:20%;
  justify-content: center;
  background-color: "red";
  border: 1px solid black;
}

</style>
