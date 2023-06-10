<template>
  <div>
    <Teleport to="body">
      <div class="promote">
        <p>This is a promotion</p>
      </div>
    </Teleport>
  </div>
</template>

<script>
export default {
  name: "PromotionComponent",
};
</script>
<style scoped>
.promote {
  position: fixed;
  top: 10%;
  left: 40%;
  background-color: red;
  margin-left: -150px;
  margin-right: auto;
  text-align: center;
  width: 600px;
}
</style>
