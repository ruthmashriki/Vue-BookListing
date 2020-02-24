<template>
  <div>  
    <H1> {{title}} </H1>
    <li>
        <ul v-for="book in books"> {{book.title}}</ul>
    </li>
  </div>
</template>

<script>
export default {
  name: 'BookList',
  data() {
      return {
        title: "All Books",
        books: [
    {title: 'Self-Reliance', author: 'Ralph Waldo Emerson'},
    {title: 'American Gods', author: 'Neil Gaiman'},
    {title: 'Amusing Ourselves to Death', author: 'Neil Postman'},
]
      }

  },
};
</script>

<style>
h1, h2 {
    font-weight: normal;
}
li
{list-style-type: none;
padding: 0;
}

ul{
    display: block;
    margin: 0 10px;
}

</style>
