<template>
<div id="Noticias"  class="row mt-md-5 mt-sm-5 mt-xs-5">
    <div class="col-lg-6 col-xs-12" v-for="(infoNoticia,index) of infoNoticias" :key="index">
        <div class="d-flex justify-content-center align-items-center" >

            <div class="p-3">
                <img :src="infoNoticia.image" alt="Foto Noticia" width="200">
            </div>

            <div class="p-2">
                <h4> {{infoNoticia.title}}</h4>
                
                <p>
                    {{infoNoticia.description}}
                </p>
                
            </div>

        </div>
        <div class="d-flex container-fluid justify-content-end pb-2 mt-n2" >
            <button type="button" onclick=":location.href='infoNoticia.url'" class="btn btn-outline-info">Info</button>
        </div>
    </div>
</div>
</template>
<script>
import axios from "axios"
export default {
    name: 'NewsSection',
    data(){
        return{
            infoNoticias : null
        }
    },
    created(){
        axios
            .get("http://api.mediastack.com/v1/news?access_key=2e66c51754dfe7a4b152bb11e76ee04b&sources=cnn,nytimes&keywords=spacex")
            .then(response => {this.infoNoticias= response.data.data.slice (0,4)}).catch(error=> console.log(error))
        console.log(this.infoNoticias)
    }
}
</script>