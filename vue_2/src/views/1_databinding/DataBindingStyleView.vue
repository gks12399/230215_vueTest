<template>
    <div>
        <div>스타일 바인딩: 글씨는 Red, 폰트크기: 30px</div>
        <p :style="style1">적용하기</p>

        <div>스타일 바인딩: 글씨는 Green, 폰트스타일: 10px</div>
        <p :style="style2">적용하기</p>
        <button @click="style2.color='blue'">색상변경</button>
        <button @click="style2.fontStyle='normal'">폰트변경</button>
    </div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            style1: {
                color: 'red',
                fontSize: '30px'
            },
            style2: {
                color: 'green',
                fontStyle: 'italic'
            }
        }
    },
    setup() {},
    created() {},
    mounted() {},
    unmounted() {},
    methods: {}
}
</script>
