<template>
  <nav class="navbar-navbar" v-bind:class="rootClassName">
    <a
      href="https://loyalbeagle.co.uk"
      target="_blank"
      rel="noreferrer noopener"
      class="navbar-link10"
    >
      <img
        alt="Loyal Beagle - Digital Loyalty Rewards"
        :src="brandingLogo"
        loading="eager"
        class="navbar-branding-logo"
      />
    </a>
    <div class="navbar-nav-content">
      <div class="navbar-nav-links1">
        <a href="#features" class="navbar-link11 nav-link">Features</a>
        <a href="#pricing" class="navbar-link12 nav-link">Prices</a>
        <a href="#faq" class="navbar-link13 nav-link">FAQ</a>
        <a href="https://app.loyalbeagle.co.uk/" class="navbar-link14 nav-link">
          Sign in
        </a>
      </div>
      <a href="https://app.loyalbeagle.co.uk/registration" class="navbar-link15">
        <div class="navbar-get-started1 get-started">
          <span class="navbar-text1">Start your Trial</span>
        </div>
      </a>
      <div id="open-mobile-menu" class="navbar-hamburger get-started">
        <img :alt="imageAlt" :src="imageSrc" class="navbar-image1" />
      </div>
    </div>
    <div id="mobile-menu" class="navbar-mobile-menu">
      <div class="navbar-branding">
        <img :alt="imageAlt1" :src="imageSrc1" class="navbar-image2" />
        <div id="close-mobile-menu" class="navbar-container1">
          <svg viewBox="0 0 1024 1024" class="navbar-icon1">
            <path
              d="M225.835 286.165l225.835 225.835-225.835 225.835c-16.683 16.683-16.683 43.691 0 60.331s43.691 16.683 60.331 0l225.835-225.835 225.835 225.835c16.683 16.683 43.691 16.683 60.331 0s16.683-43.691 0-60.331l-225.835-225.835 225.835-225.835c16.683-16.683 16.683-43.691 0-60.331s-43.691-16.683-60.331 0l-225.835 225.835-225.835-225.835c-16.683-16.683-43.691-16.683-60.331 0s-16.683 43.691 0 60.331z"
            ></path>
          </svg>
        </div>
      </div>
      <div class="navbar-nav-links2">
        <a
          href="https://www.loyalbeagle.co.uk/#features"
          class="navbar-link16 nav-link"
        >
          Features
        </a>
        <span class="nav-link navbar-link17">Why us</span>
        <a
          href="https://www.loyalbeagle.co.uk/#pricing"
          class="navbar-link18 nav-link"
        >
          Prices
        </a>
        <a
          href="mailto:help@support.loyalbeagle.co.uk?subject="
          class="navbar-link19 nav-link"
        >
          Contact
        </a>
      </div>
      <a
        href="https://app.loyalbeagle.co.uk/registration"
        target="_blank"
        rel="noreferrer noopener"
        class="navbar-link20"
      >
        <div class="navbar-get-started2 get-started">
          <span class="navbar-text2">Get started</span>
        </div>
      </a>
    </div>
    <div>
      <div class="navbar-container3">
        <DangerousHTML
          html="<script>
      /*
  Mobile menu - Code Embed
  */
  
  /* listenForUrlChangesMobileMenu() makes sure that if you changes pages inside your app, 
  the mobile menu will still work*/
  
  const listenForUrlChangesMobileMenu = () => {
      let url = location.href;
      document.body.addEventListener('click', () => {
          requestAnimationFrame(() => {
              if (url !== location.href) {
                  runMobileMenuCodeEmbed();
                  url = location.href;
              }
          });
      },
      true
      );
  };
  
  const runMobileMenuCodeEmbed = () => {
      // Mobile menu
      const mobileMenu = document.querySelector('#mobile-menu')
  
      // Buttons
      const closeButton = document.querySelector('#close-mobile-menu')
      const openButton = document.querySelector('#open-mobile-menu')
  
      // On openButton click, set the mobileMenu position left to -100vw
      openButton && openButton.addEventListener('click', function() {
          mobileMenu.style.transform = 'translateX(0%)'
      })
  
      // On closeButton click, set the mobileMenu position to 0vw
      closeButton && closeButton.addEventListener('click', function() {
          mobileMenu.style.transform = 'translateX(100%)'
      })
  }
  
  runMobileMenuCodeEmbed()
  listenForUrlChangesMobileMenu()
  </script>"
        ></DangerousHTML>
      </div>
    </div>
  </nav>
</template>

<script>
import DangerousHTML from 'dangerous-html/dist/vue/lib.js'

export default {
  name: 'Navbar',
  props: {
    imageAlt: {
      type: String,
      default: 'image',
    },
    imageSrc1: {
      type: String,
      default: '/Branding/planical7012-ttpb.svg',
    },
    imageSrc: {
      type: String,
      default: '/Icons/hamburger-200h.png',
    },
    imageAlt1: {
      type: String,
      default: 'image',
    },
    rootClassName: String,
    brandingLogo: {
      type: String,
      default: '/Branding/loyalbeagle_text.svg',
    },
  },
  components: {
    DangerousHTML,
  },
}
</script>

