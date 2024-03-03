<template>
  <img src="../assets/dots.png" alt="" class="dots-1">
  <img src="../assets/dots.png" alt="" class="dots-2">
  <section class="hero">
    <div class="left-side">
      <div class="clip-text clip-text_one align-left">CONNECTING THE WORLD THROUGH WORDS</div>
      <p class="align-left">Professional trasnlation services that <em>really</em> capture the essense of each language.
      </p>
      <button class="button-62" role="button">
        <span class="button-icon"><img src="../assets/send.png" alt="Contact"></span>
        <span class="button-text">CONTACT ME</span>
      </button>


    </div>
    <div class="right-side">
      <img src="../assets/translator.png" alt="">
      <svg viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg" class="blob">

        <path fill="#24A148"
          d="M23.8,-37.8C34.1,-35.2,48.1,-35.5,58.5,-29.7C68.9,-23.9,75.8,-11.9,72.9,-1.7C69.9,8.5,57.1,17,50.9,30.2C44.7,43.3,45.1,61,37.7,71.6C30.3,82.3,15.2,85.7,-0.5,86.5C-16.1,87.3,-32.2,85.4,-46.6,78.9C-61,72.4,-73.8,61.2,-72.2,47.3C-70.6,33.3,-54.6,16.7,-54,0.4C-53.4,-16,-68.2,-31.9,-67.2,-41.5C-66.3,-51.1,-49.8,-54.3,-35.9,-54.9C-22.1,-55.4,-11.1,-53.4,-2.2,-49.6C6.7,-45.9,13.5,-40.4,23.8,-37.8Z"
          transform="translate(100 100)" filter="url(#blur)" />
      </svg>
    </div>
  </section>
</template>

<script>
export default {
  name: 'HeroSection',
};
</script>

<style>
.hero {
  height: calc(100% - 4em);
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 4em 0;
}

.dots-1 {
  position: absolute;
  top: 0;
  left: -10%;
  z-index: -1;
  filter: opacity(0.1);
}

.dots-2 {
  position: absolute;
  bottom: 0;
  right: 0;
  z-index: -1;
  filter: opacity(0.1);
  height: 30em;
  width: 30em;
}

.left-side {
  width: 50%;
  padding: 2em;
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}

.left-side p {
  font-size: 1.5em;
  font-weight: 500;
  margin-top: 1em;
  color: #696B71;

}

.right-side {
  width: 50%;
  position: relative;

}

.right-side img {
  width: 60%;
  height: auto;
}

.blob {
  position: absolute;
  top: 0;
  right: 0;
  width: 100%;
  height: 100%;
  z-index: -1;
  filter: opacity(0.4);
}

.align-left {
  text-align: left;
}

.clip-text {
  font-size: 6vw;
  font-weight: bold;
  line-height: 1;
  position: relative;
  display: inline-block;
  /* Color fallback */
  color: #fff;
  -webkit-background-clip: text;

  -webkit-text-fill-color: transparent;
  white-space: normal;

}

.clip-text_one {
  background-image: url(https://source.unsplash.com/random/?dark,night,city);
}

.button-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  background: #75b381;
  border-top-left-radius: 12px;
  border-bottom-left-radius: 12px;
}

.button-icon img {
  display: block;
  width: 2em;
  height: auto;
}

.button-text {
  background: #FFFFFF;
  /* White background */
  color: #75b381;
  /* Adjust text color to match the design */
  padding: 0.5em 1em;
  /* Adjust padding */
  border-top-right-radius: 12px;
  /* Match the button's border radius */
  border-bottom-right-radius: 12px;
  flex-grow: 1;
  /* Ensure the text part fills the remaining space */
}

.button-62 {
  width: auto;
  background: linear-gradient(to right, #75b381 0%, #75b381 30%, #f3f2f0 30%);
  box-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2);
  border: 0;
  border-radius: 12px;
  color: #FFFFFF;
  cursor: pointer;
  display: flex;
  align-items: center;
  font-family: -apple-system, system-ui, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  font-size: 16px;
  font-weight: 500;
  line-height: 2.5;
  outline: transparent;
  padding: 0;
  text-align: center;
  text-decoration: none;
  transition: box-shadow .2s ease-in-out;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
  white-space: nowrap;
}

.button-icon img {
  width: 2em;
  height: 2em;
  padding: 0 1em;
  color: #FFFFFF;
  filter: invert(100%);

}

.button-text {
  color: #75b381;
  flex: 1;
  background: #f3f2f0;
  margin: 0 1em;
}

.button-62:not([disabled]):focus {
  box-shadow: 0 0 .25rem rgba(0, 0, 0, 0.5), -.125rem -.125rem 1rem rgba(156, 206, 166, 0.5) 1rem rgba(117, 179, 129, 0.5);
}

.button-62:not([disabled]):hover {
  box-shadow: 0 0 .25rem rgba(0, 0, 0, 0.5), -.125rem -.125rem 1rem rgba(68, 187, 68, 0.5), .125rem .125rem 1rem rgba(51, 172, 51, 0.5);
}

@media (max-width: 768px) {

  /* Adjust the breakpoint as needed */
  .hero {
    flex-direction: column;
    justify-content: flex-start;
  }

  .left-side,
  .right-side {
    width: 100%;
    /* Make them take the full width on smaller screens */
  }

  .left-side p {
    font-size: 3vw;
  }

  .align-left {
    text-align: center;
  }

  .right-side img {
    width: 60%;
    /* Adjust the image size as needed */
    margin: 0 auto;
    /* Center the image */
  }

}

.right-side img {
  animation: floatAnimation 7s ease-in-out infinite;
}

.right-side .blob {
  animation: floatAnimation 6s ease-in-out infinite;
}


@keyframes floatAnimation {

  0%,
  100% {
    transform: translateY(0);
  }

  50% {
    transform: translateY(-15px);
  }
}
</style>
