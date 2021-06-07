<template>
  <v-container>
    <ol>
      <li><nuxt-link to="/exercise1">Exercise 1</nuxt-link></li>
      <li><nuxt-link to="/exercise2">Exercise 2</nuxt-link></li>
    </ol>
    <br>
    Bonus
    <p>('b' + 'a' + + 'a' + 'a').toLowerCase() is "banana"</p>
    <p>
      For real I am not sure, the second 'a' (after the two plus signs) is assumed number why it returned 'Not a Number' aka 'NaN' which in lower case is nan<br>
      combined you got ba'nan'a.<br><br>It seems it is a shorthand for a number parsing.
    </p>
  </v-container>
</template>

<script>
export default {
}
</script>
