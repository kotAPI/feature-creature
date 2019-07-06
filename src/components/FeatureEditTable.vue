<template>
  <div>
    <table class="ui celled table">
      <thead>
        <tr>
          <th>&nbsp;</th>
          <th v-for="(feature,fX) in features" :key="fX">{{feature}}</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td data-label="Name">James</td>
          <td data-label="Age">24</td>
          <td data-label="Job">Engineer</td>
        </tr>
      </tbody>
    </table>

    <div class="ui action input">
      <input type="text" placeholder="Search..." v-model="newFeatureName" />
      <button class="ui labeled icon button" @click="addNewFeature">
        <i class="add icon"></i>
        Add Plan
      </button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      newFeatureName: "",
      features: [],
      plans: ["1"]
    };
  },
  methods: {
    addNewFeature() {
      this.features.push(this.newFeatureName);
    }
  }
};
</script>

<style>
</style>
