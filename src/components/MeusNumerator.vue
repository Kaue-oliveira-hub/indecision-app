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
import { useNumerator } from '@/composables/useNumarator';
import { computed, ref } from 'vue';

interface Props {
    valorem: number;
}

const props = defineProps<Props>();
//variable reactiva hay que poner value

const {numerus, quadrataNumerus } =useNumerator (props.valorem);
</script>
