<template>
  <layout>
    <ul>
      <li v-for="{ node } in $page.posts.edges" :key="node.id">
        <g-link :to="node.slug">
          <div class=" border-solid border-2 border-primary max-auto-sm overflow-hidden shadow-lg p-20 m-4 rounded-md">
            <h1 class="text-2xl text-primary font-bold">  {{node.title}}  </h1>
            <p class="pt-5 text-darkgray"> {{node.description}} </p>
            <p class="font-normal text-sm pt-5 text-primary"> Posted on {{node.date}} </p>
          </div>
        </g-link>
      </li>

    </ul>
  </layout>
</template>

<page-query>
query Posts{
  posts:allContentfulBlogPost{
    edges{
      node{
      id,
      title,
slug,

      description,
date (format: "MMMM DD, YYYY"),




      }
    }
 }
}
</page-query>