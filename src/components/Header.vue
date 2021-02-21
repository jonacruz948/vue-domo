<template>
  <div>
    <v-toolbar color="black" dark fixed app>
      <v-toolbar-title>
        <v-img
          src="../assets/logo.svg"
          class="shrink mr-2"
          contain
          transition="scale-transition"
          max-width="128"
          max-height="50"
          width="100%"
      /></v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="hidden-sm-and-down">
        <v-btn
          :to="itemGuide.link"
          exact
          class="black white--text"
          min-width="96"
        >
          {{ itemGuide.name }}
        </v-btn>
        <v-btn
          :to="itemClaim.link"
          exact
          class="black  white--text"
          min-width="96"
        >
          {{ itemClaim.name }}
        </v-btn>
        <v-btn
          :to="itemBlog.link"
          exact
          class="black white--text"
          min-width="96"
        >
          {{ itemBlog.name }}
        </v-btn>
        <v-btn icon class="hidden-sm-and-down">
          <v-icon color="white">mdi-twitter</v-icon>
        </v-btn>

        <v-btn icon class="hidden-sm-and-down">
          <v-icon color="white">mdi-discord</v-icon>
        </v-btn>

        <v-btn icon class="hidden-sm-and-down">
          <v-icon color="white">mdi-github</v-icon>
        </v-btn>

        <v-btn text color="#e6007a" class="hidden-sm-and-down">
          Start Building
        </v-btn>
      </v-toolbar-items>
      <!-- <v-app-bar-nav-icon class="hidden-md-and-up"></v-app-bar-nav-icon> -->

      <v-menu class="hidden-md-and-up">
        <!-- <v-toolbar-side-icon slot="activator"></v-toolbar-side-icon> -->
        <template v-slot:activator="{ on, attrs }">
          <v-btn
            icon
            color="white"
            class="hidden-md-and-up"
            v-bind="attrs"
            v-on="on"
          >
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </template>
        <v-list class="">
          <v-list-item>
            <v-list-item-title class="black--text">{{
              itemGuide.name
            }}</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title class="black--text">{{
              itemClaim.name
            }}</v-list-item-title>
          </v-list-item>
          <v-list-item>
            <v-list-item-title class="black--text">{{
              itemBlog.name
            }}</v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
      <!-- <div class="hidden-sm-and-down">
        <v-tabs optional dark v-model="active_tab">
          <v-tab
            :to="itemGuide.link"
            exact
            class="black white--text"
            min-width="96"
          >
            {{ itemGuide.name }}
          </v-tab>
          <v-tab
            :to="itemClaim.link"
            exact
            class="black  white--text"
            min-width="96"
          >
            {{ itemClaim.name }}
          </v-tab>
          <v-tab
            :to="itemBlog.link"
            exact
            class="black white--text"
            min-width="96"
          >
            {{ itemBlog.name }}
          </v-tab>
        </v-tabs>
      </div> -->

      <!-- <v-app-bar-nav-icon></v-app-bar-nav-icon> -->
    </v-toolbar>
  </div>
</template>

<script>
export default {
  data: () => ({
    active_tab: 0,
    itemGuide: { name: "Guide", link: "/" },
    itemClaim: { name: "Claim KSM", link: "/precos" },
    itemBlog: { name: "Blog", link: "/pagesblog" },
  }),
};
</script>

<style lang="scss"></style>
