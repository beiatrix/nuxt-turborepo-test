<script setup lang="ts">
import { add } from "math-helpers-test";
import { Page } from "ui";

const config = useRuntimeConfig()
const { appName } = config.public

useHead({
  title: "Create Turborepo (vue-nuxt:docs)",
  meta: [{ name: "description", content: "Generated by create turbo" }],
});
</script>

<template>
  <Page :app-name="`${appName} - ${add(1, 2)} - :)`" />
</template>
