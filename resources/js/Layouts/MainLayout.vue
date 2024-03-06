<template>
 <Link href="/">HomePage</Link>&nbsp;
 <Link href="/hello">ShowPage</Link>
 <div>The timer is : {{ timer }}</div>
    <slot></slot>
</template>

<script setup>
import { Link } from '@inertiajs/vue3';
import { ref } from 'vue';

const timer = ref(0);
setInterval(()=> timer.value++, 1000);
</script>
