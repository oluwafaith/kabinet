<template>
  <div>
    <transition-group name="fade" tag="div">
      <div v-for="image in currentImg" :key="image.id">
        <!-- <img :src="currentImg" /> -->
        <div class="h-screen bg-gradient-to-b from-blue-900 to-blue-400 text-white">
            <div class="flex justify-between h-full px-32">
                <div class="self-end pb-32">
                    <h1 class="text-6xl font-semibold mb-6">{{ image.first }}</h1>
                    <h1 class="text-6xl font-semibold mb-6">{{ image.second }}</h1>
                    <p class="mb-12">{{ image.sub }}</p>
                    <p class="mb-12">{{ image.otherSub }}</p>
                    <p class="mb-6">{{ image.name }}</p>
                    <nuxt-link to="/signup">
                        <a class="inline-block text-sm text-center text-white py-2 px-16 bg-sky-500 leading-none border-solid border-2 border-sky-500 rounded hover:border-transparent hover:bg-sky-800 mt-4 lg:mt-0">Sign Up</a>
                    </nuxt-link>
                </div>
                <img class="self-end" src="/guy1.png" alt="">
            </div>
        </div>
      </div>
    </transition-group>
    <a class="prev" @click="prev" href="#">&#10094; Previous</a>
    <a class="next" @click="next" href="#">&#10095; Next</a>
  </div>
</template>
<script>
export default {
  name: "Slider",
  data() {
    return {
      images: [
        {
            id: 0,
            first: "Influence the change",
            second: "you want to see",
            sub: "“The most important political office is that of",
            otherSub: "the private citizen.”",
            name: "– Louis D. Brandeis"
        },
        {
            id: 1,
            first: "Harness the power of",
            second: "a youth nation",
            sub: "“Irrespective of any political party, Be a supporter of",
            otherSub: "good people who want to do something for the society.”",
            name: "– Kapil Dev"
        },
        {
            id: 2,
            first: "Support Civic participation & drive",
            second: "impactful change",
            sub: "“Action without thought is empty. Thought without action",
            otherSub: "is blind.”",
            name: "– Kwame Nkrumah"
        },
      ],
      timer: null,
      currentIndex: 0
    };
  },

  mounted: function() {
    this.startSlide();
  },

  methods: {
    startSlide: function() {
      this.timer = setInterval(this.next, 4000);
    },

    next: function() {
      this.images.id += 1;
    },
    prev: function() {
      this.images.id -= 1;
    }
  },

  computed: {
    currentImg: function() {
      return this.images[Math.abs(this.currentIndex) % this.images.length];
    }
  }
};
</script>

<style>
    .fade-enter-active,
.fade-leave-active {
  transition: all 0.9s ease;
  overflow: hidden;
  visibility: visible;
  position: absolute;
  width:100%;
  opacity: 1;
}

.fade-enter,
.fade-leave-to {
  visibility: hidden;
  width:100%;
  opacity: 0;
}

img {
  height:600px;
  width:100%
}

.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 40%;
  width: auto;
  padding: 16px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.7s ease;
  border-radius: 0 4px 4px 0;
  text-decoration: none;
  user-select: none;
}

.next {
  right: 0;
}

.prev {
  left: 0;
}

.prev:hover, .next:hover {
  background-color: rgba(0,0,0,0.9);
}
</style>