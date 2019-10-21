<template>
  <div class="content_two">
    <h2> {{ message }} </h2>
  </div>
</template>

<script lang="ts">

import { Component, Prop, Vue } from 'vue-property-decorator';
import Click from './Click.vue';

@Component

export default class ContentTwo extends Vue {
  @Prop(String) message: string;
}

</script>

<style scoped>
h1 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
