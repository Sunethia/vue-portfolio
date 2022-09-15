<template>
  <div class="footer">
    <div class="row">
      <div class="col">
        <a href="https://www.linkedin.com/in/sunethia-lawrence-83a82a247/"
          ><i class="fa-brands fa-linkedin-in"></i></a
        ><br />
        <a href="https://codepen.io/sunethia-lawrence"
          ><i class="fa-brands fa-codepen"></i> </a
        ><br />
        <i class="fa-regular fa-at">lawrencesunethia@gmail.com</i><br />
        <i class="fa-solid fa-phone">084 582 8653 </i><br />
      </div>
    </div>
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
  color: black;
}
p {
  color: black;
  font-family: Rampart One;
}
.col {
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
}
i {
  display: flex;
  align-items: center;
  justify-content: space-between;
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
