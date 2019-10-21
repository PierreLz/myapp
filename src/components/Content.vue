<template>
  <div class="content">
    <h1> {{ title }} </h1>
    <ContentTwo message="This is a component inside the CONTENT component"/>
  </div>
</template>

<script lang="ts">
import { Component, Prop, Vue } from 'vue-property-decorator';
import ContentTwo from './ContentTwo.vue';

@Component({
  components: {
    ContentTwo
  },
})
export default class Content extends Vue {
  @Prop(String) title: string;
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
