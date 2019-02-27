<template>
  <div id="app">
    <drop-down-input v-model="msg"
      :drop-down-list="list"
      key-name="label"
      placeholder="请下拉选择或者输入"
      errorMsg="输入不正确"
      @clear="onClear"
      @focus.native="onFocus"
      @on-query-change="onQueryChange">
    </drop-down-input>
  </div>
</template>

<script>
import dropDowninput from '../src/package/drop-down-input/drop-down-input'
export default {
  name: 'app',
  components: {
    'drop-down-input': dropDowninput
  },
  data () {
    return {
      msg: '',
      list: [
        {
          label: 'hello',
          value: 1
        },
        {
          label: 'word',
          value: 2
        }
      ]
    }
  },
  methods: {
    onClear (value) {
    },
    onFocus (value) {
    },
    onQueryChange (query) {
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
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
