<template>
    <v-app-bar flat>
        <v-app-bar-nav-icon></v-app-bar-nav-icon>
        <v-app-bar-title>Meu App</v-app-bar-title>

        <template #append>
            <v-btn icon class="mr-2">
                <v-badge dot color="info">
                    <v-icon icon="mdi-bell-outline"></v-icon>
                </v-badge>
            </v-btn>
            <v-avatar>
                <v-img
                    src="https://images.pexels.com/photos/27333753/pexels-photo-27333753/free-photo-of-cidade-meio-urbano-moda-tendencia.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
                    cover
                ></v-img>
            </v-avatar>
        </template>
    </v-app-bar>
</template>
  
<script setup lang="ts">
    //
</script>  