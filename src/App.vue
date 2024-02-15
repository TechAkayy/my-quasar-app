<script setup lang="ts">
  import { useQuasar } from 'quasar'

  import 'uno.css'

  // Set brand
  const { setTheme } = useTheme()
  setTheme()

  const $q = useQuasar()
  $q.iconMapFn = (iconName) => {
    return {
      icon: `i-${iconName}`,
    }
  }
</script>

<template>
  <div class="q-pl-xl">
    <!-- <router-view /> -->
    <q-icon name="i-mdi-menu"></q-icon>
  </div>
</template>
