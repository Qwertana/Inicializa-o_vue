<template>
<div>
 <h1>Sua idade é:</h1>
 <h2>{{idade}}</h2>
 <input type="number" v-model.number="idade">
 <br><br> 
 <button @click="aumentarIdade">Aumentar idade</button>
 <button @click="diminuirIdade">Diminuir idade</button>
</div>
</template>

<script>
export default {
    data() {
        return {
            idade: 24
        }
    },
    methods: {
        aumentarIdade() {
            this.idade++
        },
        diminuirIdade(){
            this.idade--
        }
    }
}
</script>
