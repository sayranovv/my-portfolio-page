<script setup lang="ts">

const projects = [
  {
    id: 1,
    title: "ToDo List App",
    description: "every frontend developer in pet projects should have a todo list app, isn't it? this one is with cloud saving yeah",
    link: "https://github.com/sayranovv/todo-list-app"
  },
  {
    id: 2,
    title: "GIBDD Registration",
    description: "this is just a final checkpoint on the subject Python in the first semester at PSU",
    link: "https://github.com/sayranovv/traffic-police-registration"
  },
  {
    id: 3,
    title: "Telegram Mini App",
    description: "This is a mini-application (tap-game), which works through the tg bot",
    link: "https://github.com/sayranovv/telegram-mini-app-vue"
  },
  {
    id: 4,
    title: "CRM System",
    description: "This is a CRM system written in Vue.js, using Nuxt.js",
    link: "https://github.com/sayranovv/crm-system-nuxt"
  },
  {
    id: 5,
    title: "Online sneaker Store",
    description: "Online sneaker store on Vue3",
    link: "https://github.com/sayranovv/vue-sneakers-online-store"
  },
  {
    id: 6,
    title: "Tic-Tac-Toe",
    description: "the game tic-tac-toe, well, everything is sort of...",
    link: "https://github.com/sayranovv/tic-tac-toe-vue3"
  },
]
</script>

<template>
<div>
  <ul class="text-right">
    <li v-for="project in projects" :key="project.id" class="hover:text-neutral-300 transition-colors max-w-xl mt-8">
      <a :href="project.link">
        <h3 class="text-6xl font-thin uppercase">{{ project.title }}</h3>
        <p class="mt-1 font-bold">{{ project.description }}</p>
      </a>
    </li>
  </ul>
</div>
</template>

<style scoped>

</style>