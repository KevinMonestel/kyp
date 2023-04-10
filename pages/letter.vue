<template>
  <div class="h-screen w-screen flex justify-center items-center">

    <div class="flex flex-col rounded-lg bg-white shadow-lg md:max-w-xl md:flex-row">
      <img class="h-96 w-full rounded-t-lg object-cover md:h-auto md:w-64 md:rounded-none md:rounded-l-lg" src="/foto.jfif"
        alt="" />
      <div class="flex flex-col justify-start p-6">
        <h1 class="text-center text-2xl p-2"><strong>¡El amor de mi vida eres tú, por siempre, para siempre!</strong></h1>
        <hr>
        <p class="text-center p-1">Mi amor, este pequeño sitio es una muestra de que siempre quiero llegar a tu corazón donde
          seas que estés.
          Quiero decirte lo mucho que te amo, lo mucho que me completas y lo grandioso que ha sido este primer mes junto a
          ti.
          Deseo que pasemos una vida juntos llena de muchas cosas lindas por vivir. Por ello, guardemos esto, como muestra de nuestro amor en este camino que empieza.
        </p>
        <hr>
        <h3 class="text-center p-2"><strong>TE AMO CON TODO MI CORAZÓN MI AMOR 🧡</strong></h3>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
const audio = ref(new Audio('/fae.mp3'));

onMounted(() => {
  audio.value.volume = 0.01;

  audio.value.play();
})

onUnmounted(() => {
  audio.value.volume = 0;
})
</script>

<style scoped></style>