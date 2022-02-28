<template>
  <v-card width="500px">
    <div class="base">
      <div class="sceen"></div>
      <div class="keypad">
        <v-card
          :printOut="0"
          class="mx-auto my-6"
          max-width="400"
          color="grey lighten-1"
          height="70px"
          width="600px"
          >{{ printOut }}</v-card
        >
        <v-row no-gutters>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn v-on:click="clear" class="AC" elevation="2">AC</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="plusMinus" elevation="2">-/+</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="percentage" elevation="2">%</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="division" elevation="2">÷</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
        </v-row>
        <v-row no-gutters>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="seven" elevation="2">7</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="eight" elevation="2">8</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="nine" elevation="2">9</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="multiplication" elevation="2">x</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
        </v-row>
        <v-row no-gutters>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="four" elevation="2">4</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="five" elevation="2">5</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="five" elevation="2">6</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="subtraction" elevation="2">-</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
        </v-row>
        <v-row no-gutters>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="one" elevation="2">1</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="two" elevation="2">2</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="three" elevation="2">3</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="addition" elevation="2">+</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
        </v-row>
        <v-row no-gutters>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="zero" width="160" elevation="2">0</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="decimal" elevation="2">.</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
          <v-col>
            <v-list-item>
              <v-list-item-content>
                <v-btn class="equal" elevation="2">=</v-btn>
              </v-list-item-content>
            </v-list-item>
          </v-col>
        </v-row>
      </div>
    </div>
  </v-card>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "HelloWorld",

  data: () => ({
    printOut: 0,
    ecosystem: [
      {
        text: "vuetify-loader",
        href: "https://github.com/vuetifyjs/vuetify-loader",
      },
      {
        text: "github",
        href: "https://github.com/vuetifyjs/vuetify",
      },
      {
        text: "awesome-vuetify",
        href: "https://github.com/vuetifyjs/awesome-vuetify",
      },
    ],
    importantLinks: [
      {
        text: "Documentation",
        href: "https://vuetifyjs.com",
      },
      {
        text: "Chat",
        href: "https://community.vuetifyjs.com",
      },
      {
        text: "Made with Vuetify",
        href: "https://madewithvuejs.com/vuetify",
      },
      {
        text: "Twitter",
        href: "https://twitter.com/vuetifyjs",
      },
      {
        text: "Articles",
        href: "https://medium.com/vuetify",
      },
    ],
    whatsNext: [
      {
        text: "Explore components",
        href: "https://vuetifyjs.com/components/api-explorer",
      },
      {
        text: "Select a layout",
        href: "https://vuetifyjs.com/getting-started/pre-made-layouts",
      },
      {
        text: "Frequently Asked Questions",
        href: "https://vuetifyjs.com/getting-started/frequently-asked-questions",
      },
    ],
  }),
});
</script>
