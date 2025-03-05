<template>
    <div ref="chatRef" class="p-4 flex-1 overflow-y-auto">
        <div class="flex- flex-col space-y-2">
           
      
<ChatBullula :meus-est="true" nuntius="let's get out soon?"/>


<ChatBullula 
v-for="nuntius in nuntii"
:key="nuntius.id"
:meus-est="nuntius.meusEst" 
:nuntius="nuntius.nuntius" 
:imago="nuntius.imago" />

<!--
<ChatBullula 
v-for="nuntius in nuntii"
:key="nuntius.id"
:v-bind="nuntius"
 />-->
</div>

</div>
</template>

<script lang="ts" setup>

import type { ChatNuntius } from '@/interfaces/chat-nuntius.interface';
import ChatBullula from './ChatBullula.vue';
import { ref, watch } from 'vue';
//props envian el padre
interface Props{
    nuntii: ChatNuntius[];
}
const props = defineProps<Props>();

const chatRef = ref<HTMLDivElement | null>(null);

watch( props.nuntii , () =>{

console.log('nuntii cambio');

setTimeout(()=>{
    chatRef.value?.scrollTo({
        top: chatRef.value.scrollHeight,
        behavior: 'smooth'
    })

})
   
});

</script>
