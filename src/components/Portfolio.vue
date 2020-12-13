<template>
  <div
    class="relative bg-gray-50 pt-8 pb-20 px-4 sm:px-6 lg:pt-16 lg:pb-28 lg:px-8"
  >
    <div class="relative max-w-7xl mx-auto">
      <section-header header="Experience" />
      <div
        class="mt-12 max-w-lg mx-auto grid gap-5 lg:grid-cols-3 lg:max-w-none"
      >
        <Card title="Motoring.co.uk" :skills="[ 'Perl', 'XHTML', 'CSS' ]">
          <p>Motoring website which allows you to create a valuation and buy used cars.</p>
        </Card>
        <Card title="Regit.cars" :skills="[ 'Laravel', 'PHP', 'SCSS', 'HTML5', 'VueJS' ]">
          <p class="mb-4">This is the second generation of motoring.co.uk this site added many extra features such as a logged in portal and finance calculator and so on</p>
          <p>This was also a chance to update my skills to a modern stack.</p>
        </Card>
        <Card title="MMU" :skills="[ 'VueJS', 'NuxtJS', 'TailwindCSS', 'JS', 'Node' ]">
          <p>This is the latest company I have worked for which has gotten me to use a wide array of skills.</p>
        </Card>
      </div>
    </div>
  </div>
</template>

<script>
import Card from "@/components/Card.vue";
import SectionHeader from './SectionHeader.vue';
export default {
  components: { Card, SectionHeader },
};
</script>
