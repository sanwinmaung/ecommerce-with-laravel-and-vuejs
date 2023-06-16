<template>
    <div class="min-h-full flex">
        <!-- Sidebar -->
        <Sidebar />
        <!-- Sidebar -->


        <div class="flex-1">
            <TopHeader />

            <!-- Content -->
            <main>
                <router-view></router-view>
            </main>
            <!-- Content -->
        </div>
    </div>
</template>

<script setup>
import Sidebar from './Sidebar.vue';
import TopHeader from './TopHeader.vue';

const {title} = defineProps({
    title: String
})
const emit = defineEmits(['submit'])
</script>

<style scoped>
</style>