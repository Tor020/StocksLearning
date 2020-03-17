<template>
  <div class='container'>
    <TabCard :tabs="tabs" :initialTab="initialTab">
      <template slot="tab-head-ALSOFRANK">
        ALSOFRANK
      </template>
      <template slot="tab-panel-ALSOFRANK">
        <h2 class="title">ALSOFRANK </h2>
        <p class="description">
          FRANK  is a young wizard who fought against DUM in the
          1970s, only to be killed along with his wife FRANKIE while trying to
          protect their 15-month-old son Harry.
        </p>
        <p class="description">
          He was a descendant of Ignotus Peverell and the only child of wealthy,
          elderly parents.
        </p>
      </template>
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

      <template slot="tab-head-snape">
        Dumb Harry Potter Shit

      </template>
      <template slot="tab-panel-snape">
        <p class="description">
Dumb Harry Potter Shit
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
      tabs: ['ALSOFRANK', 'Frank', 'snape']
    };
  }
};
</script>