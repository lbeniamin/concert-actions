<template>
  <v-container class="fill-height" max-width="900">
    <div class="mx-auto">
      <v-img class="mb-4" height="150" src="@/assets/logo.webp"/>
      <div class="mb-8 text-center">
        <div class="text-body-2 font-weight-regular mb-n1">POLAND</div>
        <h1 class="text-h2 font-weight-bold">LINKIN PARK</h1>
      </div>
    </div>
    <div class="actionsContainer pa-4">
      <h2 class="font-weight-bold text-center mb-6">Opener Festival 2025 - Akcje koncertowe</h2>
      <div class="action d-flex">
        <img height="150" src="@/assets/welcome-back.webp" alt="Welcome back" class="mr-4" />
        <div class="d-flex flex-column justify-space-around">
          <h3 class="mb-2">Kartki "Welcome back"</h3>
          <p class="mb-2">Na początku koncertu wszyscy podnosimy kartki z napisem "WELCOME BACK", tworząc niesamowity widok dla zespołu. Pokażmy im naszą jedność, wsparcie i wdzięczność za powrót! 🖤</p>
          <v-btn append-icon="mdi-chevron-triple-right" :ripple="false" variant="outlined" @click="openAction1">Czytaj więcej</v-btn>
        </div>
      </div>
      <v-divider class="my-4"/>
      <div class="action d-flex">
        <img height="150" src="@/assets/welcome-back.webp" alt="Welcome back" class="mr-4" />
        <div class="d-flex flex-column justify-space-around">
          <h3 class="mb-2">Kartki "Welcome back"</h3>
          <p class="mb-2">Na początku koncertu wszyscy podnosimy kartki z napisem "WELCOME BACK", tworząc niesamowity widok dla zespołu. Pokażmy im naszą jedność, wsparcie i wdzięczność za powrót! 🖤</p>
          <v-btn append-icon="mdi-chevron-triple-right" :ripple="false" variant="outlined" @click="openAction1">Czytaj więcej</v-btn>
        </div>
      </div>
      <v-divider class="my-4"/>
      <div class="action d-flex">
        <img height="150" src="@/assets/welcome-back.webp" alt="Welcome back" class="mr-4" />
        <div class="d-flex flex-column justify-space-around">
          <h3 class="mb-2">Kartki "Welcome back"</h3>
          <p class="mb-2">Na początku koncertu wszyscy podnosimy kartki z napisem "WELCOME BACK", tworząc niesamowity widok dla zespołu. Pokażmy im naszą jedność, wsparcie i wdzięczność za powrót! 🖤</p>
          <v-btn append-icon="mdi-chevron-triple-right" :ripple="false" variant="outlined" @click="openAction1">Czytaj więcej</v-btn>
        </div>
      </div>
    </div>
  </v-container>
</template>

<script setup lang="ts">
const ACTION_1 = 'https://www.facebook.com/LPPoland/posts/pfbid0zNfQ6ZrVDFAZ8xnr2VNVtoEveCdfi2F63UK641EK7gjUo7pmhbpHbQzmFQydvGRYl';

function openAction1(): void {
  window.open(ACTION_1, '_blank');
}
</script>
<style lang="scss">
.v-container {
  user-select: none;
}
.actionsContainer {
  user-select: none;
  background-color: #282828;
  width: 100%;
  border-radius: 8px;
  h2 {
    font-size: 24px;
  }
  h3 {
    font-size: 18px;
  }
  p {
    font-size: 13px;
  }
  button {
    width: fit-content;
    .v-btn__append i {
      margin-top: -1px;
    }
  }
  @media (max-width: 599px) {
    .action {
      flex-direction: column;
      align-items: center;
      img {
        margin-right: 0 !important;
        width: fit-content;
        margin-bottom: 8px;
      }
      h3, p {
        text-align: center;
      }
      button {
        margin: 0 auto;
      }
    }
  }
}
@media (max-width: 599px) {
  h1.text-h2 {
    font-size: 2.5rem !important;
  }
}
</style>
