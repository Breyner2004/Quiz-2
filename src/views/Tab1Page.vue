<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>
          Pais
        </ion-title>
      </ion-toolbar>
    </ion-header>  
    <ion-content>       
      <div id="login-container">  
        <div id="login-form">
             <GenericComponents/>   
             <InputComponents id="pais" name="pais" label="Pais: "/>
        </div>

        <div> 
           <!--Traer el componente de los botones de la crud  -->
          <CrudButtonComponent />
        </div>          
      </div>
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
import InputComponents from '@/components/InputComponents.vue';
import CrudButtonComponent from '@/components/CrudButtonComponents.vue';
import GenericComponents from '@/components/GenericComponents.vue';
</script>

<style scoped src="../theme/container.css"></style>