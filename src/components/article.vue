<template>
    <div id="users">
        <ul>
            <li v-for="i in users" :key="i" v-on:click="i.status = !i.status" >
                <h2>
                    {{i.name}}
                </h2>
                <p v-if="i.status">{{i.job}} </p>
            </li>
        </ul>
        <button v-on:click="DeleteUser()">Sil</button>
    </div>

</template>

<script>
export default {
    props:["users"],
    data(){
        return{
            

        }
    },
    methods:{
        DeleteUser(){
            this.users.pop();

        }
    }
}
</script>

<style scoped>

ul{
    display: flex;
    flex-wrap: wrap;
    list-style-type: none;
    padding: 0;
}

li{
    flex-grow: 1;
    flex-basis: 300px;
    text-align: center;
    padding: 30px;
    border: 1px solid black;
    margin: 10px;
}

#users{
    width: 100%;
    max-width: 1200px;
    margin: 40px auto;
    padding: 0 20px;
    box-sizing: border-box;
}

</style>

