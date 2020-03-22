<template>
  <div class="container">
    <div class="flex flex-col md:w-2/4 px-4 md:px-0">
      <div class="card card--quote">
        <div class="px-6 py-4">
          <blockquote>{{ this.quoteText }}</blockquote>
        </div>

        <p class="self-end mr-4">- Carl Sagan, Cosmos</p>
      </div>

      <div class="md:inline-flex block md:self-end">
        <a type="button" class="button button--tweet md:mr-4 mb-4 md:mb-0 hover:bg-blue-500 w-full md:w-auto text-center"
          :href="this.shareLink" target="_blank"
          rel="noopener noreferrer">
          Share on Twitter
        </a>

        <button class="button button--generate hover:bg-green-700 w-full md:w-auto" @click="this.pickQuote">
          New Quote
        </button>
      </div>
    </div>
  </div>
</template>

<script>
import quotes from '~/static/quotes.json'

export default {
  created () {
    this.pickQuote()
  },

  data () {
    return {
      quotes: quotes,
      quoteText: '',
    }
  },

  computed: {
    shareLink: function() {
      return `https://twitter.com/intent/tweet?text=${this.quoteText} - Carl Sagan, Cosmos %23cosmos%0D%0A%0D%0Ahttps://bit.ly/cosmosq by @akiocodes`
    },
  },

  methods: {
    pickQuote () {
      let randomizer = Math.floor(Math.random() * this.quotes.length)

      this.quoteText = this.quotes[randomizer].text
    }
  }
}
</script>

<style>
.button {
  @apply block text-white font-bold py-2 px-4 rounded;
}

.button--tweet {
  @apply bg-blue-400;
}

.button--generate {
  @apply bg-green-500;
}

@media only screen and (max-width: 768px) {
  .card {
    height: 35rem;
  }
}
</style>
