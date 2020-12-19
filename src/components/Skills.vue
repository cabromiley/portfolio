<template>
    <!-- This example requires Tailwind CSS v2.0+ -->
    <div class="bg-gray-50">
    <div class="max-w-7xl mx-auto py-16 px-4 sm:px-6 lg:py-16 lg:px-8">
        <section-header header="What can I provide for you" />
        <dl class="mt-12 space-y-10 sm:space-y-0 sm:grid sm:grid-cols-2 sm:gap-x-6 sm:gap-y-12 lg:grid-cols-4 lg:gap-x-8">
            <SkillItem header="API">
                Build and consume apis for your web projects
            </SkillItem>

            <SkillItem header="Web Components">
                Build out your web pages in a modular fashion so that everything is reusable
            </SkillItem>

            <SkillItem header="Static Websites">
                Build out your applications in a static application to reduce running costs and improve web page performance
            </SkillItem>

            <SkillItem header="Dynamic Websites">
                For your more complex application needs such as authentication and so on
            </SkillItem>

            <SkillItem header="Modern frameworks">
                To gain all the latest features such as performance and imrpoved security.
            </SkillItem>

            <SkillItem header="SEO optimisation">
                To improve your score on popular search engines such as google and bing
            </SkillItem>
            
            <SkillItem header="Unit Testing">
                So your web applications does exactly what you expect it to do.
            </SkillItem>
                        
            <SkillItem header="Devops">
                To automate deployment of your applications/web sites
            </SkillItem>
        </dl>
    </div>
    </div>
</template>

<script>
import SkillItem from "@/components/SkillItem.vue"
import SectionHeader from './SectionHeader.vue'

export default {
    components: { SkillItem, SectionHeader }
}
</script>