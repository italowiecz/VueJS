<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
   
    <ul>
      <li v-for="user in users">
        {{user.firstname}} {{user.lastname}}
      </li>
    </ul>


  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data() {
    return {
      users: [
        { firstname: 'Italo', lastname: 'Wieczorek' },
        { firstname: 'Henrique', lastname: 'Mentz' },
        { firstname: 'Ironi', lastname: 'Medina' }
      ],
      input_val: '',
      msg: 'Já é uma realidade!',
      counter: 0
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
