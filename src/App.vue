<template>
  <div class='container'>
    <TabCard :tabs="tabs" :initialTab="initialTab">
      
      <!-- 1 -->
      <template slot="tab-head-ALSOFRANK">
        ALSOFRANK
      </template>
      <template slot="tab-panel-ALSOFRANK">
        <h2 class="title">ALSOFRANK </h2>
        
        <p class="description">
        <a href="https://babylonbee.com/">Funny haha meme christian satire</a>
        https://babylonbee.com/
          FRANK  is a young wizard who fought against DUM in the
          1970s, only to be killed along with his wife FRANKIE while trying to
          protect their 15-month-old son Harry.
        </p>
        <p class="description">
          He was a descendant of Ignotus Peverell and the only child of wealthy,
          elderly parents.
        </p>
      </template>

      <!-- 2 -->

      <template slot="tab-head-Frank">
        Frank
      </template>
      <template slot="tab-panel-Frank">
        <h2 class="title">FRANK</h2>
        <p class="description">
          Lily J. Potter was a Muggle-born witch, the younger daughter of Mr and
          Mrs Evans, and the younger sister of Petunia Evans.
        </p>
        <p class="description">
        DUMB
        </p>
      </template>


        <!-- 3 -->
      <template slot="tab-head-Links">
        Links

      </template>
      <template slot="tab-panel-Links">
        <p class="description">
          <a href="https://github.com/Tor020/StocksLearning">Github</a>
          <a href="https://app.netlify.com/sites/tender-goldwasser-3cbe93/overview">Netlify</a>
        </p>
      </template>

    </TabCard>
  </div>
</template>

<script>
import TabCard from './components/TabCard';

export default {
  name: 'App',
  components: {
    TabCard
  },
  data() {
    return {
      initialTab: 'ALSOFRANK',
      tabs: ['ALSOFRANK', 'Frank', 'Links']
    };
  }
};
</script>
