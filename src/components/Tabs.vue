<template>
<div>
    <div class="tabs">
      <ul>
        <li v-for="tab in tabs">{{tab.name}}</li>
      </ul>
    </div>

    <div class="tabs-details">
      <slot></slot>
    </div>
</div>

</template>

<script>
export default  {
  components:{

  },
  data() {
        return { tabs: [] };
    },

    created() {
        this.tabs = this.$children;
    },

    methods: {
        selectTab(selectedTab) {
            this.tabs.forEach(tab => {
                tab.isActive = (tab.href == selectedTab.href);
            });
        }
    }
}

</script>