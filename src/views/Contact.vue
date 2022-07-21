<template>
  <div class="contact">
    <!-- <vue-aos animation-class="fadeIn animated">
      <div>Hello</div>
    </vue-aos>
    <h1 class="title" v-vue-aos="{ animationClass: 'fadeIn animated' }">
      Contact
    </h1> -->
    <form action="https://formspree.io/f/xvolegyo" method="POST">
      <label>
        <textarea name="name" placeholder="Your name goes here..."></textarea>
      </label>
      <label>
        <input
          type="email"
          name="email"
          placeholder="Your email goes here..."
        />
      </label>
      <label>
        <textarea
          name="message"
          placeholder="Your message goes here"
        ></textarea>
      </label>
      <!-- your other form fields go here -->
      <button
        type="submit"
        style="
          background-color: #333;
          border: none;
          font-size: 5rem;
          font-family: 'Rampart One';
          color: white;
        "
      >
        Send
      </button>
    </form>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
.contact {
  width: 100vw;
  height: 100vh;
  background-color: #333;
}
.title {
  margin-bottom: 10rem;
  padding-top: 5rem;
  font-family: Rampart One;
  font-size: 5rem;
}
form {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 2rem;
}
textarea {
  width: 30rem;
  height: 2rem;
  background-color: #333;
}
input {
  width: 30em;
  height: 2rem;
  background-color: #333;
}
</style>
