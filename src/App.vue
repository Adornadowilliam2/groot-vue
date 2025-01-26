<template>
  <div v-html="content"></div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      content: `
        <div>
          <nav class="flex items-center gap-2 p-2 bg-green-200">
            <img
              src="https://i.etsystatic.com/13693104/r/il/6f7817/1499379340/il_fullxfull.1499379340_9dk7.jpg"
              alt="Groot"
              class="w-20"
            />
            <h1>Groot</h1>
          </nav>
          <section id="grid">
            <div>
              <img src="https://th.bing.com/th/id/OIP.YtbFN_v7qC9fFv_Njx_fKQHaEK?rs=1&pid=ImgDetMain" alt="" class="w-[100%]" />
            </div>
            <div class="p-2 border-[2px] border-black rounded-lg" >
Groot (/ɡruːt/) is a character appearing in American comic books published by Marvel Comics. Created by Stan Lee, Larry Lieber and Jack Kirby, the character first appeared in Tales to Astonish #13 (November 1960). An extraterrestrial, sentient tree-like creature, the original Groot first appeared as an invader that intended to capture humans for experimentation. The character can only say the repeated line "I am Groot", but has different meanings depending on context. In the Marvel Cinematic Universe (MCU) franchise, Star-Lord, Thor, Rocket Raccoon, Gamora and Drax the Destroyer are able to understand him.
            </div>
          </section>

          <main class="flex p-2 gap-4 flex-wrap justify-center">
            <div class="card border-[2px] p-2">
              <img
                src="https://th.bing.com/th/id/OIP.P7HXnvB-lCh06L6KeOEtZwHaEK?rs=1&pid=ImgDetMain"
                alt="Teen Groot"
                class="w-[200px] h-[150px]"
              />
              <h3 class="font-bold">Teen Groot</h3>
            </div>
            <div class="card border-[2px] p-2">
              <img
                src="https://th.bing.com/th/id/OIP.CYSTnSclV9tY2hnxth28fgHaFf?rs=1&pid=ImgDetMain"
                alt="Baby Groot"
                class="w-[200px] h-[150px]"
              />
              <h3 class="font-bold">Baby Groot</h3>
            </div>
            <div class="card border-[2px] p-2">
              <img
                src="https://www.slashfilm.com/img/gallery/groot-isnt-nearly-as-old-as-he-looks-in-guardians-of-the-galaxy/l-intro-1688139459.jpg"
                alt="Adult Groot"
                class="w-[200px] h-[150px]"
              />
              <h3 class="font-bold">Adult Groot</h3>
            </div>
          </main>

          <section class="p-[20px] border-t-2 border-black">
            <h2 class="text-center text-3xl mb-2">Contact Us</h2>
            <form action="" class="border-[2px] rounded-lg p-2 block m-auto">
              <div>
                <label for="username" class="block">Username:</label>
                <input
                  type="text"
                  id="username"
                  class="border-[2px] rounded-lg p-2 w-[100%]"
                  placeholder="Enter your username"
                />
              </div>
              <div class="mt-2">
                <label for="message" class="block">Message:</label>
                <textarea
                  id="message"
                  cols="30"
                  rows="10"
                  class="border-[2px] rounded-lg p-2 w-[100%]"
                  placeholder="Enter your message"
                ></textarea>
              </div>
              <div class="mt-2">
                <button
                  class="bg-green-200 p-2 rounded-lg w-[100%] hover:cursor-pointer"
                >
                  Submit
                </button>
              </div>
            </form>
          </section>
        </div>
      `,
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

#grid{
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 10px;
  padding:20px;
}

@media (max-width: 767px){
  #grid{
    grid-template-columns: 1fr;
  }
}
</style>
