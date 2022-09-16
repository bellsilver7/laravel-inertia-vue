<script setup>
import Nav from "@/Shared/Nav.vue";
import { computed } from "vue";
import { usePage } from "@inertiajs/inertia-vue3";

const user = computed(() => usePage().props.value.auth.user);
</script>

<template>
    <section class="p-6 bg-gray-200">
        <header class="flex justify-between">
            <div class="flex items-center">
                <h1 class="font-bold text-lg">
                    <input type="text" value="My app" />
                </h1>
                <p class="text-sm ml-4">Welcome back, {{ user.name }}!</p>
            </div>
            <Nav />
        </header>
    </section>
    <section class="p-6">
        <div class="max-w-3xl mx-auto">
            <slot />
        </div>
    </section>
</template>
