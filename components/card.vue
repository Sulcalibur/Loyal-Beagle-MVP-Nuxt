<template>
  <section class="card-card" v-bind:class="rootClassName">
    <div class="card-icon1">
      <svg viewBox="0 0 1024 1024" class="card-icon2">
        <path
          d="M768 682l86 86v42h-684v-42l86-86v-212q0-100 51-174t141-96v-30q0-26 18-45t46-19 46 19 18 45v30q90 22 141 96t51 174v212zM512 938q-36 0-61-24t-25-60h172q0 34-26 59t-60 25z"
        ></path>
      </svg>
    </div>
    <main class="card-content">
      <h1 class="card-header">{{ header }}</h1>
      <p class="card-description">{{ description }}</p>
    </main>
  </section>
</template>

<script>
export default {
  name: 'Card',
  props: {
    description: {
      type: String,
      default:
        'Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium',
    },
    rootClassName: String,
    header: {
      type: String,
      default: 'Sima Mosbacher',
    },
  },
}
</script>

<style scoped>
.card-card {
  gap: var(--dl-space-space-oneandhalfunits);
  flex: 1;
  display: flex;
  padding: var(--dl-space-space-threeunits);
  position: relative;
  align-items: flex-start;
  border-radius: 20px;
  flex-direction: column;
  justify-content: flex-start;
  background-color: var(--dl-color-loyalbeaglebranding-lb_primary-800);
}
.card-icon1 {
  display: flex;
  padding: var(--dl-space-space-unit);
  align-items: center;
  aspect-ratio: 1;
  border-radius: 50%;
  flex-direction: column;
  padding-bottom: 16px;
  justify-content: center;
  background-color: var(--dl-color-primary-500);
}
.card-icon2 {
  fill: var(--dl-color-gray-white);
  width: 24px;
  height: 24px;
}
.card-content {
  gap: var(--dl-space-space-halfunit);
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  justify-content: flex-start;
}
.card-header {
  color: rgb(255, 255, 255);
  font-size: 24px;
  font-style: normal;
  font-family: Poppins;
  font-weight: 600;
  line-height: 36px;
}
.card-description {
  color: #C2C6CC;
  font-family: Poppins;
  line-height: 28px;
}



@media(max-width: 1200px) {
  .card-icon1 {
    background-color: var(--dl-color-loyalbeaglebranding-lb_primary-500);
  }
  .card-icon2 {
    fill: var(--dl-color-gray-white);
  }
}
@media(max-width: 991px) {
  .cardroot-class-name {
    flex: 0 0 auto;
    width: 100%;
  }
  .cardroot-class-name1 {
    flex: 0 0 auto;
    width: 100%;
  }
  .cardroot-class-name2 {
    flex: 0 0 auto;
    width: 100%;
  }
}
</style>
