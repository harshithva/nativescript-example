<template>
  <Page>
    <ActionBar title="Love Calculator" />
    <FlexboxLayout flexDirection="column">
      <button @tap="onButtonTap">Calculate again</button>
    </FlexboxLayout>
  </Page>
</template>

<script>
export default {
  methods: {
    onButtonTap() {
      this.$navigateBack();
    }
  }
};
</script>

<style scoped>
ActionBar {
  background-color: #f5365c;
  color: #ffffff;
}
</style>