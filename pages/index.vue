<template>
  <div class="container">
    <!-- side desktop view -->
    <aside class="sticky md:w-1/5 lg:w-1/6 xl:w-1/12 h-screen top-0 md:bg-black md:flex md:flex-col hidden md:overflow-y-auto">
      <!-- Name, Initial and postion section -->
      <div class="flex flex-col justify-center items-center mt-4">
        <!-- My Initial with glow shadow -->
        <div class="flex justify-center">
          <h1 class="text-8xl font-bold text-cyan-300 self-center">E</h1>
          <h1 class="text-8xl font-bold text-rose-600 -ml-14 -mt-2 self-center">
            E
          </h1>
        </div>
        <!-- My name -->
        <h1 class="text-white font-bold text-2xl mb-1">Elyas</h1>
        <!-- My job -->
        <h1 class="text-white text-opacity-60 text-xs mb-5 font-semibold">
          Full Stack Developer
        </h1>
      </div>
      <!-- Menu section -->
      <div class="flex flex-col bg-white bg-opacity-5 h-full">
        <!-- List of sections -->
        <nuxt-link
          @click.native="activeSection = 'about'"
          :class="{ active: activeSection === 'about' }"
          to="/about"
          class="
            text-white text-center
            py-3
            text-opacity-50
            border-y border-white border-opacity-10
            mt-14
          "
        >
          About</nuxt-link
        >
        <nuxt-link
          @click.native="activeSection = 'myskills'"
          :class="{ active: activeSection === 'myskills' }"
          to="/myskills"
          class="
            text-white text-center
            py-3
            text-opacity-50
            border-b border-white border-opacity-10
          "
        >
          My skills</nuxt-link
        >
        <nuxt-link
          @click.native="activeSection = 'work'"
          :class="{ active: activeSection === 'work' }"
          to="/work"
          class="
            text-white text-center
            py-3
            text-opacity-50
            border-b border-white border-opacity-10
          "
        >
          Work</nuxt-link
        >
        <nuxt-link
          @click.native="activeSection = 'contact'"
          :class="{ active: activeSection === 'contact' }"
          to="/contact"
          class="
            text-white text-center
            py-3
            text-opacity-50
            border-b border-white border-opacity-10
          "
        >
          Contact</nuxt-link
        >
        <nuxt-link
          @click.native="activeSection = 'blog'"
          :class="{ active: activeSection === 'blog' }"
          to="/"
          class="
            text-white text-center
            py-3
            text-opacity-50
            border-b border-white border-opacity-10
          "
        >
          Blog</nuxt-link
        >
        <!-- Social links side by side -->
        <div class="flex justify-center items-center mt-10 gap-x-4">
          <!-- linkedin icon -->
          <a
            href="https://www.linkedin.com/in/elyas-mohamed-b8a8b817b/"
            target="_blank"
            class="text-white text-opacity-50 py-3 text-center"
          >
            <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
              <path
                d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"
              />
            </svg>
          </a>
          <!-- github icon -->
          <a
            href="https://www.github.com/elyas-demeke/"
            target="_blank"
            class="text-white text-opacity-50 py-3 text-center"
          >
            <svg
              aria-hidden="true"
              fill="currentColor"
              class="octicon octicon-mark-github"
              height="24"
              version="1.1"
              viewBox="0 0 16 16"
              width="24"
            >
              <path
                fill-rule="evenodd"
                d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"
              ></path>
            </svg>
          </a>
          <!-- tiktok icon -->
          <a
            href="https://www.linkedin.com/in/elyas-demeke/"
            target="_blank"
            class="text-white text-opacity-50 py-3 text-center"
          >
            aa<i class="fas fas-upload text-red-400"></i>
          </a>
        </div>
      </div>
    </aside>
    <!-- Hamburger -->
    <button
      class="
        p-4
        absolute
        border-none
        rounded-md
        bg-gray-800
        text-white
        hover:bg-gray-600
        transition
        top-4
        left-4
        z-40
        md:hidden
      "
      @click="showSideNavBar = true"
    >
      hamburger
    </button>

    <!-- side mobile view -->
    <aside
      :class="showSideNavBar ? 'translate-x-0 ' : '-translate-x-96 '"
      class="transition duration-300 w-1/2 min-h-screen bg-black flex flex-col md:hidden absolute z-50 top-0"
    >
      <!-- Name, Initial and postion section -->
      <div class="flex flex-col justify-center items-center mt-4">
        <!-- My Initial with glow shadow -->
        <div class="flex justify-center">
          <h1 class="text-8xl font-bold text-cyan-300 self-center">E</h1>
          <h1 class="text-8xl font-bold text-rose-600 -ml-14 -mt-2 self-center">
            E
          </h1>
        </div>
        <!-- My name -->
        <h1 class="text-white font-bold text-2xl mb-1">Elyas</h1>
        <!-- My job -->
        <h1 class="text-white text-opacity-60 text-xs mb-5 font-semibold">
          Full Stack Developer
        </h1>
      </div>
      <!-- Menu section -->
      <div class="flex flex-col bg-white bg-opacity-5 h-full">
        <!-- List of sections -->
        <nuxt-link
          @click.native="activeSection = 'about'; showSideNavBar = false"
          :class="{ active: activeSection === 'about' }"
          to="/about"
          class="
            text-white text-center
            py-3
            text-opacity-50
            border-y border-white border-opacity-10
            mt-14
          "
        >
          About</nuxt-link
        >
        <nuxt-link
          @click.native="activeSection = 'myskills'; showSideNavBar = false"
          :class="{ active: activeSection === 'myskills' }"
          to="/myskills"
          class="
            text-white text-center
            py-3
            text-opacity-50
            border-b border-white border-opacity-10
          "
        >
          My skills</nuxt-link
        >
        <nuxt-link
          @click.native="activeSection = 'work'; showSideNavBar = false"
          :class="{ active: activeSection === 'work' }"
          to="/work"
          class="
            text-white text-center
            py-3
            text-opacity-50
            border-b border-white border-opacity-10
          "
        >
          Work</nuxt-link
        >
        <nuxt-link
          @click.native="activeSection = 'contact'; showSideNavBar = false"
          :class="{ active: activeSection === 'contact' }"
          to="/contact"
          class="
            text-white text-center
            py-3
            text-opacity-50
            border-b border-white border-opacity-10
          "
        >
          Contact</nuxt-link
        >
        <nuxt-link
          @click.native="activeSection = 'blog'; showSideNavBar = false"
          :class="{ active: activeSection === 'blog' }"
          to="/"
          class="
            text-white text-center
            py-3
            text-opacity-50
            border-b border-white border-opacity-10
          "
        >
          Blog</nuxt-link
        >
        <!-- Social links side by side -->
        <div class="flex justify-center items-center mt-10 gap-x-4">
          <!-- linkedin icon -->
          <a
            href="https://www.linkedin.com/in/elyas-mohamed-b8a8b817b/"
            target="_blank"
            class="text-white text-opacity-50 py-3 text-center"
          >
            <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24">
              <path
                d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"
              />
            </svg>
          </a>
          <!-- github icon -->
          <a
            href="https://www.github.com/elyas-demeke/"
            target="_blank"
            class="text-white text-opacity-50 py-3 text-center"
          >
            <svg
              aria-hidden="true"
              fill="currentColor"
              class="octicon octicon-mark-github"
              height="24"
              version="1.1"
              viewBox="0 0 16 16"
              width="24"
            >
              <path
                fill-rule="evenodd"
                d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0 0 16 8c0-4.42-3.58-8-8-8z"
              ></path>
            </svg>
          </a>
          <!-- tiktok icon -->
          <a
            href="https://www.linkedin.com/in/elyas-demeke/"
            target="_blank"
            class="text-white text-opacity-50 py-3 text-center"
          >
            aa<i class="fas fas-upload text-red-400"></i>
          </a>
        </div>
      </div>
    </aside>
    <!-- main section desktop view -->
    <section
      class="md:w-4/5 lg:w-5/6 xl:w-11/12 md:h-full md:bg-black md:opacity-90 md:flex hidden"
    >
      <nuxt-child class="w-full h-full"/>
    </section>
    <!-- main section mobile view -->
    <section class="w-full min-h-screen bg-black opacity-90 md:hidden overflow-y-auto" @click="showSideNavBar = false">
      <nuxt-child />
    </section>
  </div>
</template>

<script>
export default {
  async asyncData({ $http }) {
    const test = await $http.$get("/api/test");
    return {
      test,
    };
  },
  data() {
    return {
      activeSection: "blog",
      showSideNavBar: false,
    };
  },
  created() {
    if (this.$route.path === "/") {
      this.activeSection = "blog";
    } else {
      this.activeSection = this.$route.path.slice(1);
    }
    console.log(this.activeSection);
  },
};
</script>

<style scoped>
.container {
  @apply min-w-full  min-h-screen  flex flex-col md:flex-row overflow-y-clip;/* md:overflow-x-hidden overflow-x-scroll;*/
}
.active {
  @apply text-teal-300 font-bold;
}
</style>
