<script setup>
import NavLink from "@/Components/NavLink.vue";
</script>

<template>
    <nav class="ml-6">
        <ul class="flex space-x-6">
            <li>
                <NavLink href="/" :active="$page.component === 'Home'">
                    Home
                </NavLink>
            </li>
            <li>
                <NavLink
                    href="/users"
                    :active="$page.component === 'Users/Index'"
                >
                    Users
                </NavLink>
            </li>
            <li>
                <NavLink
                    href="/settings"
                    :active="$page.component === 'Settings'"
                >
                    Settings
                </NavLink>
            </li>
            <li>
                <NavLink href="/logout" method="post">Log Out</NavLink>
            </li>
        </ul>
    </nav>
</template>
