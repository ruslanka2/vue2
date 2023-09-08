<template>
  <IndexComponents/>
    <BlogComponents/>
    <BlogdetalisComponents/>
   <CategoryComponents/>
   <ProjectDetalisComponent/>
  </template>
  
  <script>
  
  import IndexComponents from './components/IndexComponents.vue';
  import BlogComponents from './components/BlogComponents.vue';
  import BlogdetalisComponents from './components/BlogdetalisComponents.vue';
  import CategoryComponents from './components/CategoryComponents.vue';
  import ProjectDetalisComponent from './components/ProjectDetalisComponent.vue';
  
  
  export default {
    name: 'App',
    components: {
      IndexComponents,
      BlogComponents,
      BlogdetalisComponents,
      CategoryComponents,
      ProjectDetalisComponent
  }
  }
  </script>
  
  <style lang="scss">
  #app {
    
  }
  </style>
  