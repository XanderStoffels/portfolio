<script setup>
import { ref } from 'vue'

const count = ref(0)
</script>

<template>
  <div class="min-h-screen bg-base-100">
    <!-- Hero Section -->
    <div class="hero min-h-screen bg-gradient-to-br from-primary to-secondary">
      <div class="hero-content text-center">
        <div class="max-w-md">
          <h1 class="text-5xl font-bold text-primary-content">Vue 3 + Vite</h1>
          <p class="py-6 text-primary-content/80">
            A modern portfolio built with Vue 3, Vite, Tailwind CSS, and DaisyUI
          </p>
          <button class="btn btn-accent" @click="count++">
            Count is {{ count }}
          </button>
        </div>
      </div>
    </div>

    <!-- Features Section -->
    <div class="container mx-auto px-4 py-16">
      <h2 class="text-3xl font-bold text-center mb-8">Features</h2>
      <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
        <div class="card bg-base-100 shadow-xl">
          <div class="card-body">
            <h3 class="card-title text-primary">Vue 3</h3>
            <p>The progressive JavaScript framework</p>
            <div class="card-actions justify-end">
              <div class="badge badge-primary">Framework</div>
            </div>
          </div>
        </div>

        <div class="card bg-base-100 shadow-xl">
          <div class="card-body">
            <h3 class="card-title text-secondary">Tailwind CSS</h3>
            <p>Utility-first CSS framework</p>
            <div class="card-actions justify-end">
              <div class="badge badge-secondary">Styling</div>
            </div>
          </div>
        </div>

        <div class="card bg-base-100 shadow-xl">
          <div class="card-body">
            <h3 class="card-title text-accent">DaisyUI</h3>
            <p>Beautiful components for Tailwind CSS</p>
            <div class="card-actions justify-end">
              <div class="badge badge-accent">Components</div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Demo Section -->
    <div class="bg-base-200 py-16">
      <div class="container mx-auto px-4 text-center">
        <h2 class="text-3xl font-bold mb-8">DaisyUI Components Demo</h2>
        <div class="space-y-4">
          <div class="btn-group">
            <button class="btn btn-primary">Primary</button>
            <button class="btn btn-secondary">Secondary</button>
            <button class="btn btn-accent">Accent</button>
          </div>
          
          <div class="alert alert-info shadow-lg max-w-md mx-auto">
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" class="stroke-current shrink-0 w-6 h-6"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg>
            <span>This is a DaisyUI alert component!</span>
          </div>

          <div class="stats shadow">
            <div class="stat">
              <div class="stat-title">Total Page Views</div>
              <div class="stat-value">89,400</div>
              <div class="stat-desc">21% more than last month</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
