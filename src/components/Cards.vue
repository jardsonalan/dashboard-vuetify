<template>
    <v-container>
        <h1 class="mb-6">Dashboard</h1>

        <v-card flat class="border mb-4">
          <v-card-title>Últimos usuários</v-card-title>
          
          <v-table>
            <thead>
              <tr>
                <th>Nome</th>
                <th>Email</th>
                <th>Cargo</th>
                <th>Ações</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>Fulano</td>
                <td>fulano@gmail.com</td>
                <td>Admin</td>
                <td>
                  <v-btn 
                    icon="mdi-pencil"
                    variant="tonal" 
                    color="primary"
                    density="comfortable"
                  ></v-btn>
                </td>
              </tr>
              <tr>
                <td>Cicrano</td>
                <td>cicrano@gmail.com</td>
                <td>Gerente</td>
                <td>
                  <v-btn 
                    icon="mdi-pencil"
                    variant="tonal" 
                    color="primary"
                    density="comfortable"
                  ></v-btn>
                </td>
              </tr>
              <tr>
                <td>Beltrano</td>
                <td>beltrano@gmail.com</td>
                <td>Convidado</td>
                <td>
                  <v-btn 
                    icon="mdi-pencil"
                    variant="tonal" 
                    color="primary"
                    density="comfortable"
                  ></v-btn>
                </td>
              </tr>
            </tbody>
          </v-table>
        </v-card>

        <v-row>
          <v-col cols="12" sm="6" md="4" lg="3">
            <v-card flat class="border">
              <v-img class="align-end text-black" src="https://images.pexels.com/photos/27054224/pexels-photo-27054224/free-photo-of-mar-baia-doca-vaga.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" cover>
                <v-card-title>Top 10 praias</v-card-title>
              </v-img>
              
              <v-card-subtitle class="pt-3">
                Praia
              </v-card-subtitle>
              <v-card-text>
                <div>Praia bonita</div>
                <div>Belas águas</div>
              </v-card-text>

              <v-card-actions>
                <v-btn prepend-icon="mdi-open-in-new" variant="outlined" color="primary">Ver mais</v-btn>
                <v-btn icon="mdi-home" variant="tonal" color="primary"></v-btn>
              </v-card-actions>
            </v-card>
          </v-col>

          <v-col cols="12" sm="6" md="4" lg="3">
            <v-card flat class="border">
              <v-img class="align-end text-black" src="https://images.pexels.com/photos/27054224/pexels-photo-27054224/free-photo-of-mar-baia-doca-vaga.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" cover>
                <v-card-title>Top 10 praias</v-card-title>
              </v-img>
              
              <v-card-subtitle class="pt-3">
                Praia
              </v-card-subtitle>
              <v-card-text>
                <div>Praia bonita</div>
                <div>Belas águas</div>
              </v-card-text>

              <v-card-actions>
                <v-btn prepend-icon="mdi-open-in-new" variant="outlined" color="primary">Ver mais</v-btn>
                <v-btn icon="mdi-home" variant="tonal" color="primary"></v-btn>
              </v-card-actions>
            </v-card>
          </v-col>

          <v-col cols="12" sm="6" md="4" lg="3">
            <v-card flat class="border">
              <v-img class="align-end text-black" src="https://images.pexels.com/photos/27054224/pexels-photo-27054224/free-photo-of-mar-baia-doca-vaga.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" cover>
                <v-card-title>Top 10 praias</v-card-title>
              </v-img>
              
              <v-card-subtitle class="pt-3">
                Praia
              </v-card-subtitle>
              <v-card-text>
                <div>Praia bonita</div>
                <div>Belas águas</div>
              </v-card-text>

              <v-card-actions>
                <v-btn prepend-icon="mdi-open-in-new" variant="outlined" color="primary">Ver mais</v-btn>
                <v-btn icon="mdi-home" variant="tonal" color="primary"></v-btn>
              </v-card-actions>
            </v-card>
          </v-col>

          <v-col cols="12" sm="6" md="4" lg="3">
            <v-card flat class="border">
              <v-img class="align-end text-black" src="https://images.pexels.com/photos/27054224/pexels-photo-27054224/free-photo-of-mar-baia-doca-vaga.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1" cover>
                <v-card-title>Top 10 praias</v-card-title>
              </v-img>
              
              <v-card-subtitle class="pt-3">
                Praia
              </v-card-subtitle>
              <v-card-text>
                <div>Praia bonita</div>
                <div>Belas águas</div>
              </v-card-text>

              <v-card-actions>
                <v-btn prepend-icon="mdi-open-in-new" variant="outlined" color="primary">Ver mais</v-btn>
                <v-btn icon="mdi-home" variant="tonal" color="primary"></v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
</template>

<script setup lang="ts">
    //
</script>  