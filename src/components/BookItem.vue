<template>
  <li v-for="book in books">{{book.title}}:{{book.author}}</li>  
</template>

<script>
export default {

    name: 'Book',
    props: ['book']
}
</script>

<style>
li{
    display: block;
    margin: 0 10px;
}

</style>
