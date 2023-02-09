<template lang="">
    <div>
        <button v-on:click="counter('+')">+</button>
        <button v-on:click="counter('-')">-</button>
        <div>{{count}}</div>
    </div>
</template>
<script>
export default {
    name:"Counter-comp",
    data()
    {
        return {
            count:0
        }
    },
    methods:{
        counter(value){
            if(value=='+'){

                this.count=this.count+1
            }else{
                this.count=this.count-1
            }
        }
       
    }
}
</script>
<style scoped>
    
</style>