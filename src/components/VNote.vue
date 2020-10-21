<template>
  <div class="container-note">
    <p>DO</p>
    <p>RÉ</p>
    <p>MI</p>
    <p>FA</p>
    <p>SOL</p>
    <p>LA</p>
    <p>SI</p>
  </div>
</template>

<script>
export default {};
</script>

<style lang="postcss" scoped>
.container-note {
  display: flex;
  justify-content: space-around;
  width: 531px;
  margin-top: 48px;
  font-family: "PT Mono", monospace;
  color: rgba(255, 255, 255, 0.4);
}

@media (max-width: 700px) {
  .container-note {
    display: none;
  }
}
</style>