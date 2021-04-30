<template>
    <div>
        <h2>this is child1</h2>
        <el-button type="primary" @click="handleClick">按钮</el-button>
    </div>
</template>

<script>
    export default {
        name: "child1",
        methods: {
            handleClick() {
                this.$bus.$emit('child1-handleClick', `this is child1's params`)
            }
        }
    }
</script>

<style scoped>

</style>