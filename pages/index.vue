<template>
  <div>
    <h1>Color mode:</h1>
    <select>
      <option value="system">System</option>
      <option value="light">Light</option>
      <option value="dark">Dark</option>
      <option value="sepia">Sepia</option>
    </select>
    <h1 class="text-3xl font-bold underline">Hola mundo</h1>
    <UIBaseLink />
    <UIColorSwitch />
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
}
</script>

<style>
body {
  background-color: #fff;
  color: #000c;
}

.dark-mode body {
  background-color: #091a28;
  color: #ebf4f1;
}

.sepia-mode body {
  background-color: #f1e7d0;
  color: #433422;
}
</style>
