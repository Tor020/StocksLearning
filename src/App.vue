<template>
  <section class="section">
    <div class="container">

      <div class="columns">

        <div class="column">
        <tabs>
            <tab name="About Us" :selected="true">
                <h1>Here is the content for the about us tab.</h1>
            </tab>

            <tab name="About Our Culture">
                <h1>Here is the content for the about our culture tab.</h1>
            </tab>

            <tab name="About Our Vision">
                <h1>Here is the content for the about our vision tab.</h1>
            </tab>
        </tabs>
        </div>
        


      </div>

    </div>
  </section>
</template>

<style lang="scss">
</style>

<script>
import Tabs from "./components/Tabs.vue";
import Tab from "./components/Tab.vue"

export default {
  components: {
    Tabs,
    Tab
  },
  data() {
    return {
      tabs: [],
      otherExample: true
    };
  },
  created(){
    this.tabs = this.$children
  },
  mounted(){
    console.log(this.$children)
  }
};
</script>