<script lang="ts" setup>
    const { text, href } = defineProps<
    {
        text:string,
        href:string,
        logo:string,
    }>()
</script>
<template>
    <li class="lg:inline-flex">
        <NuxtLink class="lg:inline-flex transition hover:text-primary ease-linear text-lg" :to="href" target="_blank">
            <img :src="logo" style="width:auto;height:20px;">{{ text }}
        </NuxtLink>
    </li>
</template>