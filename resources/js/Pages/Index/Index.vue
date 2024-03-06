<template>
  
        <h1>Home</h1>
        <Link href="/hello">ShowPage</Link>
        <div>
            The Message is : {{ message }}
        </div>

</template>

<script setup>
import { Link } from '@inertiajs/vue3'
defineProps({
    message: String
})
</script>

<script>
    import MainLayout from '../../Layouts/MainLayout.vue';
    export default {
        layout: MainLayout,
}
</script>
