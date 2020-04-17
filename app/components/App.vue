<template>
  <Page>
    <ActionBar title="Love Calculator" />
    <FlexboxLayout flexDirection="column">
      <Image
        src="https://i.ya-webdesign.com/images/facebook-reactions-png-4.png"
        class="text-center"
        height="200"
        marginTop="20"
      />
      <TextView editable="false" class="h2 text-center">
        <FormattedString>
          <Span text="Welcome to Doctor Love!" fontWeight="Bold" />
        </FormattedString>
      </TextView>
      <TextField :text="name" hint="Enter Your name" height="80" class="h3" />
      <TextField :text="crush" hint="Enter Your Crush name" height="80" class="h3" />
      <button
        backgroundColor="#f5365c"
        color="#fff"
        marginTop="40"
        height="60"
        borderRadius="10"
        class="h2"
        @tap="onButtonTap"
      >Calculate</button>
    </FlexboxLayout>
  </Page>
</template>

<script>
import Home from "./Home";
export default {
  data() {
    return {
      msg: "Hello Harshith!",
      name: "",
      crush: ""
    };
  },
  methods: {
    onButtonTap() {
      this.$navigateTo(Home);
    }
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

