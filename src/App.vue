<template>
  <div class="app">
    <div class="wrapper">
      <h3 class="app__header" @click="showUl">List Header</h3>
      <ul class="app__ul">
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
      </ul>
      <h3 class="app__header">List Header</h3>
      <ul class="app__ul">
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
      </ul>
      <h3 class="app__header">List Header</h3>
      <ul class="app__ul">
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
      </ul>
      <h3 class="app__header">List Header</h3>
      <ul class="app__ul">
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
      </ul>
      <h3 class="app__header">List Header</h3>
      <ul class="app__ul">
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
      </ul>
      <h3 class="app__header">List Header</h3>
      <ul class="app__ul">
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
        <li class="app__list">List element</li>
      </ul>
    </div>
  </div>
</template>

<script>

export default {
  name: 'App',
  data () {
    return {

    }
  },
  methods: {
    showUl: function () {
      const ul = document.querySelectorAll('.app__ul')
      ul.classList.add('showUl')
      console.log('clicked')
    }
  }
}
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
li {
  list-style: none;
}
.showUl {
  display: none;
}
.app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  &__header {
    padding: 10px;
    border: 1px solid black;
    background: #ccc;
    margin: 10px 0;
  }
  &__ul {
    padding-left: 20px;
  }
  &__list {
    padding: 10px 10px;
    margin: 10px 0;
    border: 1px solid #ccc;
    background: aqua;
  }
}
.wrapper {
  margin: 0 auto;
  width: 700px;
  background: #fff;
}
</style>
