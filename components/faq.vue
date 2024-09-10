<template>
  <div class="faq-accordion" v-bind:class="rootClassName">
    <div data-role="accordion-container" class="faq-element1 accordion-element">
      <div class="faq-details1">
        <span class="faq-text10">
          Do you take any credit card details for the trial?
          <span v-html="rawia9f"></span>
        </span>
        <span data-role="accordion-content" class="faq-text11">
          No. You only add your payment details once you finish your trial.
        </span>
      </div>
      <div data-role="accordion-icon">
        <svg viewBox="0 0 1024 1024" class="faq-icon10">
          <path d="M366 708l196-196-196-196 60-60 256 256-256 256z"></path>
        </svg>
      </div>
    </div>
    <div data-role="accordion-container" class="faq-element2 accordion-element">
      <div class="faq-details2">
        <span class="faq-text12">
          Is my customers data safe and will it be used for other marketing or
          sold on?
        </span>
        <span data-role="accordion-content" class="faq-text13">
          Your customers data will remain on the Loyal Beagle system accessible
          for you to use, they agree upon their data being used for your marketing
          purposes not ours so it will not be used for any other purposes beside
          your own. You will be liable to maintain best practises when
          outreaching.
        </span>
      </div>
      <div data-role="accordion-icon">
        <svg viewBox="0 0 1024 1024" class="faq-icon12">
          <path d="M366 708l196-196-196-196 60-60 256 256-256 256z"></path>
        </svg>
      </div>
    </div>
    <div data-role="accordion-container" class="faq-element3 accordion-element">
      <div class="faq-details3">
        <span class="faq-text14">Is this an app for my business?</span>
        <span data-role="accordion-content" class="faq-text15">
          This is an online portal designed to help you engage with your
          customers,  reward them for being loyal and keep them coming back, the
          system can be used on your phone or tablet and your customers can access
          this on their apple or android phones.
        </span>
      </div>
      <div data-role="accordion-icon">
        <svg viewBox="0 0 1024 1024" class="faq-icon14">
          <path d="M366 708l196-196-196-196 60-60 256 256-256 256z"></path>
        </svg>
      </div>
    </div>
    <div data-role="accordion-container" class="faq-element4 accordion-element">
      <div class="faq-details4">
        <span class="faq-text16">
          How do the customers download the Loyalty Card?
        </span>
        <span data-role="accordion-content" class="faq-text17">
          This can be downloaded through a link shared on social media, email or
          direct message alternatively you can have a QR code in-store customers
          can scan and download in seconds.
        </span>
      </div>
      <div data-role="accordion-icon">
        <svg viewBox="0 0 1024 1024" class="faq-icon16">
          <path d="M366 708l196-196-196-196 60-60 256 256-256 256z"></path>
        </svg>
      </div>
    </div>
    <div data-role="accordion-container" class="faq-element5 accordion-element">
      <div class="faq-details5">
        <span class="faq-text18">
          Should we get rid of our physical loyalty cards now?
        </span>
        <span data-role="accordion-content" class="faq-text19">
          Keep your current cards! Some customers will like the physical ones or
          want to cash these in for rewards, however you can encourage them to use
          your new QR code to download the digital loyalty card.
        </span>
      </div>
      <div data-role="accordion-icon">
        <svg viewBox="0 0 1024 1024" class="faq-icon18">
          <path d="M366 708l196-196-196-196 60-60 256 256-256 256z"></path>
        </svg>
      </div>
    </div>
    <div data-role="accordion-container" class="faq-element6 accordion-element">
      <div class="faq-details6">
        <span class="faq-text20">
          Can we transfer points from physical cards over to the digital ones?
        </span>
        <span data-role="accordion-content" class="faq-text21">
          Yes! Once you scan your customers card you can choose how many stamps
          they receive, they can stack up rewards overtime as well. 
        </span>
      </div>
      <div data-role="accordion-icon">
        <svg viewBox="0 0 1024 1024" class="faq-icon20">
          <path d="M366 708l196-196-196-196 60-60 256 256-256 256z"></path>
        </svg>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FAQ',
  props: {
    rootClassName: String,
  },
  data() {
    return {
      rawia9f: ' ',
    }
  },
}
</script>

