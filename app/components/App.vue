<template>
  <Page>
    <ActionBar title="Love Calculator" />
    <FlexboxLayout flexDirection="column">
      <TextView editable="false" class="h2 text-center">
        <FormattedString>
          <Span text="Welcome to Doctor Love!" fontWeight="Bold" />
        </FormattedString>
      </TextView>
      <TextField :text="textFieldValue" hint="Enter Your name" height="80" class="h3" />
      <TextField :text="textFieldValue" hint="Enter Your Crush name" height="80" class="h3" />
      <button
        backgroundColor="#f5365c"
        color="#fff"
        marginTop="40"
        height="60"
        borderRadius="10"
        class="h2"
      >Calculate</button>
    </FlexboxLayout>
  </Page>
</template>

<script >
export default {
  data() {
    return {
      msg: "Hello Harshith!"
    };
  }
};
</script>

<style scoped>
ActionBar {
  background-color: #f5365c;
  color: #ffffff;
}

.message {
  vertical-align: center;
  text-align: center;
  font-size: 20;
  color: #333333;
}
</style>
