<template>
    <div>
        <h2>this is child2</h2>
        <el-button type="primary">按钮</el-button>
    </div>
</template>

<script>
    export default {
        name: "child2",
        methods: {

        },
        mounted() {
            this.$bus.$on('child1-handleClick', (params) => {
                console.log('child2 receive params', params);
            })
        }
    }
</script>

<style scoped>

</style>