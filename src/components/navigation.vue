<template>
  <span>
    <v-navigation-drawer app v-model="drawer">
      <v-list>
        <template v-for="(menu, i) in menus">
          <v-list-item :key="i">
            <v-list-item-content>
              {{ menu.value }}
            </v-list-item-content>
          </v-list-item>
          <v-divider :key="`divider-${i}`"></v-divider>
        </template>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar app dark>
      <v-app-bar-nav-icon
        class="hidden-md-and-up"
        @click="drawer = !drawer"
      ></v-app-bar-nav-icon>
      <v-spacer class="hidden-md-and-up"></v-spacer>
      <v-img
        src="https://assets.logrocket.io/img/logo.png"
        max-width="120px"
        max-height="25px"
      ></v-img>
      <v-btn flat class="hidden-sm-and-down">Pricing</v-btn>
      <v-spacer class="hidden-sm-and-down"></v-spacer>
      <v-btn flat class="hidden-sm-and-down">Customers</v-btn>
      <v-btn flat class="hidden-sm-and-down">Docs</v-btn>
      <v-btn flat class="hidden-sm-and-down">Blog</v-btn>
      <v-btn flat class="hidden-sm-and-down">Login</v-btn>
      <v-btn color="purple darken-3" class="hidden-sm-and-down">Sign Up</v-btn>
    </v-app-bar>
  </span>
</template>

<script>
export default {
  name: "RocketNavigation",
  data() {
    return {
      drawer: false,
      menus: [
        { value: "Pricing" },
        { value: "Customers" },
        { value: "Docs" },
        { value: "Blog" },
        { value: "Login" },
        { value: "Sign Up" },
      ],
    };
  },
};
</script>

<style scoped></style>
<template>
  <v-container>
    <v-navigation-drawer app v-model="drawer">
      <v-list>
        <template v-for="(menu, i) in menus">
          <v-list-item :key="i">
            <v-list-item-content>
              {{ menu.value }}
            </v-list-item-content>
          </v-list-item>
          <v-divider :key="`divider-${i}`"></v-divider>
        </template>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar app dark>
      <v-app-bar-nav-icon
        class="hidden-md-and-up"
        @click="drawer = !drawer"
      ></v-app-bar-nav-icon>
      <v-spacer class="hidden-md-and-up"></v-spacer>
      <v-img
        src="https://assets.logrocket.io/img/logo.png"
        max-width="120px"
        max-height="25px"
      ></v-img>
      <v-btn flat class="hidden-sm-and-down">Pricing</v-btn>
      <v-spacer class="hidden-sm-and-down"></v-spacer>
      <v-btn flat class="hidden-sm-and-down">Customers</v-btn>
      <v-btn flat class="hidden-sm-and-down">Docs</v-btn>
      <v-btn flat class="hidden-sm-and-down">Blog</v-btn>
      <v-btn flat class="hidden-sm-and-down">Login</v-btn>
      <v-btn color="purple darken-3" class="hidden-sm-and-down">Sign Up</v-btn>
    </v-app-bar>
  </v-container>
</template>

<script>
export default {
  name: "RocketNavigation",
  data() {
    return {
      drawer: false,
      menus: [
        { value: "Pricing" },
        { value: "Customers" },
        { value: "Docs" },
        { value: "Blog" },
        { value: "Login" },
        { value: "Sign Up" },
      ],
    };
  },
};
</script>
