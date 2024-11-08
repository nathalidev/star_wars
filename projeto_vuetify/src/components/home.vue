<template>
  <div class="home">
    <v-row justify="start">
      <v-col cols="4">
        <v-text-field
          v-model="searchTerm"
          hint="Digite o nome do personagem"
          persistent-hint
          label="Nome"
          variant="outlined"
        ></v-text-field>
      </v-col>
    </v-row>

    <v-card-actions>
      <v-btn id="botao" variant="tonal" color="success" @click="showDialog">Pesquisar</v-btn>
    </v-card-actions>

    <!-- Dialog para mostrar o personagem encontrado -->
    <v-dialog v-model="dialog" max-width="500px">
      <v-card>
        <v-card-title class="headline">Personagem Encontrado:</v-card-title>
        <v-card-text>
          <div v-if="filteredCharacter"> <!-- Se personagem encontrado -->
            <v-img :src="filteredCharacter.image" class="align-end text-white">
              <v-card-title>{{ filteredCharacter.name }}</v-card-title>
            </v-img>
            <v-card-subtitle>{{ filteredCharacter.subtitle }}</v-card-subtitle>
            <v-card-text>
              <div>{{ filteredCharacter.description }}</div>
              <br />
              Nível de Poder: {{ filteredCharacter.power }} / 100
            </v-card-text>
          </div>
        </v-card-text>
        <v-card-actions>
          <v-btn color="primary" @click="dialog = false">Fechar</v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>

    <h3 class="mb-1">Personagens</h3>
    <v-row>
      <v-col cols="12" sm="6" md="4" lg="3" v-for="character in characters" :key="character.name">
        <v-card class="card-fixed-size d-flex flex-column">
          <v-img :src="character.image" class="align-end text-white">
            <v-card-title>{{ character.name }}</v-card-title>
          </v-img>
          <v-card-subtitle class="pt-3">{{ character.subtitle }}</v-card-subtitle>
          <v-card-text>
            <div>{{ character.description }}</div>
            <br />
            Nível de Poder: {{ character.power }} / 100
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script setup>
import { ref, computed } from 'vue';

