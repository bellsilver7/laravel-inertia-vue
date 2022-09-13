<script setup>
defineProps({
    name: String,
    frameworks: Object,
});
</script>

<template>
    <main>
        <h1 class="text-xl">Hello, {{ name }}</h1>
        <p>In this series, we will use the following frameworks:</p>
        <ul class="flex">
            <li
                v-for="framework of frameworks"
                v-text="framework"
                class="text-sm bg-slate-200 rounded px-2 py-1 m-1"
            ></li>
        </ul>
    </main>
</template>
