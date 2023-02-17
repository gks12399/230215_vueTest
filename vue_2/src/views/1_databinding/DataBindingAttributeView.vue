<template>
    <div>
        <p>
            v-bind를 사용하여 단방향 데이터 바인딩 처리<br>
            속성에 직접 접근하여 데이터를 바인딩 한다.<br>
            v-bind:[속성]에서 :[속성]으로 v-bind는 생략 가능하다.
        </p>
        <input type="text" v-bind:value="userId" readonly>
        <input type="text" :value="userId" readonly>
        <br><br>
        <img :src="imgSrc" alt="" style="width: 100px; height: 100px;">
        <br>
        <input type="search" v-model="txt1">
        <button :disabled="txt1 === ''">조회</button>
    </div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            userId: 'abc',
            imgSrc: 'data:image/png;base64,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',
            txr1: ''
        }
    },
    setup() {},
    created() {},
    mounted() {},
    unmounted() {},
    methods: {}
}
</script>
