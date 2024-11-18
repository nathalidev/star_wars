<template>
  <div class="home">
    <v-row justify="start">
      <v-col cols="12" sm="6" md="4" lg="3" v-for="(planeta, index) in planetas " :key="index">
        <v-card class="card-fixed-size d-flex flex-column">
          <v-img :src="planeta.imagem" class="align-end text-white"></v-img>
          <v-card-subtitle class="pt-3">{{ planeta.nome_planeta }}</v-card-subtitle>
          <v-card-text>
            <div>
              {{ planeta.mini_descricao }}
            </div>
            <v-btn
                  color="surface-variant"
                  text="VER MAIS"
                  variant="flat"
                  @click="showDialog"
                  style="margin-top: 20px;"
                ></v-btn>
          </v-card-text>

          <v-card-actions>
            <v-dialog v-model="dialog" max-width="500">
                <v-card :title="planetas.nome_planeta">
                  <v-card-text>
                    <p style="font-weight: 700; color: yellow;">1. Localização</p>
                    <li style="font-weight: 500;"><strong class="font-weight text-yellow">Região:</strong> {{ planeta.regiao }}</li>
                    <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistema:</strong>{{ planeta.sistema }}</li>
                    <li style="font-weight: 500;"><strong class="font-weight text-yellow">Tipo de planeta:</strong>{{ planeta.tipo_planeta }}</li>
                    <li style="font-weight: 500;"><strong class="font-weight text-yellow">Atmosfera:</strong>{{ planeta.atmosfera }}</li><br>
                    <v-spacer></v-spacer>
                    <p style="font-weight: 700; color: yellow;">2.Clima e Ambiente</p>
                    <li style="font-weight: 500;"><strong class="font-weight text-yellow">Clima:</strong>{{ planeta.clima }}</li><br>
                    <v-spacer></v-spacer>
                    <p style="font-weight: 700; color: yellow;">3.Geografia e terreno</p>
                    <li style="font-weight: 500;"><strong class="font-weight text-yellow">Geografia e terreno:</strong>{{ planeta.geografia_terreno }}</li><br>
                    <v-spacer></v-spacer>
                    <p style="font-weight: 700; color: yellow;">4. Ecossistema e vida selvagem</p>
                    <li style="font-weight: 500;"><strong class="font-weight text-yellow">Espécies Nativas:</strong>{{ planeta.especies }}</li>
                    <li style="font-weight: 500;"><strong class="font-weight text-yellow">Flora:</strong>{{ planeta.flora }}</li>
                  </v-card-text>

                  <v-card-actions>
                    <v-spacer></v-spacer>

                    <v-btn
                      text="Fechar"
                      @click="dialog = false"
                    ></v-btn>
                  </v-card-actions>
                </v-card>
            </v-dialog>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script setup>
