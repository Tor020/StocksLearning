<template>
  <div>
    <TabCard :tabs="tabs" :initialTab="initialTab">
      <template slot="tab-head-james">
        James
      </template>
      <template slot="tab-panel-james">
        <h2 class="title">James Potter</h2>
        <p class="description">
          James Potter is a young wizard who fought against Voldemort in the
          1970s, only to be killed along with his wife Lily while trying to
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
        <h2 class="title">Lily Potter</h2>
        <p class="description">
          Lily J. Potter was a Muggle-born witch, the younger daughter of Mr and
          Mrs Evans, and the younger sister of Petunia Evans.
        </p>
        <p class="description">
          She sacrificed herself to save Harry and caused Voldemort to loose the
          <strong>First Wizarding War</strong>.
        </p>
      </template>
      <template slot="tab-head-snape">
        Snape
      </template>
      <template slot="tab-panel-snape">
        <h3 class="title">no description needed</h3>
        <img
          class="image"
          src="https://media1.tenor.com/images/b58f4b6f5cc71fb1d9663c66d0b42cb7/tenor.gif"
          alt=""
        />
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
      initialTab: 'james',
      tabs: ['james', 'Frank', 'snape']
    };
  }
};
</script>