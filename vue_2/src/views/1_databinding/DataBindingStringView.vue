<!-- 뷰의 장점 : 양방향 데이터 바인딩이 가능하다. -->
<!-- 뷰의 장점 : html, script, css를 완벽하게 분리할 수 있다. -->
<!-- 새로운 화면 구현시 router에 추가 해주어야 한다. -->
<!-- html 코드를 넣는 부분 -->
<template>
    <!-- 최상위 태그가 하나 있어야 한다. vue3은 필수가 아니지만 확장성을 위해 선언하는 것이 좋다. -->
    <div>
        <p>중괄호 두개 : 문자형 데이터 바인딩</p>
        <h1>hello {{ userName }}</h1>
        <p>{{ message }}</p>
    </div>
</template>
<!-- java script 코드를 넣는 부분 -->
<script>
export default {
    // 뷰는 함수를 만들 때 앞에 function을 명시하지 않아도 가능하다.
    data() {
        // 리턴안에 정의해야 상단 template에서 사용할 수 있다. ( key:value )
        return {
            userName: 'name',
            message: 'welcome 개발자의 품격',
            arr: [],
            obj: {}
        }
    }
}
</script>
<!-- css 코드를 넣는 부분 -->
<style scoped>
    /* scoped : 해당 화면에 대한 CSS만을 나타낸다. */

</style>
