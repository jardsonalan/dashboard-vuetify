<template>
    <v-navigation-drawer v-model="isDrawerOpen">
        <v-list>
            <v-list-item prepend-icon="mdi-home">Home</v-list-item>
            <v-list-item prepend-icon="mdi-account">Usuários</v-list-item>

            <v-list-group value="Clientes">
                <template v-slot:activator="{ props }">
                    <v-list-item
                        v-bind="props"
                        prepend-icon="mdi-account-circle"
                        title="Clientes"
                    >
                    </v-list-item>
                </template>

                <v-list-item prepend-icon="mdi-currency-usd">Vendas</v-list-item>
                <v-list-item prepend-icon="mdi-chart-line">Relatório</v-list-item>
            </v-list-group>
        </v-list>
    </v-navigation-drawer>

    <v-app-bar flat class="border-b">
        <v-app-bar-nav-icon @click="isDrawerOpen = !isDrawerOpen"></v-app-bar-nav-icon>
        <v-app-bar-title>Meu App</v-app-bar-title>

        <template #append>
            <v-menu>
                <template #activator="{ props }">
                    <v-btn icon class="mr-2" v-bind="props">
                        <v-badge dot color="info">
                            <v-icon icon="mdi-bell-outline"></v-icon>
                        </v-badge>
                    </v-btn>
                </template>
                <v-card min-width="300px">
                    <v-list :lines="false" density="compact">
                        <v-list-item>
                            <v-list-item-title>Notificações</v-list-item-title>
                        </v-list-item>
                    </v-list>
                </v-card>
            </v-menu>

            <v-menu>
                <template #activator="{ props }">
                    <v-avatar v-bind="props">
                        <v-img
                            src="https://images.pexels.com/photos/27333753/pexels-photo-27333753/free-photo-of-cidade-meio-urbano-moda-tendencia.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
                            cover
                        ></v-img>
                    </v-avatar>
                </template>
                <v-card min-width="200px">
                    <v-list :lines="false" density="compact" nav>
                        <v-list-item prepend-icon="mdi-account-outline">
                            <v-list-item-title>Meu perfil</v-list-item-title>
                        </v-list-item>
                        <v-list-item prepend-icon="mdi-heart-outline">
                            <v-list-item-title>Favoritos</v-list-item-title>
                        </v-list-item>
                    </v-list>
                </v-card>
            </v-menu>

        </template>
    </v-app-bar>
</template>
  
<script setup lang="ts">
import { ref } from 'vue';

    const isDrawerOpen = ref(false)
</script>  