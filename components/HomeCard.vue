<template>
    <div>
        <img :src="home.images[0]" style="width:200px" alt=""><br />
        {{ home.title }} <br />
        {{ home.location.adress }} {{ home.location.city }} {{ home.location.state }}<br />
        {{ home.guest }} guests<br />
        {{ home.pricePerNight }} €<br />
    </div>
</template>

<script>
    export default{
        props:{
            home:{
                type: Object,
                required: true,
            }
        }
    }
    
    </script>
    