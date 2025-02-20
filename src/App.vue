
<template>
<h1>Mi primer app de Vue</h1>
<MeusNumerator :valorem="7" />
<MeusNumeratorScript :valorem="10" />


</template>
<!--  esto abajo es un script setup con eso ya aparece en html-->
<script lang="ts" setup>
import MeusNumerator from './components/MeusNumerator.vue';
import MeusNumeratorScript from './components/MeusNumeratorScript.vue';

</script>