<style scoped>
.navbar-navbar {
  width: 100%;
  display: flex;
  z-index: 1000;
  position: relative;
  max-width: 1200px;
  align-self: auto;
  align-items: center;
  flex-shrink: 1;
  padding-top: var(--dl-space-space-threeunits);
  padding-right: 5px;
  padding-bottom: var(--dl-space-space-fiveunits);
}
.navbar-link10 {
  display: contents;
}
.navbar-branding-logo {
  top: 0px;
  left: -8px;
  width: 296px;
  bottom: 0px;
  height: 113px;
  position: absolute;
  align-self: flex-start;
  box-sizing: content-box;
  padding-top: var(--dl-space-space-oneandhalfunits);
  text-decoration: none;
}
.navbar-nav-content {
  gap: var(--dl-space-space-threeunits);
  display: flex;
  align-items: center;
  margin-left: auto;
  flex-direction: row;
  justify-content: flex-start;
}
.navbar-nav-links1 {
  gap: var(--dl-space-space-threeunits);
  display: flex;
  align-items: flex-start;
  border-color: transparent;
}
.navbar-link11 {
  color: var(--dl-color-gray-black);
  text-decoration: none;
}
.navbar-link12 {
  color: var(--dl-color-gray-black);
  text-decoration: none;
}
.navbar-link13 {
  color: var(--dl-color-gray-black);
  text-decoration: none;
}
.navbar-link14 {
  color: var(--dl-color-gray-black);
  text-decoration: none;
}
.navbar-link15 {
  display: contents;
}
.navbar-get-started1 {
  text-decoration: none;
  background-color: var(--dl-color-loyalbeaglebranding-lb_primary-500);
}
.navbar-text1 {
  color: rgba(255, 255, 255, 1);
  align-self: auto;
  font-style: Medium;
  text-align: left;
  font-family: Poppins;
  font-weight: 500;
  font-stretch: normal;
  text-decoration: none;
}
.navbar-hamburger {
  display: none;
}
.navbar-image1 {
  width: 100px;
  object-fit: cover;
}
.navbar-mobile-menu {
  gap: var(--dl-space-space-twounits);
  top: 0;
  left: 0;
  width: 100vw;
  height: 100vh;
  display: flex;
  padding: var(--dl-space-space-twounits);
  z-index: 100;
  position: fixed;
  transform: translateX(100%);
  transition: 0.3s;
  align-items: stretch;
  flex-direction: column;
  background-color: #fff;
}
.navbar-branding {
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
}
.navbar-image2 {
  width: 100px;
  filter: brightness(0) saturate(100%);
  object-fit: cover;
}
.navbar-container1 {
  display: flex;
  align-items: center;
  flex-direction: row;
  justify-content: space-between;
}
.navbar-icon1 {
  width: 24px;
  height: 24px;
}
.navbar-nav-links2 {
  gap: var(--dl-space-space-unit);
  color: var(--dl-color-gray-black);
  display: flex;
  flex-direction: column;
}
.navbar-link16 {
  text-decoration: none;
}
.navbar-link18 {
  text-decoration: none;
}
.navbar-link19 {
  text-decoration: none;
}
.navbar-link20 {
  display: contents;
}
.navbar-get-started2 {
  text-decoration: none;
}
.navbar-text2 {
  color: rgba(255, 255, 255, 1);
  align-self: auto;
  font-style: Medium;
  text-align: left;
  font-family: Poppins;
  font-weight: 500;
  font-stretch: normal;
  text-decoration: none;
}
.navbar-container3 {
  display: contents;
}

@media(max-width: 1200px) {
  .navbar-link14 {
    color: var(--dl-color-gray-black);
  }
  .navbar-get-started1 {
    background-color: var(--dl-color-loyalbeaglebranding-lb_primary-500);
  }
  .navbar-text1 {
    color: rgb(255, 255, 255);
    font-family: Poppins;
    font-weight: 500;
    text-decoration: none;
  }
}
@media(max-width: 767px) {
  .navbar-navbar {
    padding-bottom: var(--dl-space-space-fourunits);
  }
  .navbar-branding-logo {
    width: 260px;
  }
  .navbar-nav-links1 {
    display: none;
  }
  .navbar-get-started1 {
    display: none;
  }
  .navbar-hamburger {
    display: flex;
    padding-left: var(--dl-space-space-unit);
    padding-right: var(--dl-space-space-unit);
  }
  .navbar-image1 {
    width: 16px;
    height: 14px;
  }
  .navbar-branding {
    width: 100%;
  }
  .navbar-image2 {
    width: var(--dl-size-size-xlarge);
  }
  .navbar-nav-links2 {
    margin-top: var(--dl-space-space-twounits);
    align-items: flex-start;
    margin-bottom: var(--dl-space-space-twounits);
    justify-content: center;
  }
  .navbar-link17 {
    display: none;
  }
  .navbar-get-started2 {
    background-color: var(--dl-color-loyalbeaglebranding-lb_primary-500);
  }
  .navbar-text2 {
    color: var(--dl-color-gray-white);
  }
}
@media(max-width: 479px) {
  .navbar-branding-logo {
    top: 4px;
    left: 21px;
    width: 199px;
  }
  .navbar-nav-links1 {
    display: none;
  }
  .navbar-link16 {
    display: none;
  }
  .navbar-link18 {
    display: none;
  }
}
</style>
