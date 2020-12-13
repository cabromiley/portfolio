<template>
    <div class="max-w-3xl mx-auto text-center">
        <h2 class="text-xl sm:text-3xl font-extrabold text-gray-900">{{ header }}</h2>
    </div>
</template>

<script>
export default {
    props:{
        header: { type: String, required: true }
    }
}
</script>