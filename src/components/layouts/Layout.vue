<script setup></script>

<template>
  <header>
    <h1 class="text-gradient">DIMGRAM</h1>
  </header>
  <main>
    <slot />
  </main>
  <footer>
    <small>Created by</small>
    <a href="https://github.com/DmytroAstakhov" target="_blank">
      <img src="/created-by.jpg" alt="pfp" />
      <p>DmytroAstakhov</p>
      <i class="fa-brands fa-github"></i>
    </a>
  </footer>
</template>

<style scoped>
header,
footer,
main {
  padding: 1rem;
  width: 100%;
  max-width: 600px;
  margin: 0 auto;
}

main {
  flex: 1;
}

footer {
  display: flex;
  flex-direction: column;
  gap: 0.5rem;
  align-items: center;
  padding: 2rem 0;
  padding-bottom: 4rem;
}

footer a {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  padding-block: 0.3rem;
  padding-inline: 0.5rem;
  background: var(--background-muted);
  border-radius: 4rem;
  border: 1px solid transparent;
  transition-duration: 0.2s;
  text-decoration: none;
}

footer a:hover {
  border-color: var(--color-link);
}

footer a img {
  max-width: 30px;
  aspect-ratio: 1 / 1;
  border-radius: 100%;
}
</style>
