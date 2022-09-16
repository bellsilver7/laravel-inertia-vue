<script setup>
defineProps({
    active: Boolean,
});
</script>

<template>
    <Link
        class="hover:underline"
        :class="{
            'font-bold underline': active,
        }"
    >
        <slot />
    </Link>
</template>
