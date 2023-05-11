<template>
  <div>
    <h5>{{article.id}}</h5>
    <p>{{article.title}}</p>
    <router-link :to="{
      name:'Detailview', 
      params:{id:article.id}}">
      [detail]
      </router-link>
    <hr>
  </div>
</template>

<script>
export default {
  name: 'ArticleListItem',
  props:{
    article:Object,
  }
}
</script>

<style>

</style>