// Dados dos personagens
const characters = [
  {
    name: "Luke Skywalker",
    subtitle: "Mestre Jedi",
    description: "Luke é considerado um dos Jedi mais poderosos da sua era. Ele demonstra habilidades excepcionais na Força.",
    power: 90,
    image: "https://imgcdn.stablediffusionweb.com/2024/4/29/9ce847cf-bfc6-4738-b372-4607b872fc14.jpg",
  },
  {
    name: "R2-D2",
    subtitle: "Droide",
    description: "R2-D2 é um droide astromech, ele desempenha papéis cruciais em várias missões.",
    power: 10,
    image: "https://75609.cdn.simplo7.net/static/75609/sku/thumb_colecionaveis-action-figures-iron-studios-r2-d2-deluxe-star-wars-sixth-scale-sideshow--p-1653332534339.jpg",
  },
  {
    name: "Darth Vader",
    subtitle: "Lord Sith (Ex Jedi)",
    description: "Anakin Skywalker, transformado em Darth Vader, se tornou um dos vilões mais temidos da galáxia.",
    power: 95,
    image: "https://media.licdn.com/dms/image/C4D12AQHC-6gk-X4sCA/article-cover_image-shrink_720_1280/0/1617995248020?e=2147483647&v=beta&t=MG8hbfEFduXhHZGgwQCzzwsoDUI7RQaxkHWjzu_TKV0"
  },
  {
    name: "C3-PO",
    subtitle: "Droide",
    description: "C-3PO é um droide de protocolo, conhecido por sua habilidade em linguística e etiqueta. Criado por Anakin Skywalker, C-3PO é fluente em mais de seis milhões de formas de comunicação.",
    power: 5,
    image: "https://lumiere-a.akamaihd.net/v1/images/c-3po-main_d6850e28.jpeg?region=176%2C0%2C951%2C536"
  },
  {
    name: "Leia Organa",
    subtitle: "Líder Política",
    description: "Após a morte de sua mãe, Leia foi adotada pelo governador de Alderaan, Bail Organa, e cresceu para se tornar uma líder carismática e determinada. Como membro da Aliança Rebelde, Leia desempenhou um papel crucial na luta contra o Império Galáctico, destacando-se por sua bravura, inteligência e habilidades e liderança.",
    power: 40,
    image: "https://i.pinimg.com/736x/f7/e2/15/f7e21564a4c39929685ad926486add77.jpg"
  },
  {
    name: "Owen Lars",
    subtitle: "Fazendeiro",
    description: "Ele é o tio adotivo de Luke Skywalker, Ele e sua esposa, Beru Whitesun, criaram Luke após a morte de Padmé Amidala e a transformação de Anakin Skywalker em Darth Vader. Owen é uma figura protetora e cautelosa, preocupado com a segurança de Luke e relutante em permitir que ele se envolva com os Jedi ou com aventuras perigosas, refletindo seu desejo de manter Luke seguro.",
    power: 8,
    image: "https://www.looper.com/img/gallery/the-untold-truth-of-owen-lars/l-intro-1652985309.jpg"
  },
  {
    name: "Beru Lars",
    subtitle: "Fazendeira",
    description: "Ela é a esposa de Owen Lars e, junto com ele, cria Luke Skywalker em Tatooine. Beru é apresentada como uma mulher gentil e amorosa, que cuida de Luke e o apoia, enquanto Owen é mais protetor e cauteloso.",
    power: 2,
    image: "https://d1m9vqlvl3fy94.cloudfront.net/role/attachment/221905/default_images__1_.jpg"

  },
  {
    name: "R5-D4",
    subtitle: "Droide",
    description: "É um droide astromech do universo de Star Wars, conhecido por sua aparência vermelha e branca. Originalmente, R5-D4 é comprado por Luke Skywalker em Tatooine para ajudá-lo em suas tarefas e, possivelmente, em aventuras futuras. No entanto, logo após a compra, R5-D4 demonstra uma falha mecânica propositada, que leva Luke a escolher outro droide",
    power: 1,
    image: "https://www.spiritkingdom.co.uk/149-medium_default/star-wars-black-series-ahsoka-r5-d4-action-figure.jpg"
  },
  {
    name: "Biggs Darklighter",
    subtittle: "Guerreiro Rebelde",
    description: "Ele é amigo de infância de Luke Skywalker e se torna um membro da equipe de pilotos da Rebelião, servindo como um dos principais pilotos de caça estelar durante a Batalha de Yavin.",
    power: 35,
    image: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR5x2Cl7g82Uwz4XdumB4uDLcxY2OizTHuOCQ&s"
  },
  {
    name: "Obi Wan Kenobi",
    subtittle: "Mestre Jedi",
    description: "Grande Mestre Jedi, Obi Wan Obi-Wan foi treinado por Qui-Gon Jinn e, após a morte de seu mestre, torna-se o mentor de Anakin Skywalker. Ele é um defensor da paz e justiça na galáxia desempenha um papel crucial nas Guerras Clônicas, lutando contra o lado sombrio e o avanço do Império. Após a queda da Ordem Jedi, Obi-Wan se exila em Tatooine, onde vigia Luke até que o jovem esteja pronto para se tornar um Jedi. Sua sabedoria, coragem habilidades na Força o tornam um dos personagens mais respeitados e admirados da saga. ",
    power: 90,
    image: "https://nsabers.es/cdn/shop/articles/opolar_Photorealistic_yet_stylized_anime_cel_shaded_Star_Wars_af471f46-f411-4783-b57d-1885fd39fe43_0.png?v=1716799055"

  }
];


const searchTerm = ref('');
const dialog = ref(false);

// Computed para filtrar o personagem com base na pesquisa
const filteredCharacter = computed(() => {
  if (searchTerm.value.trim()) {
    return characters.find(character =>
      character.name.toLowerCase().includes(searchTerm.value.toLowerCase())
    );
  }
  return null;
});

// Função para mostrar o dialog
const showDialog = () => {
  if (filteredCharacter.value) {
    dialog.value = true;  // Exibe o dialog se o personagem for encontrado
  } else {
    alert("Personagem não encontrado!");  // Exibe um alerta caso não encontre o personagem
  }
};
</script>

<style scoped>
      #image2 {
        height: 200px;
        width: 100%;
        object-fit: contain;
      } 

      .card-fixed-size{
        height: 700px;
      }

      #botao {
        margin-top: 30px;
        margin-bottom: 30px;
      }
</style>