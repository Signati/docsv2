<script setup>
const packages = [
  {
    name: "@cfdi/xml",
    icon: "xml",
    description:
      "Libreria para crear y sellar xml cfdi V4.0 de forma mas sencilla y rapida",
  },
  {
    name: "@cfdi/complementos",
    icon: "xml",
    description:
      "Libreria para generar los complementos",
  },
  {
    name: "@cfdi/csd",
    icon: "csd",
    description:
      "Libreria para obtener datos de los Certificado de Sello Digital",
  },
  {
    name: "@cfdi/catalogos",
    icon: "csd",
    description: "Libreria para centralizar informacion de catalos del SAT",
  },
  {
    name: "@cfdi/utils",
    icon: "csd",
    description:
      "Libreria  para poder ayudar a la creacion del xml cfdi V4, exponiendo metodos",
  },
  {
    name: "@cfdi/pdf",
    icon: "csd",
    description: "En desarrollo",
  },
  {
    name: "@cfdi/curp",
    icon: "csd",
    description: "En desarrollo",
  },
  {
    name: "@cfdi/csf",
    icon: "csd",
    description: "Estado en beta",
  },
  {
    name: "@cfdi/rfc",
    icon: "csd",
    description: "En desarrollo",
  },
];
</script>

<template>
  <h5
    class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white"
  >
    <a href="https://cfdi.recreando.dev">Ir a Nueva Documentacion</a>
  </h5>
   <h5
    class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white"
  >
    Recientemente se a migrado de @signati/core a @cfdi/xml
  </h5>
  <div class="grid xs:grid-cols-1  sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-4">
    <div v-for="(lib, i) of packages" :key="i">
      <a
        href="#"
        :key="i"
        class="block max-w-sm p-6 bg-white border border-gray-200 rounded-lg shadow hover:bg-gray-100 dark:bg-gray-800 dark:border-gray-700 dark:hover:bg-gray-700"
      >
        <h5
          class="mb-2 text-2xl font-bold tracking-tight text-gray-900 dark:text-white"
          style="color: #3fcf8e"
        >
          {{ lib.name }}
        </h5>
        <p class="font-normal text-gray-700 dark:text-gray-400">
          {{ lib.description }}
        </p>
      </a>
    </div>
  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
