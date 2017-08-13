<template>
    <div>
        <button class="btn btn-primary" @click="asyncIncrement({by: 50, duretion: 1500})">AsyncIncrement</button>
        <button class="btn btn-primary" @click="asyncDecrement({by: 50, duration: 2500})">AsyncDecrement</button>
    </div>
</template>

<script>
    import {mapActions } from 'vuex';
    export default {
        methods: {
                ...mapActions([
                    'asyncIncrement',
                    'asyncDecrement'
                ])
        }
    }
</script>