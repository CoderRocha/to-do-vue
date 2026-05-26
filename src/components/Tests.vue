<script setup>
// hmr module replacement
// hot reload
import { ref } from 'vue'

const title = ref('Hello World 3!')
const showTitle = ref(true)
// diretivas

const score = ref(0)

const showMore = ref(false)
</script>

<template>
  <!-- <div>
    <h1 v-if="showTitle">{{ title }}</h1>
  </div> -->

  <!-- <div v-if="score === 0">
    Comece a jogar!
  </div>

  <div v-else-if="score > 0 && score < 50">
    Continue assim!
  </div>

  <div v-else-if="score >= 50 && score < 100">
    Quase lá!
  </div>

  <div v-else>
    Finalmente!
  </div> -->

  <div>
    <div>
      <p>Lorem ipsum</p>

      <p v-show="showMore">Ipsum Lorum</p>

      <a>Ver mais</a>
    </div>
  </div>

</template>
