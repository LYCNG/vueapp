<template lang="">
    <div>
        <p>當前 1 日幣 = 0.278 台幣</p>
        <div>台幣 <input type="text" v-model="twd" v-on:input="twd2jpy"></div>
        <div>日幣 <input type="text" v-model="jpy" v-on:input="jpy2twd"></div>
        <div>美金 <input type="text" v-model="usd"></div>
    </div>
</template>
<script>
export default {
    data() {
        return {
        twd: 0.278
        }
    },
    computed: {
        jpy:{
            get(){
                return Number.parseFloat(Number(this.twd) / 0.278).toFixed(3);
            },
            set(val){
                this.twd = Number.parseFloat(Number(val) * 0.278).toFixed(3);
            }
        },
        usd: {
            get() {
                return Number.parseFloat(Number(this.twd) / 28.540).toFixed(3);
            },
            set(val) {
                this.twd = Number.parseFloat(Number(val) * 28.540).toFixed(3);
            }
        }
    }
}
</script>
<style lang="">
    
</style>