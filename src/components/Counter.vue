<template lang="">
    <div>
        <button v-on:click="inc">+</button>
        <button v-on:click="dec">-</button>
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
        inc(){
            this.count=this.count+1
        },
        dec(){
            this.count=this.count-1
        }
    }
}
</script>
<style scoped>
    
</style>