<template>
  <v-container>
    <v-row>
      <v-col
        v-for="(garant, i) in garants"
        :key="i"
        justify="center"
        style="border-style: dashed"
        class="text-end"
      >
        <span>
          {{ garant.name }}
        </span>
        <a href="#" class="subheading mx-3" target="_blank">
          {{ garant.search }}
        </a>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "Home",
  data: () => ({
    garants: [
      {
        name: "good",
        search: "جستجو بر اساس کالا",
      },
      {
        name: "person",
        search: "جستجو بر اساس فرد",
      },
    ],
  }),
};
</script>

<style>
</style>