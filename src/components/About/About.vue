<script setup>
const strong = 'text-blue-400 font-normal'
const p = 'text-blue-200 font-pp lg:text-lg text-xl'
const p2 = 'font-pp text-xl text-blue-50 font-bold'
const div1 =
  'flex flex-col lg:flex-row items-center lg:justify-between gap-14 md:gap-x-60 text-center lg:text-start'
const div2 = 'flex flex-col md:gap-12 gap-4 justify-center items-center lg:items-start'
const h1 = 'text-blue-200 font-ms font-bold text-2xl lg:w-[120%] md:w-[100%] leading-10'
const a =
  'bg-blue-950 w-[258px] h-[50px] rounded-xl flex items-center justify-center hover:bg-blue-800'
const square = 'rounded-3xl lg:w-[100%]'
</script>

<template>
  <section>
    <div id="about" :class="div1">
      <div :class="div2">
        <h1 :class="h1">How does it work?</h1>
        <p :class="p">
          Vivi Bot, just like Vivi and its Black Mage brothers, can be
          <strong :class="strong">cloned</strong> into similar or
          <strong :class="strong">identical applications</strong>.
        </p>
        <p :class="p">
          By cloning the repository, you gain access to
          <strong :class="strong">all of its features</strong>, having
          <strong :class="strong">your own Vivi Bot</strong> to
          <strong :class="strong">use and customize as much as you want to!</strong>
        </p>
        <p :class="p">It’s made to be easy, fast and <strong :class="strong">simple</strong>!</p>
        <a href="https://github.com/daviebatista/vivi-bot/tree/V2.3" target="_blank" :class="a">
          <p :class="p2">Check it out</p>
          <img src="../../assets/button-arrow.svg" alt="arrow-right" />
        </a>
      </div>
      <img src="../../assets/vivi-square.jpg" alt="vivi-square" :class="square" id="vivi-square" />
    </div>
  </section>
</template>

<style scoped lang="scss">
section {
  background: url('../../assets/about-2.jpg') no-repeat;
  background-size: cover;
  min-height: 120vh;
}

#about {
  padding: 100px 12.361111111111%;
}

h1 {
  font-size: 48px;
}

p {
  transition: 0.3s;
}

img {
  transition: 0.3s;
}

a {
  transition: 0.3s;

  &:hover {
    p {
      margin-left: 40px;
    }

    img {
      padding-left: 40px;
    }
  }
}

#vivi-square {
  filter: drop-shadow(0px 0px 21px #0c134f);
}

@media (max-width: 1366px) {
  #about {
    padding: 120px 85px;
  }
}

@media (max-width: 768px) {
  #about {
    padding: 50px 40px;
  }

  h1 {
    font-size: 28px;
    margin-top: 0px;
  }
}

@media (max-width: 610px) {
  #about {
    padding: 50px 40px;
  }
}
</style>
