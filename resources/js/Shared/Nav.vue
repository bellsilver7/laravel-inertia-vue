<script setup>
import { Link } from "@inertiajs/inertia-vue3";
</script>

<template>
    <nav>
        <ul class="flex">
            <li class="text-sm bg-indigo-200 rounded px-2 py-1 mx-1">
                <Link href="/">Home</Link>
            </li>
            <li class="text-sm bg-indigo-200 rounded px-2 py-1 mx-1">
                <Link href="/users">Users</Link>
            </li>
            <li class="text-sm bg-indigo-200 rounded px-2 py-1 mx-1">
                <Link href="/settings">Settings</Link>
            </li>
        </ul>
    </nav>
</template>
