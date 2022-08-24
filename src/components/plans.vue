<template>
  <v-container grid-list-lg>
    <v-row column>
      <v-col class="text-xs-center display-1 my-5">Pricing</v-col>
      <v-col class="text-xs-center display-1 font-weight-black"
        >Plans that scale with your user growth</v-col
      >
    </v-row>
    <v-row row wrap>
      <v-col>
        <v-card>
          <v-img :src="images.rocket1" height="300px">
            <v-container fluid>
              <v-row>
                <v-col flexbox>
                  <span class="subheading purple white--text px-1 py-1"
                    >DEVELOPER</span
                  >
                </v-col>
                <v-btn small>Try it</v-btn>
              </v-row>
            </v-container>
          </v-img>

          <v-card-title primary-title>
            <div>
              <h3 class="headline">Developer</h3>
              <ul>
                <li>Includes 1,000 sessions / mo</li>
                <li>14 day data retention</li>
              </ul>
            </div>
          </v-card-title>
        </v-card>
      </v-col>

      <v-col>
        <v-card>
          <v-img :src="images.rocket2" height="300px">
            <v-container fluid>
              <v-row fill-height>
                <v-col flexbox>
                  <span class="subheading purple white--text px-1 py-1"
                    >TEAM</span
                  >
                </v-col>
                <v-btn small>Try it</v-btn>
              </v-row>
            </v-container>
          </v-img>
          <v-card-title primary-title>
            <div>
              <h3 class="headline">Team</h3>
              <ul>
                <li>Starting at 10,000 sessions / mo</li>
                <li>Starting at 1 month retention</li>
              </ul>
            </div>
          </v-card-title>
        </v-card>
      </v-col>

      <v-col>
        <v-card>
          <v-img :src="images.rocket3" height="300px">
            <v-container fluid>
              <v-row fill-height>
                <v-col flexbox>
                  <span class="subheading purple white--text px-1 py-1"
                    >PROFESSIONAL</span
                  >
                </v-col>
                <v-btn small>Try it</v-btn>
              </v-row>
            </v-container>
          </v-img>
          <v-card-title primary-title>
            <div>
              <h3 class="headline">Professional</h3>
              <ul>
                <li>Any volume of Sessions</li>
                <li>Custom data retention</li>
                <li>On-premise available</li>
              </ul>
            </div>
          </v-card-title>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "RocketPlans",
  data() {
    return {
      images: {
        rocket1: require("../assets/rocket_1.jpg"),
        rocket2: require("../assets/rocket_2.jpg"),
        rocket3: require("../assets/rocket_3.jpg"),
      },
    };
  },
};
</script>
