<template>
<div class="container">
  <main class="main d-flex justify-center flex-column align-center text-center">
    <h1 class="main__heading">n|u</h1>
    <h2 class="main__sub main__sub--1">welcome to null</h2>
    <h2 class="main__sub main__sub--2">The open security community</h2>
    <p class="main__info">
     null is India's largest open security community. Registered as a non-profit society in 2010, 
     we have been active since even before that. null is about spreading information security awareness. 
     All our activities such as null Monthly Meets, null Humla, null Bachaav, null Puliya, null Job Portal 
     are for the cause of that.
    </p>
    <div class="main__actions">
      <v-btn color="blue" class="cta" outlined rounded>
        <img src="../assets/images/null.svg" alt="null community" class="icon">
        join the null community
      </v-btn>
      <v-btn color="red" class="cta" outlined rounded>
        <v-icon dark>mdi-vertical-dots</v-icon>
        Sign in with google
      </v-btn>
    </div>
  </main>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss">
.main {
  height: 100vh;
  align-items: flex-start;

  &__heading{
    font-size: 8rem;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    font-weight: 300;
    margin-top: -15rem;
  }

  &__sub{
    font-weight: 300;

    &--1{
      font-size: 3rem;
    }

    &--2{
      font-size: 2.5rem;
      margin-bottom: 2rem;
    }
  }

  &__info{
    max-width: 55%;
  }

  &__actions{
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    // justify-content: space-around;
    margin-top: 2rem;

    & > * {
      margin: 0 1rem;
      display: flex;
      align-items: center;
      justify-content: center;
    }
  }

  &__typewriter {
    font-family: monospace;
    overflow: hidden;
    white-space: nowrap;
    margin: 0 auto;
    letter-spacing: 0.17em;
    animation: typing 3.5s steps(30, end), step-end infinite;
    animation-fill-mode: forwards;
  }
}

.icon{
  height: 2rem;
  margin-right: .5rem;
  filter: invert(1);
}

/* The typing effect */
@keyframes typing {
  from {
    width: 0;
  }
  to {
    width: 100%;
  }
}
</style>
