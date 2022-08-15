<script setup>
defineProps(['file', 'type', 'size'])
</script>

<template>
    <div class="flex">
        <a href="../api/{{file}}">{{ file }}</a>
        <p>{{ type }}</p>
        <p>{{ size }}</p>
    </div>
</template>