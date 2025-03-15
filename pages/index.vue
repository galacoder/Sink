<script setup>
// No additional script needed - dark mode is handled automatically by Tailwind using the prefers-color-scheme media query
</script>

<template>
  <main class="flex flex-col min-h-screen transition-colors duration-200 bg-gray-50 dark:bg-gray-900">
    <!-- Header Section -->
    <header class="container px-4 pt-8 mx-auto">
      <div class="flex items-center justify-between">
        <div class="flex items-center">
          <!-- Updated to use the provided logo -->
          <img src="/assets/images/galatek-logo.png" alt="Galatek Logo" class="w-auto h-12">
        </div>
      </div>
    </header>

    <!-- Main Content Section -->
    <section class="container flex-grow px-4 py-16 mx-auto">
      <div class="max-w-3xl p-8 mx-auto transition-colors duration-200 bg-white shadow-sm dark:bg-gray-800 rounded-3xl">
        <!-- Updated headline with Russell Brunson-style copy -->
        <h2 class="mb-6 text-4xl font-black tracking-tight text-transparent bg-clip-text bg-gradient-to-r from-blue-500 to-orange-500">
          You're Just One Step Away From Your Digital Breakthrough
        </h2>

        <!-- Updated opening paragraph -->
        <p class="mb-6 text-xl font-bold text-gray-800 dark:text-gray-200">
          You've discovered Galatek's special link shortening system—the same technology that's helped our clients generate millions in revenue with lightning-fast marketing campaigns. While this is our internal tool, what you really need is just on the other side.
        </p>

        <div class="mb-8">
          <h3 class="mb-3 text-2xl font-bold text-gray-900 dark:text-white">
            To access a shortened link, please use the complete URL format:
          </h3>
          <div class="p-4 font-mono text-lg text-gray-800 bg-gray-100 rounded-lg dark:text-gray-200 dark:bg-gray-700">
            up.galatek.dev/<span class="font-bold text-blue-600 dark:text-blue-400">[your-unique-code]</span>
          </div>
        </div>

        <!-- Callout Box -->
        <div class="p-6 mb-8 border border-blue-200 dark:border-blue-800 bg-blue-50 dark:bg-blue-900/30 rounded-xl">
          <h3 class="mb-3 text-xl font-bold text-gray-900 dark:text-white">
            Did you receive a shortened link?
          </h3>
          <p class="mb-4 text-gray-800 dark:text-gray-200">
            Make sure to include the unique code after the slash.
          </p>

          <div class="flex flex-col space-y-2">
            <div class="flex items-center">
              <svg class="w-5 h-5 mr-2 text-green-600 dark:text-green-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
              </svg>
              <span class="font-semibold text-gray-900 dark:text-white">Correct: <code class="px-2 py-1 text-white bg-gray-700 rounded dark:bg-gray-600">up.galatek.dev/sales2024</code></span>
            </div>
            <div class="flex items-center">
              <svg class="w-5 h-5 mr-2 text-red-600 dark:text-red-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
              </svg>
              <span class="font-semibold text-gray-900 dark:text-white">Incorrect: <code class="px-2 py-1 text-white bg-gray-700 rounded dark:bg-gray-600">up.galatek.dev</code></span>
            </div>
          </div>
        </div>

        <!-- Enhanced story-driven Internal Tool Notice section -->
        <div class="p-6 border border-gray-200 dark:border-gray-700 rounded-xl bg-gray-50 dark:bg-gray-700/50">
          <h3 class="mb-3 text-xl font-bold text-gray-900 dark:text-white">
            What If You Could Put YOUR Business In The Fast Lane Too?
          </h3>
          <p class="mb-4 text-gray-800 dark:text-gray-200">
            Every day, entrepreneurs struggle with slow product launches, ineffective marketing, and wasted resources—just like I did before discovering the formula that changed everything.
          </p>
          <p class="mb-4 text-gray-800 dark:text-gray-200">
            After 13+ years and 250+ successful projects, our team has developed a system that's helped businesses just like yours achieve results in months, not years.
          </p>
          <p class="mb-6 font-semibold text-gray-800 dark:text-gray-200">
            The secret isn't in the links—it's in our unique approach to technology and marketing that puts your business on the express route to success.
          </p>

          <!-- Moving CTA button here with enhanced effects -->
          <div class="mt-8 text-center">
            <a href="https://galatek.dev" class="inline-block px-8 py-4 text-lg font-bold text-white transition-all duration-300 transform rounded-full bg-gradient-to-r from-blue-600 to-orange-500 hover:from-blue-700 hover:to-orange-600 hover:shadow-lg hover:shadow-orange-500/30 hover:-translate-y-1 hover:scale-105 animate-pulse-subtle">
              <span class="flex items-center">
                Discover The System That's Transforming Businesses Right Now
                <svg class="w-5 h-5 ml-2 transition-transform duration-300 transform group-hover:translate-x-1" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3" />
                </svg>
              </span>
            </a>
          </div>
        </div>
      </div>
    </section>

    <!-- Footer Section with copyright only -->
    <footer class="container px-4 py-8 mx-auto border-t border-gray-200 dark:border-gray-700">
      <div class="flex justify-center md:justify-end">
        <div class="mx-auto text-sm text-gray-800 dark:text-gray-300">
          © {{ new Date().getFullYear() }} Galatek. All rights reserved.
        </div>
      </div>
    </footer>
  </main>
</template>

<style>
/* Ensure dark mode works with system preferences */
@media (prefers-color-scheme: dark) {
  html.dark-mode {
    color-scheme: dark;
  }
}

/* Add subtle pulse animation for the CTA button */
@keyframes pulse-subtle {
  0%, 100% {
    opacity: 1;
  }
  50% {
    opacity: 0.9;
  }
}

.animate-pulse-subtle {
  animation: pulse-subtle 2s ease-in-out infinite;
}
</style>
