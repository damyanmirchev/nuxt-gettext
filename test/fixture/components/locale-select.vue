<script>
export default {
    name: 'LocaleSelect'
}
</script>

<template>
  <div class="locale-select">
    <a
      v-for="(l, k) in $language.available"
      :key="k"
      href="javascript:void(0);"
      @click="$language.current = k"
    >
      {{ l }}
    </a>
  </div>
</template>

<style>
  .locale-select > a {
    padding: 2px 4px;
    margin: 0 3px;
  }
</style>
