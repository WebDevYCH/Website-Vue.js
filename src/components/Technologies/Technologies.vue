<template>
  <section class="technologies">
    <div class="technologies-content">
      <h2>#technologies</h2>
      <div class="technologies-grid">
        <Item v-for="technology of technologies" :key="technology.name" :technology="technology" />
      </div>
    </div>
  </section>
</template>
<script>
import Item from "./Item.vue";

import { useAge } from "../../hooks/useAge";

import reactLogo from "../../img/technologies/react.svg";
import gatsbyLogo from "../../img/technologies/gatsby.svg";
import nodejsLogo from "../../img/technologies/nodejs.svg";
import jsLogo from "../../img/technologies/js.svg";
import tsLogo from "../../img/technologies/ts.svg";
import vueLogo from "../../img/technologies/vue.svg";
import nextjsLogo from "../../img/technologies/nextjs.svg";
import elixirLogo from "../../img/technologies/elixir.png";
import swiftLogo from "../../img/technologies/swift.svg";

const technologies = [
  {
    name: "TypeScript",
    logo: tsLogo,
    bgColor: "#007acc",
    fgColor: "#ffffff",
    website: "https://www.typescriptlang.org",
  },
  {
    name: "JavaScript",
    logo: jsLogo,
    bgColor: "#f7df1e",
    fgColor: "#000000",
    website: "https://developer.mozilla.org/en-US/docs/Web",
  },
  {
    name: "React",
    logo: reactLogo,
    bgColor: "#53C1DE",
    fgColor: "#000000",
    website: "https://reactjs.org",
  },
  {
    name: "Gatsby",
    logo: gatsbyLogo,
    bgColor: "#663399",
    fgColor: "#ffffff",
    website: "https://gatsbyjs.org",
  },
  {
    name: "Swift",
    logo: swiftLogo,
    bgColor: "#f57929",
    fgColor: "#ffffff",
    website: "https://swift.org/",
  },
  {
    name: "Node.js",
    logo: nodejsLogo,
    bgColor: "#539E43",
    fgColor: "#ffffff",
    website: "https://nodejs.org",
  },
  {
    name: "Next.js",
    logo: nextjsLogo,
    bgColor: "#eeeeee",
    fgColor: "#000000",
    website: "https://nextjs.org",
  },
  {
    name: "Vue.js",
    logo: vueLogo,
    bgColor: "#42b883",
    fgColor: "#ffffff",
    website: "https://vuejs.org",
  },
  {
    name: "React Native",
    logo: reactLogo,
    bgColor: "#53C1DE",
    fgColor: "#000000",
    website: "https://reactnative.dev",
  },
  {
    name: "Elixir",
    logo: elixirLogo,
    bgColor: "#ffffff",
    fgColor: "#000000",
    website: "https://elixir-lang.org",
  },
];

export default {
  setup() {
    const age = useAge(2004);

    return { age, technologies };
  },
  components: {
    Item,
  },
};
</script>
<style lang="scss" scoped>
.technologies {
  &-content {
    max-width: 800px;
    margin: 0 auto;
    padding: 50px 25px;
    padding-bottom: 0;
  }

  &-grid {
    display: grid;
    grid-gap: 15px;
    overflow: auto;
    padding-bottom: 15px;

    grid-template-rows: auto auto;
    grid-template-columns: repeat(5, 200px);
  }
}
</style>
