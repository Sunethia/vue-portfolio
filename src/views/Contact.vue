<template>
  <div class="contact">
    <h1>Contact</h1>
    <form action="https://formspree.io/f/xvolegyo" method="POST">
      <label>
        <textarea
          class="input"
          name="name"
          placeholder="Your name goes here..."
        ></textarea>
      </label>
      <label>
        <input
          class="input"
          type="email"
          name="email"
          placeholder="Your email goes here..."
        />
      </label>
      <label>
        <textarea
          class="input"
          name="message"
          placeholder="Your message goes here"
        ></textarea>
      </label>
      <!-- your other form fields go here -->
      <button
        type="submit"
        style="
          background-color: white;
          border: none;
          font-size: 5rem;
          font-family: 'Rampart One';
          color: black;
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
  background-color: white;
}
h1 {
  font-size: 5rem;
  font-family: "Rampart One";
  color: black;
  padding-bottom: 3rem;
  padding-top: 3rem;
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
  background-color: white;
}
input {
  width: 30em;
  height: 2rem;
  background-color: white;
}

@media (min-width: 300px) and (max-width: 520px) {
  .input {
    width: 400px;
  }
}
@media (min-width: 300px) and (max-width: 440px) {
  .input {
    width: 350px;
  }
  h1 {
    font-size: 3.5rem;
  }
}
@media (min-width: 300px) and (max-width: 388px) {
  .input {
    width: 300px;
  }
  h1 {
    font-size: 2rem;
  }
}
@media (min-width: 300px) and (max-width: 388px) {
  .input {
    width: 250px;
  }
  h1 {
    font-size: 1.8rem;
  }
}
</style>
