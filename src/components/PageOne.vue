<template>
  <div class="hello">
    <span v-html="title"></span>
    <h1>{{ name }}</h1>
    <h2 v-text="firstname"></h2>
    <ul v-if="showList" id="example-1">
  <li v-for="item in items" :key="item">
    {{ item.age }}
  </li>
</ul>
    </div>
</template>

<script>
export default {
  name: 'PageOne',
  data () {
    return {
      name: 'Dheeraj started Vue.js',
      title: '<h1>HEllo</h1>',
      firstname: 'dheeraj',
      showList: false,
      items: [
          {
              roll: 2,
              age: 22
          },
           {
              roll: 3,
              age: 23
           }
      ]
    }
  }
}
</script>
