<template>
    <div>
        <p>v-model : 양방향 데이터 바인딩</p>
        <input type="text" v-model="userId" />
        <!-- 전달할 파라미터가 없을 때는 ();을 생략할 수 있다. -->
        <button @click="myfuc">클릭</button>
        <button @click="changeData">변경</button>
        <p>{{ userId }}</p>
        <br>
        <p>문자열로 계산</p>
        <input type="text" v-model="num1"/> +
        <input type="text" v-model="num2"/> =
        <span>{{ num1 + num2 }}</span>
        <br>
        <p>숫자로 계산</p>
        <input type="text" v-model.number="num3"/> +
        <input type="text" v-model.number="num4"/> =
        <span>{{ num3 + num4 }}</span>
    </div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            userId: 'userId',
            num1: 0,
            num2: 0,
            num3: 0,
            num4: 0
        }
    },
    setup() {},
    created() {},
    mounted() {},
    unmounted() {},
    // 함수 선언시 function 생략 가능하다.
    methods: {
        myfuc() {
            // 오브젝트 사용 시 this. 를 꼭 사용해야 한다.
            console.log(this.userId)
        },
        changeData() {
            this.userId = 'hello'
        }
    }
}
</script>
