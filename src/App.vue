<template>
  <div id="app">
    <Home v-if="!isLogin"></Home>
    <Editor v-if="isLogin"></Editor>
  </div>
</template>

<script>
import Home from './components/Home'
import Editor from './components/Editor'

export default {
  name: 'App',
  data () {
    return {
      isLogin: false
    }
  },
  components: {
    'Home': Home,
    'Editor': Editor
  }
}
</script>
