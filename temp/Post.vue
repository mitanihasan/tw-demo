<script setup>
const post = {
  image: 'https://images.unsplash.com/photo-1495474472287-4d71bcdd2085',
  title: '5 Easy Tips That Will Make Your Latte Art Flourish',
  description:
    'Latte art is quite often the most attractive thing for a new barista, and latte art is an excellent gateway to the exciting world of coffee. Latte art easy to start with, but to master latte art patterns, you need a lot practice and determination. Here are my tips that helped me to improve my latte art a few years ago!',
};
</script>
<template>
  <section class="bg-gray-100 dark:bg-gray-900 py-10 px-12">
    <div
      class="grid grid-flow-row gap-8 text-neutral-600 sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4"
    >
      <!-- Card Item -->
      <div
        class="my-8 rounded shadow-lg shadow-gray-200 dark:shadow-gray-900 bg-white dark:bg-gray-800 duration-300 hover:-translate-y-1"
      >
        <!-- Clickable Area -->
        <a _href="link" class="cursor-pointer">
          <figure>
            <!-- Image -->
            <img :src="post.image" class="rounded-t h-72 w-full object-cover" />

            <figcaption class="p-4">
              <!-- Title -->
              <p
                class="text-lg mb-4 font-bold leading-relaxed text-gray-800 dark:text-gray-300"
              >
                {{ post.title }}
                <!-- Post Title -->
              </p>

              <!-- Description -->
              <small class="leading-5 text-gray-500 dark:text-gray-400">
                {{ post.description }}
                <!-- Post Description -->
              </small>
            </figcaption>
          </figure>
        </a>
      </div>
    </div>
  </section>
</template>
