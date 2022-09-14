<script setup>
import NavLink from "@/Components/NavLink.vue";
</script>

<template>
    <nav class="ml-6">
        <ul class="flex list-disc space-x-4 list-inside">
            <li>
                <NavLink href="/" :active="$page.component === 'Home'">
                    Home
                </NavLink>
            </li>
            <li>
                <NavLink href="/users" :active="$page.component === 'Users'">
                    Users
                </NavLink>
            </li>
            <li>
                <NavLink
                    href="/settings"
                    :active="$page.component === 'settings'"
                >
                    Settings
                </NavLink>
            </li>
        </ul>
    </nav>
</template>
