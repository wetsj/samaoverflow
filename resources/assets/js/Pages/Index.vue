<template>
  <div>
    <hero class="hero--full">
      <template #header>
        <navbar dark />
      </template>
      <template #body>
        <div class="lg:grid lg:grid-cols-2 lg:gap-4 lg:content-center">
          <div class="text-center lg:text-left lg:flex lg:flex-col lg:justify-center lg:items-start space-y-7">
            <h1 class="hero__leading">Learn. Share. Build</h1>
            <p class="max-w-prose opacity-80">
              A community-based space to find and contribute answers to technical challenges, and one of the most
              popular websites in the world.
            </p>
            <div class="flex flex-col xl:flex-row space-y-6 md:space-y-4 xl:space-x-4">
              <p>
                <Link :href="route('register')" class="button button--primary button--xl">
                  Join the community
                  <font-awesome-icon class="ml-1.5" icon="fa-solid fa-arrow-right" />
                </Link>
              </p>
              <p>
                <Link
                  :href="route('questions.index')"
                  class="md:text-sm underline hover:text-yellow-400 focus:text-primary-500 active:text-yellow-500"
                >
                  or continue browsing the website
                </Link>
              </p>
            </div>
          </div>
          <img class="hidden lg:inline rounded-lg shadow" src="img/index/small.png" alt="test" />
        </div>
      </template>
      <template #footer>
        <p class="text-5xl text-center text-primary-100 opacity-50 mb-8 animate-bounce">
          <font-awesome-icon icon="fa-solid fa-circle-arrow-down" />
        </p>
      </template>
    </hero>
    <!--
    <section class="section">
      <div class="container space-y-8">
        <div class="card">
          <div class="card__header"></div>
          <div class="grid grid-cols-3 p-4 rounded w-full">
            <div>
              <h1 class="font-semibold">
                100+ million
              </h1>
              <p>
                monthly visitors to Stack Underflow
              </p>
            </div>
            <div>
              <h1 class="font-semibold">
                45.1+ billion
              </h1>
              <p>
                Times a developer got help since 2019
              </p>
            </div>
            <div>
              <h1 class="font-semibold">
                150+ billion
              </h1>
              <p>
                different answers accross the website
              </p>
            </div>
          </div>
          <div class="card__footer"></div>
        </div>
        <div class="rounded-lg p-8 bg-slate-900">
          <div class="grid grid-cols-2">
            <div>

            </div>
          </div>
        </div>
      </div>
    </section>
    -->
  </div>
</template>

<script>
import Hero from '@/Components/Home/Hero'
import Navbar from '@/Components/Navbar/Navbar'
import { Link } from '@inertiajs/inertia-vue'

export default {
  name: 'Index',
  components: { Navbar, Hero, Link },
}
</script>
