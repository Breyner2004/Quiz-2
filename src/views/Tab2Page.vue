<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>
          Departamento
        </ion-title>
      </ion-toolbar>
    </ion-header>  
    <ion-content>       
      <div id="login-container">  
        <div id="login-form">
          <GenericComponent/>
          <InputComponents id="departamento" name="departamento" label="Departamento: "/>
                      
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
import GenericComponent from '@/components/GenericComponents.vue';
import CrudButtonComponent from '@/components/CrudButtonComponents.vue';
</script>

<style scoped src="../theme/container.css"></style>