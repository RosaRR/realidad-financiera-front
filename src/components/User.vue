<template>
    <div id="User">
        <h2>Hola <span> {{username}}, </span> ¡Bienvenido a nuestra Aplicación!</h2>
    </div>
</template>
<script>
    export default {
        name: "User",
        data:function(){
            return {
                username: "none"
            }
        },
        created: function(){
            this.username = this.$route.params.username
        }
    }
</script>
<style>
    #User{
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    #User h2{
        font-size: 50px;
        color: #282829;
    }
    #User span{
        color: rgb(11, 221, 186);
        font-weight: bold;
    }
</style>