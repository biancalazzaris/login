<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title class="bg-header">
            <div class="header">
                <h1>Login</h1>
            </div>
        </ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
            <ion-title class="bg-header">
                <div class="header">
                    <h1>Login</h1>
                </div>
            </ion-title>
        </ion-toolbar>
      </ion-header>
      <div>
        <div class="container">
          <div class="bg">
            <ion-item class="item">
              <ion-label position="floating">Email</ion-label>
              <ion-input type="email"></ion-input>
            </ion-item>
            <ion-item class="item">
              <ion-label position="floating">Senha</ion-label>
              <ion-input type="password"></ion-input>
            </ion-item>
            <ion-button class="btn" color="light" expand="block" href="/home">Login</ion-button>
          </div>
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
    IonItem,
    IonLabel,
    IonInput
} from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'Login',
  components: {
    IonContent,
    IonHeader,
    IonPage,
    IonTitle,
    IonToolbar,
    IonButton,
    IonItem,
    IonLabel,
    IonInput
  }
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
  justify-content: center;
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
  margin-bottom:  20px;
  border-radius: 10px;
}
</style>