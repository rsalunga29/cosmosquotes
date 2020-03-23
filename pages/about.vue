<template>
  <div class="container">
    <div class="flex flex-col md:w-2/4 px-4 md:px-0">
      <div class="card">
        <div class="py-6 px-4">
          <div class="mb-4">
            <p class="text-xl font-bold">What is this?</p>
            <p>
              This is a Cosmos quote generator, which randomly picks quotes from a pre-built JSON array.
              Cosmos is one of my favorite science shows, and Carl Sagan is one of the many scientists who influenced me to take a liking to
              Astronomy.

              <br /><br />

              All content rights belong to their respective owners. The quotes were scraped off using Python from
              <a href="https://www.goodreads.com/work/quotes/3237312-cosmos"
                target="_blank" rel="noopener noreferrer">Goodreads</a>.
            </p>
          </div>

          <div class="mb-4">
            <p class="text-xl font-bold">What is Cosmos?</p>
            <p>
              <a href="https://en.wikipedia.org/wiki/Cosmos_(Carl_Sagan_book)"
                target="_blank" rel="noopener noreferrer">Cosmos</a> is a popular science book published in 1980 by Carl Sagan.
              It has 13 chapters, corresponding to the 13 episodes of the <a href="https://en.wikipedia.org/wiki/Cosmos:_A_Personal_Voyage"
                target="_blank" rel="noopener noreferrer">Cosmos: A Personal Voyage</a> TV series. The book covers a broad range of topics,
                comprising Sagan's reflections on anthropological, cosmological, biological, historical, and astronomical matters from antiquity
                to contemporary times. Sagan explores 15 billion years of cosmic evolution and the development of science and civilization. 
                He traces the origins of knowledge and the scientific method, mixing science and philosophy, 
                and speculates about the future of science.
            </p>
          </div>

          <div>
            <p class="text-xl font-bold">Who is Carl Sagan?</p>
            <p>
              Carl Edward Sagan (1934-1996) was an American astronomer and science author. Sagan earned his bachelor's and a master's degree in Physics
              in 1955 and 1956, respectively, and a doctorate in astronomy and astrophysics in 1960. Sagan assembled the first physical messages sent 
              into space: the Pioneer plaque and the Voyager Golden Record, universal messages that could potentially be understood by any 
              extraterrestrial intelligence that might find them. He spent most of his career as a professor of astronomy at Cornell University, 
              where he directed the Laboratory for Planetary Studies. Sagan and his works received numerous awards and honors, including 
              the NASA Distinguished Public Service Medal, the National Academy of Sciences Public Welfare Medal, and many more. 
              Sagan died of pneumonia at the age of 62, on December 20, 1996.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style>
a {
  @apply underline;
}
</style>
