<template>
  <!-- Parent wrapper to span full height using Tailwind classes -->
  <div class="min-h-screen flex flex-col w-full bg-white dark:bg-gray-800">
    <el-header class="p-0 m-0">
      <!-- Header -->
      <HeaderComponent />
    </el-header>

    <el-container>
      <!-- Aside -->
      <AsideComponent />

      <!-- Main Content -->
      <el-main class="p-0 m-0">
        <TabView />
      </el-main>
    </el-container>

    <el-footer class="p-0 m-0">
      <!-- Footer -->
      <FooterComponent />
    </el-footer>
  </div>
</template>

<script setup lang="ts">
// Import your components
import HeaderComponent from '@/components/layout/HeaderComponent.vue'
import AsideComponent from '@/components/layout/AsideComponent.vue'
import FooterComponent from '@/components/layout/FooterComponent.vue'
import { ElContainer, ElMain } from 'element-plus'
// import MainComponent from '@/components/layout/MainComponent.vue'
import TabView from '@/components/tabs/TabView.vue'
</script>
