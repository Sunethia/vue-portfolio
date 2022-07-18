<template>
  <div class="contact">
    <h1>Contact</h1>
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
      <button type="submit">Send</button>
    </form>
  </div>
</template>
<script>
export default {};
</script>
<style>
.contact {
  width: 100vw;
  height: 100vh;
  background-color: #333;
}
form {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 2rem;
}
textarea {
  width: 20rem;
  height: 2rem;
  background-color: #333;
}
input {
  width: 20rem;
  height: 2rem;
  background-color: #333;
}
</style>
