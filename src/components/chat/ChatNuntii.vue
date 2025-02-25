<template>
    <div class="p-4 flex-1 overflow-y-auto">
        <div class="flex- flex-col space-y-2">
           
           <!-- 
            <div class="flex justify-end">
                <div class="bg-blue-200 text-black p-4 max-w-xs rounded-lg">
        Hi, What about your day?
         </div>
</div>

<div class="flex justify-start">
    <div class="bg-gray-300 text-black p-4 max-w-xs rounded-lg">
        That was great. What about your day? 
            </div>
        </div>

-->
<ChatBullula :meus-est="true" nuntius="let's get out soon?"/>
    </div>
</div>

</template>

<script lang="ts" setup>

import ChatBullula from './ChatBullula.vue';

</script>
