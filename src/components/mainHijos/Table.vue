<template>
    <section class="container">
        
        <div v-for="(item, index) in dataUsers" :key="index">
            <div class="mb-3" style="max-width: 540px;">
                <div class="row no-gutters">
                    <div class="col-md-4">
                        <img :src="item.src" :alt="item.nombre" class="card-img rounded-circle">
                    </div>
                    <div class="col-md-8">
                        <div class="card-body text-white">
                            <h5 class="card-title">{{item.nombre}}</h5>
                        </div>
                    </div>
                </div>
            </div>
        </div> 

    </section>
</template>

<script>
export default {
    name: 'Table',
    props: {
        dataUsers: {
            type: Array,
            required: true,
            default(){
                return [
                    {nombre: 'No tiene', src: 'no tiene'}
                ]
            } 
        }
    },
}
</script>

<style>
    
</style>