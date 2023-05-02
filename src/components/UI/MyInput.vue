<template>
    <input :value="modelValue" @input="updateInput" class="input" type="text">
</template>

<script>
    export default {
       name: 'my-input',
       props: {
        modelValue: [String, Number]
       },
       methods: {
        updateInput(event) {
            this.$emit('update:modelValue', event.target.value)
            
        }
       }
    }
</script>

<style scoped>
.input{
        width: 100%;
        margin-top: 15px;
        border: 1px solid  #009ee3;
        background-color: #009ee3;
        padding: 18px 15px;
    }
    .input:hover{
        background-color: #0070d2;
    }
    
</style>