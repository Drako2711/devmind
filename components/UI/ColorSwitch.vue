<template>
  <div>
    {{ $colorMode.preference }}
    <IconDark
      v-if="$colorMode.preference === 'dark'"
      @click="changeTheme('light')"
    />
    <IconLight else @click="changeTheme('dark')" />
  </div>
</template>

<script>
export default {
  name: 'ColorSwitch',
  components: {
    IconDark: () => import('@/assets/icons/Moon.svg?inline'),
    IconLight: () => import('@/assets/icons/Sun.svg?inline'),
  },
  methods: {
    changeTheme(theme) {
      this.$colorMode.preference = theme
    },
  },
}
</script>
