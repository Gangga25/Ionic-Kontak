<template>
    <ion-page>
        <ion-header>
            <ion-toolbar>
                <ion-title>Todo Apps</ion-title>
            </ion-toolbar>
        </ion-header>

        <ion-content :fullscreen="true">
            <ion-list>
                <ion-list-header>
                    <ion-label>TodoOOO</ion-label>
                </ion-list-header>

                <ion-item>
                    <ion-label>
                        <h2>GG</h2>
                        <P>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eaque deleniti dignissimos sequi, officiis quam non modi officia dolores quaerat itaque beatae aspernatur quasi fugit nam? Voluptatem eum molestias tempora aperiam!</P>
                    </ion-label>
                </ion-item>

                <ion-item>
                    <ion-label>
                        <h2>GG</h2>
                        <P>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eaque deleniti dignissimos sequi, officiis quam non modi officia dolores quaerat itaque beatae aspernatur quasi fugit nam? Voluptatem eum molestias tempora aperiam!</P>
                    </ion-label>
                </ion-item>

                <ion-item>
                    <ion-label>
                        <h2>GG</h2>
                        <P>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eaque deleniti dignissimos sequi, officiis quam non modi officia dolores quaerat itaque beatae aspernatur quasi fugit nam? Voluptatem eum molestias tempora aperiam!</P>
                    </ion-label>
                </ion-item>
            </ion-list>

            <ion-fab slot="fixed" horizontal="end" vertical="bottom">
                <ion-fab-button>
                    <ion_icon :icon="add"></ion_icon>
                </ion-fab-button>
            </ion-fab>

        </ion-content>
    </ion-page>
</template>

<script setup>
import { logoIonic, add} from 'ionicons/icons';
</script>

<style>
ion-content {
    height: 90%;
}
</style>