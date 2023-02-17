<template>
    <div>
        <p>:class="{ 'key':[ture|false] } => 클래스이름:ture or false</p>
        <div :class="{ 'text-red':hasError, active: isActive }">클래스 바인딩</div>
        <div :class="{ 'text-red':isActive, active: hasError }">클래스 바인딩</div>
        <div :class="class2">클래스 바인딩 2</div>
    </div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            isActive: false,
            hasError: true,
            class2: [
                'text-red', 'isActive'
            ]
        }
    },
    setup() {},
    created() {},
    mounted() {},
    unmounted() {},
    methods: {}
}
</script>
<style scoped>
.active{
    background-color: greenyellow;
    font-weight: bold;
}
.text-red{
    color: red;
}
</style>
