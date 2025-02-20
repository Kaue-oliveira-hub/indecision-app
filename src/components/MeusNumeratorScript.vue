<template>
    <section>
        <h3>counter: {{ numerus}}</h3>
        <h3> Square: {{ quadrataNumerus }}</h3>
    <div>
        <button @click="numerus++">+1</button>
        <button @click="numerus--">-1</button>
    </div>
    </section>
    </template>

<script lang="ts" setup>
import { computed, ref } from 'vue';

defineProps<{
    valorem: number;
}>();

const numerus = ref(valorem);
const quadrataNumerus = computed(() => numerus.value * numerus.value);

return {
    numerus,
    quadrataNumerus,
};




//variable reactiva hay que poner value

</script>
