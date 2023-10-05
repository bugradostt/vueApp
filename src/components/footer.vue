<template>
    <footer>
        <p>{{title}}</p>
        <p>{{copyright}} - {{year}}</p>
    </footer>
</template>

<script>

export default{
    props:["title"],
    data(){
        return{
            year:2023,
            copyright:"Tüm hakkları saklıdır."

        }
    }
}
</script>

<style scoped>
footer{
    background: #222;
    padding: 6px;
}
p{
    color: lightgreen;
    text-align: center;
}
</style>
