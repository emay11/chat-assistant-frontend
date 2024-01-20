<script setup>
defineProps({
  msg: {
    type: String,
    required: true
  }
})
</script>

<template>
  <h1>Login</h1>
  <form @submit.prevent="registerAnswer">
    <label> 
      <textarea v-model="txtInp" placeholder="Write something.." rows="4" cols="35"></textarea>
    </label>
    
  </form> 
</template>
<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  text-align: center;
  border: 1px solid red;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
