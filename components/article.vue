<template>
  <section class="article-card" v-bind:class="rootClassName">
    <main class="article-content">
      <header class="article-header1">
        <h1 class="article-header2">{{ header }}</h1>
      </header>
      <p class="article-description">{{ description }}</p>
      <div class="article-button">
        <a
          :href="buttonLink"
          target="_blank"
          rel="noreferrer noopener"
          class="article-link"
        >
          <p class="article-text">{{ button }}</p>
        </a>
      </div>
    </main>
  </section>
</template>

<script>
export default {
  name: 'Article',
  props: {
    rootClassName: String,
    button: {
      type: String,
      default: 'Read ->',
    },
    buttonLink: String,
    description: {
      type: String,
      default:
        'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor.',
    },
    header: {
      type: String,
      default: 'TechCrunch',
    },
  },
}
</script>

<style scoped>
.article-card {
  gap: var(--dl-space-space-oneandhalfunits);
  flex: 1;
  display: flex;
  padding: var(--dl-space-space-threeunits);
  position: relative;
  align-items: flex-start;
  border-radius: 20px;
  flex-direction: column;
  justify-content: flex-start;
  background-color: #292929;
}
.article-content {
  gap: var(--dl-space-space-twounits);
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  justify-content: flex-start;
}
.article-header1 {
  display: flex;
  align-items: flex-start;
  flex-direction: row;
  justify-content: flex-start;
}
.article-header2 {
  color: rgb(255, 255, 255);
  font-size: 24px;
  font-style: normal;
  font-family: Poppins;
  font-weight: 600;
  line-height: 36px;
}
.article-description {
  color: #C2C6CC;
  font-family: Poppins;
  line-height: 28px;
}
.article-button {
  gap: var(--dl-space-space-oneandhalfunits);
  cursor: pointer;
  display: flex;
  transition: 0.3s;
  align-items: center;
  border-color: #80FF44;
  flex-direction: column;
  padding-bottom: var(--dl-space-space-halfunit);
  justify-content: center;
  border-bottom-width: 1px;
}
.article-button:hover {
  opacity: 0.5;
}
.article-link {
  display: contents;
}
.article-text {
  color: #80FF44;
  font-style: normal;
  font-weight: 500;
  line-height: 24px;
  text-decoration: none;
}





@media(max-width: 1200px) {
  .article-button {
    border-color: var(--dl-color-loyalbeaglebranding-lb_primary-300);
  }
  .article-text {
    color: var(--dl-color-loyalbeaglebranding-lb_primary-300);
  }
}
@media(max-width: 991px) {
  .article-card {
    padding-top: var(--dl-space-space-twounits);
    padding-left: var(--dl-space-space-oneandhalfunits);
    padding-right: var(--dl-space-space-oneandhalfunits);
    padding-bottom: var(--dl-space-space-twounits);
  }
}
</style>
