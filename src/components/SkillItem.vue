<template>
    <div class="flex">
        <!-- Heroicon name: check -->
        <svg class="flex-shrink-0 h-6 w-6 text-green-500" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
        </svg>
        <div class="ml-3">
            <dt class="text-lg leading-6 font-medium text-gray-900">
                {{ header }}
            </dt>
            <dd class="mt-2 text-base text-gray-500">
                <slot>{{ description }}</slot>
            </dd>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        header: { type: String, required: true },
        description: { type: String, default: '' }
    }
}
</script>