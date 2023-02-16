<template>
    <div>
        <p>v-html : html 형식으로 데이터 바인딩</p>
        <div>{{ htmlString }}</div>
        <div v-html="htmlString"></div>
    </div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            htmlString: '<p style="color:red;">빨간색문자</p>'
        }
    },
    setup() {},
    created() {},
    mounted() {},
    unmounted() {},
    methods: {}
}
</script>
