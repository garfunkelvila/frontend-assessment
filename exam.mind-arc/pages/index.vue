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
      For real I am not sure, the second 'a' (after the two plus signs) is assumed number thats why it returned 'Not a Number' aka 'NaN' which in lower case is nan
      combined you got ba'nan'a.
    </p>
    <p>
      It seems it is a shorthand for a number parsing because single quote in javascript assumes string and use concat for the enclosed parenthesis.
    </p>
    <p>
      I usually nest it with parenthesis to be more explicit.
    </p>
  </v-container>
</template>

<script>
export default {
}
</script>
<style scoped lang="scss">
p {
  max-width: 5in;
}
</style>
