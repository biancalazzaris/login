<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title class="bg-header">
          <div class="header">
            <h1>Home</h1>
            <ion-button color="light" href="/">Login</ion-button>
          </div></ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title class="bg-header">
            <div class="header">
              <h1>Home</h1>
            </div>
          </ion-title>
        </ion-toolbar>
      </ion-header>
      <div>
        <div class="container">
          <ion-button color="light" href="/school">School</ion-button>
        </div>
      </div>
    </ion-content>
  </ion-page>
</template>

<script lang="ts">
import {
  IonContent,
  IonHeader,
  IonPage,
  IonTitle,
  IonToolbar,
  IonButton,
} from "@ionic/vue";
import { defineComponent } from "vue";
export default defineComponent({
  name: "Home",
  components: {
    IonContent,
    IonHeader,
    IonPage,
    IonTitle,
    IonToolbar,
    IonButton,
  },
});
</script>

<style scoped>
.bg-header {
  background-color: #000000;
  color: #ffffff;
}
.header {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.container {
  height: 93vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #321b36;
}
.bg {
  padding: 20px;
  border-radius: 5px;
  background-color: #75219c;
}
.item {
  margin-bottom: 20px;
  border-radius: 10px;
}
</style>