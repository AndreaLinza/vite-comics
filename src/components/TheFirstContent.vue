<script>
export default {};
</script>

<template>
    <section>
        <div class="container d-flex">
            <h3> ->Content goes here </h3>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use "../styles/partials/variables" as *;

section {
    font-family: $font-primary;
    background-color: #24201F;
    height: 150px;
    display: flex;
    align-items: center;
    justify-content: start;

    div {
        
        h3 {
            font-weight: 600;
            color: white;
        }
    }
}
</style>