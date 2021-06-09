<template>
    <main>
        <h2>Content goes here</h2>
    </main>
</template>

<script>
export default {
    name: "Center"
}
</script>

<style lang="scss" scope>
    @import "../style/Color.scss";

    main {
        display: flex;
        width: 100%;
        height: 100px; 
        background-color: $bg-center;

        h2 {
            margin: auto;
            font-size: 20px;
            color: $text-color;
        }
    }
    
</style>