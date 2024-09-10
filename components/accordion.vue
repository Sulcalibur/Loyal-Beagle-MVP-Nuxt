<template>
  <div class="accordion-accordion" v-bind:class="rootClassName">
    <div
      data-role="accordion-container"
      class="accordion-element1 accordion-element"
    >
      <div class="accordion-details1">
        <span class="accordion-text1">{{ text }}</span>
        <span data-role="accordion-content" class="accordion-text2">
          {{ text1 }}
        </span>
      </div>
      <svg
        viewBox="0 0 1024 1024"
        data-role="accordion-icon"
        class="accordion-icon1"
      >
        <path d="M366 708l196-196-196-196 60-60 256 256-256 256z"></path>
      </svg>
    </div>
    <div
      data-role="accordion-container"
      class="accordion-element2 accordion-element"
    >
      <div class="accordion-details2">
        <span class="accordion-text3">{{ text2 }}</span>
        <span data-role="accordion-content" class="accordion-text4">
          {{ text3 }}
        </span>
      </div>
      <svg
        viewBox="0 0 1024 1024"
        data-role="accordion-icon"
        class="accordion-icon3"
      >
        <path d="M366 708l196-196-196-196 60-60 256 256-256 256z"></path>
      </svg>
    </div>
    <div
      data-role="accordion-container"
      class="accordion-element3 accordion-element"
    >
      <div class="accordion-details3">
        <span class="accordion-text5">{{ text4 }}</span>
        <span data-role="accordion-content" class="accordion-text6">
          {{ text5 }}
        </span>
      </div>
      <svg
        viewBox="0 0 1024 1024"
        data-role="accordion-icon"
        class="accordion-icon5"
      >
        <path d="M366 708l196-196-196-196 60-60 256 256-256 256z"></path>
      </svg>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Accordion',
  props: {
    text2: {
      type: String,
      default: 'Nemo enim ipsam voluptatem quia voluptas',
    },
    text1: {
      type: String,
      default:
        'Sed do eiusmod tempor incididunt ut labore et dolore magna aliquat enim ad minim veniam, quis nostrud',
    },
    text: {
      type: String,
      default: 'Aliquam quaerat voluptatem',
    },
    text4: {
      type: String,
      default: 'Magnam aliquam quaerat voluptatem',
    },
    text5: {
      type: String,
      default:
        'Sed do eiusmod tempor incididunt ut labore et dolore magna aliquat enim ad minim veniam, quis nostrud',
    },
    text3: {
      type: String,
      default:
        'Sed do eiusmod tempor incididunt ut labore et dolore magna aliquat enim ad minim veniam, quis nostrud',
    },
    rootClassName: String,
  },
}
</script>

<style scoped>
.accordion-accordion {
  display: flex;
  position: relative;
  align-items: flex-start;
  flex-direction: column;
  justify-content: center;
}
.accordion-element1 {
  width: 640px;
  user-select: none;
}
.accordion-details1 {
  gap: var(--dl-space-space-halfunit);
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  justify-content: center;
}
.accordion-text1 {
  color: #000000;
  width: 100%;
  font-size: 18px;
  max-width: 535px;
  font-style: normal;
  font-family: Poppins;
  font-weight: 600;
  line-height: 27px;
}
.accordion-text2 {
  color: #000000;
  width: 100%;
  max-width: 535px;
  font-family: Poppins;
  line-height: 24px;
  user-select: text;
}
.accordion-icon1 {
  fill: var(--dl-color-gray-white);
  width: var(--dl-size-size-xsmall);
  height: var(--dl-size-size-xsmall);
}
.accordion-element2 {
  width: 640px;
  user-select: none;
}
.accordion-details2 {
  gap: var(--dl-space-space-halfunit);
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  justify-content: center;
}
.accordion-text3 {
  color: #000000;
  width: 100%;
  font-size: 18px;
  max-width: 535px;
  font-style: normal;
  font-family: Poppins;
  font-weight: 600;
  line-height: 27px;
}
.accordion-text4 {
  color: #000000;
  width: 100%;
  max-width: 535px;
  font-family: Poppins;
  line-height: 24px;
  user-select: text;
}
.accordion-icon3 {
  fill: var(--dl-color-gray-white);
  width: var(--dl-size-size-xsmall);
  height: var(--dl-size-size-xsmall);
}
.accordion-element3 {
  width: 640px;
  user-select: none;
}
.accordion-details3 {
  gap: var(--dl-space-space-halfunit);
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  justify-content: center;
}
.accordion-text5 {
  color: #000000;
  width: 100%;
  font-size: 18px;
  max-width: 535px;
  font-style: normal;
  font-family: Poppins;
  font-weight: 600;
  line-height: 27px;
}
.accordion-text6 {
  color: #000000;
  width: 100%;
  max-width: 535px;
  font-family: Poppins;
  line-height: 24px;
  user-select: text;
}
.accordion-icon5 {
  fill: var(--dl-color-gray-white);
  width: var(--dl-size-size-xsmall);
  height: var(--dl-size-size-xsmall);
}

@media(max-width: 767px) {
  .accordion-element1 {
    width: 100%;
    max-width: 560px;
  }
  .accordion-text1 {
    font-size: 16px;
    line-height: 24px;
  }
  .accordion-element2 {
    width: 100%;
    max-width: 560px;
  }
  .accordion-text3 {
    font-size: 16px;
  }
  .accordion-element3 {
    width: 100%;
    max-width: 560px;
  }
  .accordion-text5 {
    font-size: 16px;
  }
}
@media(max-width: 479px) {
  .accordion-element1 {
    width: 350px;
    max-width: auto;
  }
  .accordion-element2 {
    width: 350px;
    max-width: auto;
  }
  .accordion-element3 {
    width: 350px;
    max-width: auto;
  }
}
</style>