const planetas = [
  {
    nome_planeta: "Tatooine",
    imagem: "https://wallpapers.com/images/hd/tatooine-1920-x-1080-wallpaper-3xa2werbhbugk3rw.jpg",
    mini_descricao: "Tatooine é um planeta desértico fictício do universo de Star Wars, conhecido por seu clima árido, vastos mares de areia e dois sóis, Tatoo I e Tatoo II. Localizado nas regiões do Borda Exterior, é o lar de comunidades como os fazendeiros de umidade e os Tusken Raiders. Embora pareça isolado e insignificante, Tatooine desempenha um papel crucial na saga, sendo o planeta natal de Anakin Skywalker e o local onde Luke Skywalker cresceu. É famoso por abrigar contrabandistas, caçadores de recompensas e outras figuras de moral duvidosa, como no porto espacial de Mos Eisley.",
    regiao: "Borda Exterior",
    sistema: "Sistema Tatoo",
    tipo_planeta: "Desértico",
    atmosfera: "Respirável",
    clima: "Árido",
    geografia_terreno: "Dunas de areia, planícies rochosas",
    especies: "Jawas, Tusken Raiders",
    flora: "Escassa",
  },
  {
    nome_planeta: "Naboo",
    imagem: "https://i.pinimg.com/550x/c5/b0/46/c5b04637a454d967501d4ff662a663ca.jpg",
    mini_descricao: "Naboo é um planeta exuberante com vastas planícies verdes, lagos cristalinos e cidades majestosas como Theed. É conhecido como o lar da Rainha Amidala e do Gungan Jar Jar Binks.",
    regiao: "Borda Média",
    sistema: "Sistema Naboo",
    tipo_planeta: "Terrestre",
    atmosfera: "Respirável",
    clima: "Tropical",
    geografia_terreno: "Montanhas, lagos, planícies",
    especies: "Gungans, Humanos",
    flora: "Densa e variada",
  },
  {
    nome_planeta: "Coruscant",
    imagem: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSYJ0RmqLmXmlnWLHCfinhQrWx_7tDah84IAw&s",
    mini_descricao: "Coruscant é o centro político e cultural da galáxia, coberto inteiramente por uma cidade-estado futurística. É a sede do Senado Galáctico.",
    regiao: "Núcleo",
    sistema: "Sistema Coruscant",
    tipo_planeta: "Urbano",
    atmosfera: "Respirável",
    clima: "Temperado",
    geografia_terreno: "Cidades, arranha-céus",
    especies: "Diversas",
    flora: "Praticamente inexistente",
  },
  {
    nome_planeta: "Hoth",
    imagem: "https://images7.alphacoders.com/641/641852.jpg",
    mini_descricao: "Hoth é um planeta gélido, coberto por gelo e neve. Foi o esconderijo temporário da Aliança Rebelde, famoso pela Batalha de Hoth.",
    regiao: "Borda Exterior",
    sistema: "Sistema Hoth",
    tipo_planeta: "Gelado",
    atmosfera: "Respirável",
    clima: "Árctico",
    geografia_terreno: "Planícies de gelo, cavernas de gelo",
    especies: "Wampas, Tauntauns",
    flora: "Escassa",
  },
  {
    nome_planeta: "Dagobah",
    imagem: "https://wallpapers.com/images/hd/dagobah-1920-x-816-wallpaper-pecj7ug7l1x66263.jpg",
    mini_descricao: "Dagobah é um planeta pantanoso e isolado, onde o Mestre Yoda viveu durante seu exílio. É conhecido por sua densa vegetação e atmosfera mística.",
    regiao: "Borda Exterior",
    sistema: "Sistema Dagobah",
    tipo_planeta: "Pantanal",
    atmosfera: "Respirável",
    clima: "Úmido",
    geografia_terreno: "Pântanos, florestas densas",
    especies: "Diversas criaturas selvagens",
    flora: "Densa e variada",
  },
  {
    nome_planeta: "Endor",
    imagem: "https://steamuserimages-a.akamaihd.net/ugc/795360029428849700/EF543AC35BC2498C6F4B9265D41726337B7AFDD7/?imw=637&imh=358&ima=fit&impolicy=Letterbox&imcolor=%23000000&letterbox=true",
    mini_descricao: "Endor é uma lua florestal coberta por árvores gigantescas e o lar dos Ewoks. Foi palco da batalha crucial contra o Império Galáctico.",
    regiao: "Borda Exterior",
    sistema: "Sistema Moddell",
    tipo_planeta: "Florestal",
    atmosfera: "Respirável",
    clima: "Temperado",
    geografia_terreno: "Florestas densas",
    especies: "Ewoks",
    flora: "Árvores gigantescas",
  },
  {
    nome_planeta: "Mustafar",
    imagem: "https://wallpapercave.com/wp/wp7512245.jpg",
    mini_descricao: "Mustafar é um planeta vulcânico e hostil, coberto por rios de lava. Foi o local do confronto entre Anakin Skywalker e Obi-Wan Kenobi.",
    regiao: "Borda Exterior",
    sistema: "Sistema Mustafar",
    tipo_planeta: "Vulcânico",
    atmosfera: "Respirável com suporte",
    clima: "Quente",
    geografia_terreno: "Vulcões, rios de lava",
    especies: "Mustafarianos",
    flora: "Inexistente",
  },
  {
    nome_planeta: "Kashyyyk",
    imagem: "https://i.pinimg.com/originals/d9/ff/6b/d9ff6b62ee71d33c67b2899b038e7e27.jpg",
    mini_descricao: "Kashyyyk é um planeta coberto por florestas tropicais e lar dos Wookiees, incluindo Chewbacca. É conhecido por sua densa vegetação e árvores altíssimas.",
    regiao: "Borda Média",
    sistema: "Sistema Kashyyyk",
    tipo_planeta: "Florestal",
    atmosfera: "Respirável",
    clima: "Tropical",
    geografia_terreno: "Florestas, rios",
    especies: "Wookiees",
    flora: "Rica e diversa",
  },
];

const dialog = ref(false);

const showDialog = () => {
  dialog.value = true;  // Exibe o dialog se o personagem for encontrado
};
</script>

<style scoped>
  #image {
    height: 200px;
    width: 100%;
    object-fit: contain;
  } 

  .card-fixed-size {
    height: 700px;
  }
</style>
