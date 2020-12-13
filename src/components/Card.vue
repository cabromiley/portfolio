<template>
  <div class="flex flex-col rounded-lg shadow-lg overflow-hidden">
    <div class="flex-shrink-0">
      <img
        class="h-48 w-full object-cover"
        loading="lazy"
        :src="image"
        alt=""
      />
    </div>
    <div class="flex-1 bg-white p-6 flex flex-col justify-between">
      <div class="flex-1">
        <p class="text-sm font-medium text-indigo-600">
          <a href="#" class="hover:underline">
            {{ skills.join(", ") }}
          </a>
        </p>
        <a href="#" class="block mt-2">
          <p class="text-xl font-semibold text-gray-900">
            {{ title }}
          </p>
          <div class="mt-3 text-base text-gray-500">
            <slot />
          </div>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: { type: String, required: true },
    skills: { type: Array, default: () => [] },
    image: { type: String, required: true }
  },
};
</script>
