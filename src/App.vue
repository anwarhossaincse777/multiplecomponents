<script setup>

import PostsComponents from "./components/PostsComponents.vue";
import ListComponent from "./components/ListComponent.vue";

const posts=[
  {
    title: "Deadbeef Decrementation",
    excerpt: "How to decrement from a magic debug value to zero.",
    tags: [
      {
        name: 'spirituality',
        slug: 'orcas',
        class: 'tag spirituality'
      },
      {

      }
      ],
  },
  {
    title: "Interior Crocodile Alligator, I Drive a Chevrolet Movie Theater",
    excerpt: "♫ Interior Crocodile Alligator, I Drive a Chevrolet Movie Theater ♫",
    tags: [{
      name: 'cats',
      slug: 'orcas',
      class: 'tag cats'
    }
    ,
      {

      }
    ]
  },
  {
    title: "Why My Practice of Thelema Makes Me Better at World of Warcraft",
    excerpt: "\"Do what thou wilt\" shall be the whole of the Law.",
    tags: [
      {
        name:'enchiladas',
        slug:'orcas',
        class:'tag enchiladas'
      },
      {

      }
      ],
  },
  {
    title:'Shrek Predicted the COVID-19 Pandemic',
    excerpt:'Find out how Shrek is disrupting astrology.',
    tags:[{
      name:'orcas',
      slug:'orcas',
      class:'tag orcas'
    },{
      name:'beer',
      slug:'beer',
      class:'tag beer'
    }]
  },
  {
    title:'Lorem Ipsum',
    excerpt:'You know what time it is: lorem ipsum time.',
    tags:[{

     name:'stoicism',
      slug: '',
      class: 'tag stoicism'
    },
      {

      }
    ]
  }
]
</script>

<template>
  <section class="mx-auto ">
    <header>
      <nav class="container mx-auto max-w-3xl px-8 pt-2 flex flex-wrap justify-between">
        <div>
          <h1>
            <a href="/11r/">11r</a>
          </h1>
          <p>america's favorite eleventy blog template</p>
        </div>

        <ul class="flex flex-wrap sm:w-32 w-full mt-6 md:justify-between justify-evenly">
          <li>
            <a href="/11r/404.html">404</a>
          </li>

          <li>
            <a href="/11r/about">About</a>
          </li>
        </ul>
      </nav>
    </header>
    <main class="container mx-auto max-w-3xl p-8 grow">

      <div>


      <PostsComponents :posts="posts"/>

      </div>

      <div>
        <div class="md:flex justify-evenly mb-6">
          <div class="flex justify-between mx-auto w-full">



            <div class="mx-auto mb-4">
              <a class="next-page md:mb-2" href="/11r/page/2/">Previous Page</a>
            </div>

          </div>

          <div class="flex justify-between mx-auto w-full">



            <div class="mx-auto">
              <a class="last-page" href="/11r/page/2/">Last Page</a>
            </div>

          </div>
        </div>

        <p class="text-center text-sm italic mb-10">(On page
          1
          of
          2.)</p>
      </div>

    <ListComponent :lists=posts />

    </main>
  </section>
</template>

<style scoped>

</style>
