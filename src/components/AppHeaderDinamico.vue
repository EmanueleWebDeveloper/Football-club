<template>
    <header>
      <div>
        <ul>
          <li v-for="(menuItem, index) in menuItems" :key="index">
            <a :href="menuItem.link">{{ menuItem.text }}</a>
          </li>
        </ul>
      </div>
    </header>
  </template>
  
  <script>
  export default {
    name: 'AppHeaderDinamico',
    props: {
      menuItems: {
        type: Array,
        default: () => []
      }
    }
  }
  </script>
  
  <style lang="scss" scoped>
  
  </style>
  