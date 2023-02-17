<template>
    <div>
        <p>
            keyup이벤트 2가지 방법<br>
            - 엔터 입력시 버튼 누른것과 같은 효과
        </p>
        <!-- <input type="search" @keyup="checkEnter($event)" v-model="searchText"> -->
        <input type="search" @keyup.enter="doSearch" v-model="searchText">
        <button @click="doSearch()">조회</button>
    </div>
</template>
<script>
export default {
    components: {},
    data() {
        return {
            searchText: ''
        }
    },
    setup() {},
    created() {},
    mounted() {},
    unmounted() {},
    methods: {
        doSearch() {
            console.log(this.searchText)
        },
        checkEnter(event) {
            if (event.keyCode === 13) {
                this.doSearch()
            }
        }
    }
}
</script>
