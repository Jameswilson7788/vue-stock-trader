<template>
    <div>
        <h1>歡迎來到資金矽谷！</h1>
        <h6>你可以在這裡進行股票買賣</h6>
        <h6>隨時檢查你的資產，並在股票市場裡購買股票，並按下"結束"來切換到下一天。</h6>
        <hr>
        <p>你的資金: {{ funds | currency }}</p>
    </div>
</template>

<script>
    export default {
        computed: {
            funds() {
                return this.$store.getters.funds;
            }
        }
    }
</script>