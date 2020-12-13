<template>
  <div class="flex flex-col rounded-lg shadow-lg overflow-hidden">
    <div class="flex-shrink-0">
      <img
        class="h-48 w-full object-cover"
        loading="lazy"
        src="https://images.unsplash.com/photo-1496128858413-b36217c2ce36?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1679&q=80"
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
  },
};
</script>
