<template>
    <button
        class="btn"
    >
        <slot></slot>
    </button>
</template>

<script>
    export default {
        name: 'my-button'
    }
</script>

<style scoped>
.btn{
    padding: 10px 15px;
    background: none;
    color: #009ee3;
    border: 1px solid #009ee3;
    }
    .btn:hover{
        color: #0070d2;
    }
</style>