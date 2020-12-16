<template>
    <div>
        <div class = "card bg-light">
            <div class = "d-flex justify-content-center p-2">
                <img :src="member.image" with="200px" height="200px" alt="imagenperfil" class="rounded-circle z-depth-2" data-holder-rendered="true">
            </div>
            <div class = "card-body">
                <h5 class="card-title"> {{ member.nombre }} </h5>
                <p class="card-text"> {{ member.descripcion }} </p>
            </div>
            <div class="card-footer">
                <small class="text-muted"> {{ member.rol }} </small>
                <a :href="member.whatsapp"><img class="zoom" src="https://www.flaticon.es/svg/static/icons/svg/733/733585.svg"/></a>
                <a :href="member.facebook"><img class="zoom" style="margin-left:5px" src="https://www.flaticon.es/premium-icon/icons/svg/3670/3670042.svg"/></a>
            </div>
        </div>
    </div>
</template>

<script> 
    require('./../assets/js/app.js');
    export default {
        name: "TeamCard",
        props: ['member']
    }
</script>


<style scoped>
    @import '../assets/css/app.css';
</style>
