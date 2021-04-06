<template>
    <button @click="onButtonClick()" :style="{background: color}" class="btn">{{ text }}</button>
</template>

<script>
export default {
    name: 'Button',
    props: {
        text: String,
        color: String
    },
    methods:{
        onButtonClick(){
           this.$emit('toggle-add-task')
        }
    }
}
</script>