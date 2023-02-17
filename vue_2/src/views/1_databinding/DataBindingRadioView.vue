<template>
    <div>
        <p>
            체크 박스, 라디오 버튼의 v-model은 <br>
            value속성에 바인딩이 아닌 <br>
            checked속성에 바인딩이 된다.
        </p>
        <p>
            * 라디오버튼은 문자열로 선언한다.
        </p>
        <div>
            <input type="radio" id="html" value="HTML" v-model="favoriteLang">
            <label for="html">HTML</label>
        </div>
        <div>
            <input type="radio" id="css" value="CSS" v-model="favoriteLang">
            <label for="css">CSS</label>
        </div>
        <div>
            <input type="radio" id="js" value="JAVASCRIPT" v-model="favoriteLang">
            <label for="js">JAVASCRIPT</label>
        </div>
        <div>
            선택 : {{ favoriteLang }}
        </div>
    </div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            favoriteLang: ''
        }
    },
    setup() {},
    created() {},
    mounted() {},
    unmounted() {},
    methods: {}
}
</script>
