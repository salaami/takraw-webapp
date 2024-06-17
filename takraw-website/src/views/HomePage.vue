<template>
  <div class="grid">
    <header>Header</header>
    <nav>Navigation</nav>
    <article>Article</article>
    <aside>Right Sidebar</aside>
    <footer>Footer</footer>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
  props: {
    title: String,
    description: String
  }
}
</script>

<style scoped>
:root {
  --primary:;
  --primary-lightest:;
  --primary-light:;
  --primary-dark:;
  --primary-darkest:;
  --grey-00:;
  --grey-10:;
  --grey-20:;
  --grey-30:;
  --grey-40:;
  --grey-50:;
  --grey-60:;
  --grey-70:;
  --grey-80:;
  --grey-90:;
  --grey-100:;
  --elevation-1:;
  --elevation-2:;
  --elevation-3:;
  --accent-1:;
  --accent-2:;
  --accent-3:;
  --highlight-1:;
  --highlight-2:;
  --highlight-3:;
}
@media(min-width: 320px){
  :root {
  --fs-huge: 3rem;
  --fs-big: 1.75rem;
  --fs-medium: 1.25rem;
  --fs-normal: 1rem;
  --fs-small: 0.75rem;
  --fs-tiny: 0.5rem;
  }
}

@media(min-width: 480px){
  :root {
  --fs-huge: 3.5rem;
  --fs-big: 1.75rem;
  --fs-medium: 1.25rem;
  --fs-normal: 1rem;
  --fs-small: 0.75rem;
  --fs-tiny: 0.5rem;
  }
}

@media(min-width: 768px){
  :root {
  --fs-huge: 6rem;
  --fs-big: 3rem;
  --fs-medium: 2rem;
  --fs-normal: 1.25rem;
  --fs-small: 1rem;
  --fs-tiny: 0.75rem;
  }
}

@media(min-width: 1024px){
  :root {
  --fs-huge: 6rem;
  --fs-big: 3rem;
  --fs-medium: 2rem;
  --fs-normal: 1.5rem;
  --fs-small: 1rem;
  --fs-tiny: 0.75rem;
  }
}

@media(min-width: 1200px){
  :root {
  --fs-huge: 6rem;
  --fs-big: 3rem;
  --fs-medium: 2rem;
  --fs-normal: 1.5rem;
  --fs-small: 1rem;
  --fs-tiny: 0.75rem;
  }
}

.grid {
  display: grid;
  grid-template-columns: repeat (3, 1fr);
  grid-template-rows: 30% 200px auto;
  grid-gap: 1em;
}

.grid > * {
  display: flex;
  align-items: center;
  justify-content: center;
}

header,
nav,
article,
aside,
footer {
  background: lightgray;
  padding: 1em;
}

header,
footer {
  grid-column: 1 / 4;
}

article {
  min-width: 15em;
}
</style>
