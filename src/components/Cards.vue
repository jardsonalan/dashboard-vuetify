<template>
    <v-container>
        <h1 class="mb-6">Dashboard</h1>

        <v-card flat class="border mb-4">
          <div class="d-flex justify-space-between">
            <v-card-title>Últimos usuários</v-card-title>
            
            <!-- Evita conflitos no código -->
            <v-card-title>
              <!-- Chamada para abrir o dialog -->
              <v-btn 
                @click="isDialogOpen = true"
                flat 
                class="border" 
                variant="tonal"
                size="small"
              >
                Adicionar usuário
              </v-btn>

              <v-dialog
                v-model="isDialogOpen"
                width="600px"
              >
                <v-card>
                  <v-card-title>Adicionar usuário</v-card-title>

                  <v-card-text>
                    <v-row>
                      <v-col>
                        <v-text-field label="Nome" variant="outlined"></v-text-field>
                      </v-col>

                      <v-col>
                        <v-text-field 
                          label="Email" 
                          variant="outlined"
                          :rules="emailRules"
                        >
                        </v-text-field>
                      </v-col>
                    </v-row>

                    <v-select 
                      label="Cargo" 
                      variant="outlined"
                      :items="cargos"
                    >
                    </v-select>
                  </v-card-text>

                  <v-card-actions>
                    <v-spacer></v-spacer>
                    <v-btn variant="text" @click="isDialogOpen = false">Cancelar</v-btn>
                    <v-btn variant="tonal" color="success">Salvar</v-btn>
                  </v-card-actions>
                </v-card>
              </v-dialog>
            </v-card-title>

          </div>
          
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
                <td>
                  <v-chip color="primary" variant="outlined" size="small">Admin</v-chip>
                </td>
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
                <td>
                  <v-chip color="success" variant="outlined" size="small">Gerente</v-chip>
                </td>
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
                <td>
                  <v-chip variant="outlined" size="small">Convidado</v-chip>
                </td>
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
import { ref } from 'vue';

    const isDialogOpen = ref(false)

    const cargos = ['Admin', 'Gerente', 'Convidado']

    // Validação de email - simples
    const emailRules = [
      value => {
        if (value) {
          return true;
        } else {
          return 'Email obrigatório';
        }
      },
      value => {
        if (value.includes('@')) {
          return true;
        } else {
          return 'Email inválido';
        }
      }
    ]
</script>  