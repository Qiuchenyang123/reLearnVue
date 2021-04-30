<template>
    <div class="about">
        <h1>This is an about page</h1>
        <child1/>
        <child2/>
    </div>
</template>

<script>
    import child1 from "./testPage/children/child1";
    import child2 from "./testPage/children/child2";

    export default {
        name: 'about',
        components: {
            'child1': child1,
            'child2': child2,
        }
    }
</script>
