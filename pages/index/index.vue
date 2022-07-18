<template>
  <div class="flex flex-col">
    <div class="flex flex-col px-12 pt-36">
      <div class="flex">
        <h1
          class="
            transition
            duration-150
            delay-75
            text-6xl
            font-extrabold
            text-white
            -tracking-widest
             flex
             hover:animate-ping
          "
        >
        <!-- transition hover:rotate-180 hover:translate-y-2 hover:translate-x-1 -->
          <div class="mr-1">
            <span>H</span>
          </div>
            <!-- transition hover:rotate-180 hover:translate-y-2 hover:translate-x-1 -->
          <div class="mr-1">
          <span>i</span>
          </div>
          <span>,</span>
          <!-- Hi, -->
          <br />
        </h1>
        <h1 class="text-6xl font-extrabold text-white ml-4 hover:animate-bounce">I am Elyas</h1>
      </div>
      <div class="flex flex-col relative">
          <h1 class="text-6xl font-extrabold text-white">I am a full-stack developer.</h1>
          <h1 class="transition text-6xl font-extrabold text-white absolute  hover:blur">I am a full-stack developer.</h1>
          <!-- :class="blurClass"  -->
          <!-- <div
          class="transition w-full blur h-28 bg-red-500 absolute opacity-50 hover:blur-2xl"></div> -->
      </div>
    </div>
    <div class="flex flex-col px-12 pt-36">
      <div class="flex">
        <h1
          class="
            transition
            duration-150
            delay-75
            text-6xl
            font-extrabold
            text-white
            -tracking-widest
             flex
             hover:animate-ping
          "
        >
        <!-- transition hover:rotate-180 hover:translate-y-2 hover:translate-x-1 -->
          <div class="mr-1">
            <span>H</span>
          </div>
            <!-- transition hover:rotate-180 hover:translate-y-2 hover:translate-x-1 -->
          <div class="mr-1">
          <span>i</span>
          </div>
          <span>,</span>
          <!-- Hi, -->
          <br />
        </h1>
        <h1 class="text-6xl font-extrabold text-white ml-4 hover:animate-bounce">I am Elyas</h1>
      </div>
      <div class="flex flex-col relative">
          <h1 class="text-6xl font-extrabold text-white">I am a full-stack developer.</h1>
          <h1 class="transition text-6xl font-extrabold text-white absolute  hover:blur">I am a full-stack developer.</h1>
          <!-- :class="blurClass"  -->
          <!-- <div
          class="transition w-full blur h-28 bg-red-500 absolute opacity-50 hover:blur-2xl"></div> -->
      </div>
    </div>
    <div class="flex flex-col px-12 pt-36">
      <div class="flex">
        <h1
          class="
            transition
            duration-150
            delay-75
            text-6xl
            font-extrabold
            text-white
            -tracking-widest
             flex
             hover:animate-ping
          "
        >
        <!-- transition hover:rotate-180 hover:translate-y-2 hover:translate-x-1 -->
          <div class="mr-1">
            <span>H</span>
          </div>
            <!-- transition hover:rotate-180 hover:translate-y-2 hover:translate-x-1 -->
          <div class="mr-1">
          <span>i</span>
          </div>
          <span>,</span>
          <!-- Hi, -->
          <br />
        </h1>
        <h1 class="text-6xl font-extrabold text-white ml-4 hover:animate-bounce">I am Elyas</h1>
      </div>
      <div class="flex flex-col relative">
          <h1 class="text-6xl font-extrabold text-white">I am a full-stack developer.</h1>
          <h1 class="transition text-6xl font-extrabold text-white absolute  hover:blur">I am a full-stack developer.</h1>
          <!-- :class="blurClass"  -->
          <!-- <div
          class="transition w-full blur h-28 bg-red-500 absolute opacity-50 hover:blur-2xl"></div> -->
      </div>
    </div>
    <div class="flex flex-col px-12 pt-36">
      <div class="flex">
        <h1
          class="
            transition
            duration-150
            delay-75
            text-6xl
            font-extrabold
            text-white
            -tracking-widest
             flex
             hover:animate-ping
          "
        >
        <!-- transition hover:rotate-180 hover:translate-y-2 hover:translate-x-1 -->
          <div class="mr-1">
            <span>H</span>
          </div>
            <!-- transition hover:rotate-180 hover:translate-y-2 hover:translate-x-1 -->
          <div class="mr-1">
          <span>i</span>
          </div>
          <span>,</span>
          <!-- Hi, -->
          <br />
        </h1>
        <h1 class="text-6xl font-extrabold text-white ml-4 hover:animate-bounce">I am Elyas</h1>
      </div>
      <div class="flex flex-col relative">
          <h1 class="text-6xl font-extrabold text-white">I am a full-stack developer.</h1>
          <h1 class="transition text-6xl font-extrabold text-white absolute  hover:blur">I am a full-stack developer.</h1>
          <!-- :class="blurClass"  -->
          <!-- <div
          class="transition w-full blur h-28 bg-red-500 absolute opacity-50 hover:blur-2xl"></div> -->
      </div>
    </div>
  </div>
</template>

<script>
export default {
    data(){
        return{
            blurClass: 'blur-3xl',
        }
    },
    created(){
        setInterval(()=> {
            this.blurClass = 'blur-2xl'
        }, 1000)
    }
};
</script>

<style scoped>
</style>