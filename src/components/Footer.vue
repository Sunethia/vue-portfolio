<template>
  <div class="footer">
    <i class="fa-solid fa-at">-lawrencesunethia@gmail.com</i>

    <i class="fa-solid fa-phone">-084 582 8653</i>

    <i class="fa-brands fa-facebook">-Sunethia Lawrence</i>
    <i class="fa-brands fa-linkedin">-Sunethia Lawrence</i>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
.footer {
  height: 20vh;
  background-color: white;
  border: 1px solid transparent;
  padding-top: 5rem;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 3rem;
  color: white;
}
p {
  color: white;
  font-family: Rampart One;
}
twofoot {
  background-color: white;
}
/* media queries */
@media (min-width: 300px) and (max-width: 616px) {
  p {
    font-size: 1rem;
  }
  i {
    font-size: 1rem;
  }
}
</style>
