<template>
    <div class="p-4 flex-1 overflow-y-auto">
        <div class="flex- flex-col space-y-2">
           
  

<ChatBullula :meus-est="true" nuntius="let's get out soon?"/>
   
<ChatBullula 
:meus-est="false" 
nuntius="no" 
imago="https://yesno.wtf/assets/yes/2.gif"/>
</div>
</div>

</template>

<script lang="ts" setup>

import ChatBullula from './ChatBullula.vue';

</script>
