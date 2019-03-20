<template>
    <div>
        <h1>{{title}}</h1>
        <ul>
            <li v-for="book in books">{{book.title}}:{{book.author}}</li>
         </ul> 
    </div>
</template>

<script>
export default {
    name:'BookList',
    data(){
        return{
            title: 'All Books',
            books: [
                {title:"Self-Reliance", author:"Neil 1"},
                {title:"American Gods", author:"Neil 2"},
                {title:"Amusing ourselves to death", author:"Neil Postman"},
            ]
            }
        }
    }

</script>

<style>

h1, h2 {font-weight: normal}
ul{
    list-style-type: none;
    padding: 0px;
}
li{
    display: block;
    margin: 0 10px;
}
</style>