<style scoped>
.faq-accordion {
  width: 100%;
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: column;
  justify-content: center;
}
.faq-element1 {
  width: 100%;
  max-width: 800px;
  padding-top: var(--dl-space-space-threeunits);
  padding-bottom: var(--dl-space-space-threeunits);
}
.faq-details1 {
  gap: var(--dl-space-space-oneandhalfunits);
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  justify-content: center;
}
.faq-text10 {
  color: rgb(0, 0, 0);
  width: 100%;
  font-size: 20px;
  font-style: normal;
  font-family: Poppins;
  font-weight: 500;
  line-height: 28px;
}
.faq-text11 {
  color: rgb(0, 0, 0);
  width: 100%;
  font-family: Poppins;
  line-height: 24px;
  user-select: text;
}
.faq-icon10 {
  fill: var(--dl-color-gray-white);
  width: var(--dl-size-size-xsmall);
  height: var(--dl-size-size-xsmall);
}
.faq-element2 {
  width: 100%;
  max-width: 800px;
  padding-top: var(--dl-space-space-threeunits);
  padding-bottom: var(--dl-space-space-threeunits);
}
.faq-details2 {
  gap: var(--dl-space-space-oneandhalfunits);
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  justify-content: center;
}
.faq-text12 {
  color: rgb(0, 0, 0);
  width: 100%;
  font-size: 20px;
  font-style: normal;
  font-family: Poppins;
  font-weight: 500;
  line-height: 28px;
}
.faq-text13 {
  color: rgb(0, 0, 0);
  width: 100%;
  font-family: Poppins;
  line-height: 28px;
  user-select: text;
}
.faq-icon12 {
  fill: var(--dl-color-gray-white);
  width: var(--dl-size-size-xsmall);
  height: var(--dl-size-size-xsmall);
}
.faq-element3 {
  width: 100%;
  max-width: 800px;
  padding-top: var(--dl-space-space-threeunits);
  padding-bottom: var(--dl-space-space-threeunits);
}
.faq-details3 {
  gap: var(--dl-space-space-oneandhalfunits);
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  justify-content: center;
}
.faq-text14 {
  color: rgb(0, 0, 0);
  width: 100%;
  font-size: 20px;
  font-style: normal;
  font-family: Poppins;
  font-weight: 500;
  line-height: 28px;
}
.faq-text15 {
  color: #000000;
  width: 100%;
  font-family: Poppins;
  line-height: 28px;
  user-select: text;
}
.faq-icon14 {
  fill: var(--dl-color-gray-white);
  width: var(--dl-size-size-xsmall);
  height: var(--dl-size-size-xsmall);
}
.faq-element4 {
  width: 100%;
  max-width: 800px;
  padding-top: var(--dl-space-space-threeunits);
  padding-bottom: var(--dl-space-space-threeunits);
}
.faq-details4 {
  gap: var(--dl-space-space-oneandhalfunits);
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  justify-content: center;
}
.faq-text16 {
  color: rgb(0, 0, 0);
  width: 100%;
  font-size: 20px;
  font-style: normal;
  font-family: Poppins;
  font-weight: 500;
  line-height: 28px;
}
.faq-text17 {
  color: #000000;
  width: 100%;
  font-family: Poppins;
  line-height: 28px;
  user-select: text;
}
.faq-icon16 {
  fill: var(--dl-color-gray-white);
  width: var(--dl-size-size-xsmall);
  height: var(--dl-size-size-xsmall);
}
.faq-element5 {
  width: 100%;
  max-width: 800px;
  padding-top: var(--dl-space-space-threeunits);
  padding-bottom: var(--dl-space-space-threeunits);
}
.faq-details5 {
  gap: var(--dl-space-space-oneandhalfunits);
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  justify-content: center;
}
.faq-text18 {
  color: rgb(0, 0, 0);
  width: 100%;
  font-size: 20px;
  font-style: normal;
  font-family: Poppins;
  font-weight: 500;
  line-height: 28px;
}
.faq-text19 {
  color: #000000;
  width: 100%;
  font-family: Poppins;
  line-height: 28px;
  user-select: text;
}
.faq-icon18 {
  fill: var(--dl-color-gray-white);
  width: var(--dl-size-size-xsmall);
  height: var(--dl-size-size-xsmall);
}
.faq-element6 {
  width: 100%;
  max-width: 800px;
  padding-top: var(--dl-space-space-threeunits);
  padding-bottom: var(--dl-space-space-threeunits);
}
.faq-details6 {
  gap: var(--dl-space-space-oneandhalfunits);
  width: 100%;
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  justify-content: center;
}
.faq-text20 {
  color: rgb(0, 0, 0);
  width: 100%;
  font-size: 20px;
  font-style: normal;
  font-family: Poppins;
  font-weight: 500;
  line-height: 28px;
}
.faq-text21 {
  color: #000000;
  width: 100%;
  font-family: Poppins;
  line-height: 28px;
  user-select: text;
}
.faq-icon20 {
  fill: var(--dl-color-gray-white);
  width: var(--dl-size-size-xsmall);
  height: var(--dl-size-size-xsmall);
}

@media(max-width: 1200px) {
  .faq-text13 {
    color: rgb(0, 0, 0);
    font-family: Poppins;
    line-height: 28px;
  }
  .faq-text15 {
    color: rgb(0, 0, 0);
    font-family: Poppins;
    line-height: 28px;
  }
  .faq-text17 {
    color: rgb(0, 0, 0);
    font-family: Poppins;
    line-height: 28px;
  }
  .faq-text19 {
    color: rgb(0, 0, 0);
    font-family: Poppins;
    line-height: 28px;
  }
  .faq-text21 {
    color: rgb(0, 0, 0);
    font-family: Poppins;
    line-height: 28px;
  }
}
@media(max-width: 767px) {
  .faq-text10 {
    font-size: 16px;
    line-height: 24px;
  }
  .faq-text12 {
    font-size: 16px;
    line-height: 24px;
  }
  .faq-text14 {
    font-size: 16px;
    line-height: 24px;
  }
  .faq-text16 {
    font-size: 16px;
    line-height: 24px;
  }
  .faq-text18 {
    font-size: 16px;
    line-height: 24px;
  }
  .faq-text20 {
    font-size: 16px;
    line-height: 24px;
  }
}
</style>
