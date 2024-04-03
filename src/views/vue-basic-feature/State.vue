<template>
    <ion-page>
        <ion-header>
            <ion-toolbar color="primary">
                <ion-buttons slot="start">
                    <ion-button @click="back">
                        <ion-icon slot="icon-only" :icon="arrowBackOutline"></ion-icon>
                    </ion-button>
                </ion-buttons>
                <ion-title>State</ion-title>
            </ion-toolbar>
        </ion-header>
        <ion-content :fullscreen="true">
            
            <ion-header collapse="condense">
                <ion-toolbar>
                    <ion-title size="large">State</ion-title>
                </ion-toolbar>
            </ion-header>

            <ion-label>
                <h2>{{  nama }}</h2>
            </ion-label>

            <ion-button @click="gantiNama" expand="blok" fill="solid">
                Ganti Nama
            </ion-button>

            <br />
            <br />
            <br />

            <ion-label>
                <h2>{{  alamat }}</h2>
            </ion-label>

            <ion-button @click="gantiAlamat" expand="blok" fill="solid">
                Ganti Alamat
            </ion-button>


        </ion-content>
    </ion-page>
</template>

<script setup>
import { ref } from "vue";
import { useRouter } from "vue-router";
import { arrowBackOutline } from "ionicons/icons";

const router =useRouter()

const back = () => {
  router.back()
}

//variabel biasa
let nama = 'gg'

const gantiNama = () => {
    console.log(nama)
    
    nama = 'gf'

    console.log(nama)
}

//variabel dengan ref

let alamat = ref ('Magetan')

const gantiAlamat = () => {
    alamat.value = 'Kawedanan'
}

</script>

<style></style>