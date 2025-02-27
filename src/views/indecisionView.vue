
<template>


<div class="bg-gray-200 h-screen  flex flex-col max-w-lg mx-auto">
    <div class="bg-blue-500 p-4 text-white flex justify-between items-center">
       <span> Mi esposa</span>
    </div>
       <ChatNuntii :nuntii="nuntii"/>
       <TextusArca />
    

</div>
</template>


<script lang="ts" setup>
import ChatNuntii from '@/components/chat/ChatNuntii.vue';
import TextusArca from '@/components/chat/TextusArca.vue';
import type { ChatNuntius } from '@/interfaces/chat-nuntius.interface';
import { ref } from 'vue';

const nuntii = ref<ChatNuntius[]>([
{
   id: new Date().getTime(),
   nuntius:'voy a tomar cafe.',
   meusEst:true,
},
{
   id: new Date().getTime() +2,
   nuntius:'vale.',
   meusEst:false,
   imago:''
}
]);

</script>