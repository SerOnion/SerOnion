<template>
    <div>
        <header>
            <ul class="nav">
                <li><router-link class="link" to="/"><b>HOME</b></router-link></li>
                <li><router-link class="link" to="/page2"><b>Page1</b></router-link></li>
                <li><router-link class="link" to="/page3"><b>History</b></router-link></li>
            </ul>
        </header>
        <section class="content">

            
            <slot/>

        </section>
    
    </div>
</template>

<script>
    export default {
        name: "Default"
    }
</script>

<style scoped>
    header{
        background-color: rgb(177, 6, 6);
        height: 70px;
        display: flex;
        align-items: center;
    }

    footer{
        background-color: rgb(211, 38, 38);
        height: 70px;
    }

    .content{
        min-height: calc(100vh - 140px);
        background-image: url('https://images.wallpaperscraft.ru/image/kresla_krasnyj_riady_152340_3840x2160.jpg');
    }

    ul{
        list-style: none;
        margin: 0;
        color: white;
    }

    li{
        color: white;
        display: inline;
        margin: 0 5px;
    }

    .link{
        color: white;
        text-decoration: none;
    }

</style>