<script setup>
import { Link } from "@inertiajs/inertia-vue3";

defineProps({
    time: String,
    users: Array,
});
</script>

<template>
    <h1 class="text-3xl">Users</h1>

    <ul>
        <li v-for="user in users" :key="user.id" v-text="user.name" />
    </ul>

    <div style="margin-top: 400px">
        <p>The current time is {{ time }}</p>
        <Link href="/users" class="text-blue-500" preserve-scroll>Refresh</Link>
    </div>
</template>
