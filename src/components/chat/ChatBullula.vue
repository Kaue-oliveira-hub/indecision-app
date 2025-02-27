<template>

<div v-if="meusEst" class="flex justify-end">
                <div class="bg-blue-200 text-black p-4 max-w-xs rounded-lg">
       {{ nuntius }}
         </div>
</div>

<div v-else class="flex justify-start">
    <div class="bg-gray-300 text-black p-4 max-w-xs rounded-lg">
       
        <span class="capitalize"> {{ nuntius }}</span>
        <img v-if="imago" :src="imago" alt="YesNoImage" class="w-52 h-52" />
            </div>
        </div>




</template>

<script lang="ts" setup>
interface Props {
    nuntius: string;
    meusEst:boolean;
    imago?: string;
}

defineProps<Props>();

</script>