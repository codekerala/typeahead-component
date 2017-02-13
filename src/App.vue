<template>
  <div id="app">
    <typeahead :options="options" v-model="selected"></typeahead>
  </div>
</template>

<script>
import Typeahead from './components/Typeahead'
export default {
  name: 'app',
  components: {
    Typeahead
  },
  data() {
    return {
      selected: null,
      options: [
        {id: 1, text: 'Apple'},
        {id: 2, text: 'Mango'},
        {id: 3, text: 'Cherry'},
        {id: 4, text: 'Orange'},
        {id: 21, text: 'Appl22e'},
        {id: 22, text: 'Mang2o'},
        {id: 23, text: 'Cher2ry'},
        {id: 24, text: 'Oran2ge'},
        {id: 41, text: 'A4pple'},
        {id: 42, text: 'Ma4ngo'},
        {id: 43, text: 'Ch4erry'},
        {id: 44, text: 'Ora4nge'}
      ]
    }
  }
}
</script>

<style>
body {
  font-family: Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 60px auto;
  width: 300px;
}
* {
  box-sizing: border-box;
}
</style>
