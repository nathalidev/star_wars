<template>
  <v-app>
    <v-navigation-drawer v-model="isDrawerOpen" app temporary>
      <v-list>
        <v-list-subheader>Menu</v-list-subheader>
        <v-list-item prepend-icon="mdi-home" @click="OnView('home')"
          >Home</v-list-item
        >
        <v-list-item prepend-icon="mdi-earth" @click="OnView('planetas')"
          >Planetas</v-list-item
        >
      </v-list>
    </v-navigation-drawer>

    <v-app-bar color="light-blue-darken-4">
      <v-app-bar-nav-icon
        @click="isDrawerOpen = !isDrawerOpen"
      ></v-app-bar-nav-icon>
      <v-app-bar-title class="text-h4 font-weight-bold"
        >Star Wars</v-app-bar-title
      >
      <template #append>
        Que a força esteja com você!
        <v-menu>
          <template #activator="{ props }">
            <v-avatar v-bind="props" class="ml-4">
              <v-img
                cover
                src="https://mir-s3-cdn-cf.behance.net/project_modules/fs/6dc20168040289.5b56a4fb13105.gif"
              ></v-img>
            </v-avatar>
          </template>
        </v-menu>
      </template>
    </v-app-bar>

    <v-main>
      <v-container>
        <home v-if="view == 'home'" />

        <planetas v-else />
      </v-container>
      <router-view />
    </v-main>
  </v-app>
</template>

<script setup>
import { ref } from "vue";
const isDrawerOpen = ref(false);

const view = ref("home");

const OnView = (pview) => {
  view.value = pview;
};
</script>

<style>
.v-img__img--contain {
  object-fit: cover !important;
}
</style>