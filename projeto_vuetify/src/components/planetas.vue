<template>
  <div class="home">
    <v-row justify="start">
      <v-col cols="12" sm="6" md="4" lg="3">
        <v-card class="card-fixed-size d-flex flex-column"> <!-- Para colocar o ícone lá embaixo -->
          <v-img class="align-end text-white" id="image" src="https://oyster.ignimgs.com/mediawiki/apis.ign.com/star-wars-episode-7/4/4b/Tatooine-3.jpg"> </v-img>
            <v-card-subtitle class="pt-3">Tatooine</v-card-subtitle>
            <v-card-text>
              <div>
                É um planeta desértico localizado na borda exterior da galáxia de "Star Wars".<br>
                Conhecido por suas vastas dunas de areia, Tatooine possui um clima extremamente árido
                com temperaturas que podem ser muito altas durante o dia e bastante frias à noite.
              </div>
            </v-card-text>
  
            <v-card-actions>
              <v-dialog max-width="500">
  <template v-slot:activator="{ props: activatorProps }">
    <v-btn
      v-bind="activatorProps"
      color="surface-variant"
      text="VER MAIS"
      variant="flat"
    ></v-btn>
  </template>

  <template v-slot:default="{ isActive }">
    <v-card title="Tatooine">
      <v-card-text>
        <p style="font-weight: 700; color: yellow;">1. Localização e tipo</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Região:</strong> Orla Exterior da galáxia</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistema:</strong>Sistema Tatoo</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Tipo de planeta:</strong> Planeta desértico e inóspito</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Atmosfera:</strong> Respirável para a maioria das espécies; ar seco e quente, o que contribui para a sensação de aridez</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">2. Clima e Ambiente</p>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">Clima:</strong> Extremamente árido, com temperaturas muito altas durante o dia e quedas significativas à noite</li>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistemas Solares:</strong> Tatooine orbita dois sóis, Tatoo I e Tatoo II, criando um efeito de “sol gêmeo” e temperaturas intensas</li>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">Areias e tempestades:</strong> O planeta é quase inteiramente coberto por desertos, com frequentes tempestades de areia que podem durar dias</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">3. Geografia e Terreno</p>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">Dunas e Desertos:</strong> Possui vastas áreas de dunas de areia, que dominam o terreno</li>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">Cânions e Cavernas:</strong> Possui vastas áreas de dunas de areia, que dominam o terreno</li>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">Oásis Raros:</strong> Possui vastas áreas de dunas de areia, que dominam o terreno</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">4. Ecossistema e Vida Selvagem</p>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">Espécies Nativas:</strong> Inclui os Tusken Raiders (Povo da Areia) e os Jawas, além de criaturas como o Bantha (um tipo de mamífero peludo usado como transporte pelos Tusken Raiders), o Sarlacc (predador que se enterra na areia) e o Krayt Dragon (um grande predador do deserto)</li>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">Plantas e Água:</strong> Raríssimas plantas resistentes ao clima e a água é extremamente escassa e cara, sendo coletada em fazendas de umidade</li>
      </v-card-text>

      <v-card-actions>
        <v-btn
          text="Fechar"
          @click="isActive.value = false"
        ></v-btn>
      </v-card-actions>
    </v-card>
  </template>
</v-dialog>
            </v-card-actions>
          </v-card>
        </v-col>

        <v-col cols="12" sm="6" md="4" lg="3">
            <v-card class="card-fixed-size d-flex flex-column">
            <v-img class="align-end text-white" id="image" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ4NRbDcTr7icmfi6cnqG8vKdchtaVI89y3Qw&s"> </v-img>
            <v-card-subtitle class="pt-3">Naboo</v-card-subtitle>
            <v-card-text>
              <div>
                Naboo é um planeta rico e diversificado, conhecido por suas paisagens exuberantes, grandes lagos, colinas verdes e cidades magníficas. 
                A arquitetura de Naboo é distinta, combinando elementos clássicos com toques futuristas.<br>
                <br>O planeta é habitado por duas principais espécies: os humanos de Naboo e os Gungans, que vivem em áreas aquáticas e subterrâneas. 
                Os Naboo são conhecidos por sua cultura pacífica e apreciativa das artes.
              </div>
            </v-card-text>
  
            <v-card-actions>
              <v-dialog max-width="500">
  <template v-slot:activator="{ props: activatorProps }">
    <v-btn
      v-bind="activatorProps"
      color="surface-variant"
      text="VER MAIS"
      variant="flat"
    ></v-btn>
  </template>

  <template v-slot:default="{ isActive }">
    <v-card title="Naboo">
      <v-card-text>
        <p style="font-weight: 700; color: yellow;">1. Localização e tipo</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Região:</strong>Região Central da Galáxia</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistema:</strong>Sistema Chommell</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Tipo de planeta:</strong> Planeta temperado e rico em ecossistemas diversos, como florestas, planícies e lagos</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Atmosfera:</strong> Respirável para a maioria das espécies, com uma atmosfera rica em oxigênio. O clima é moderado e agradável, com uma umidade saudável, favorecendo uma vegetação luxuriante e vida selvagem diversificada.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">2. Clima e Ambiente</p>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">Clima:</strong> O clima de Naboo é temperado, com estações bem definidas. As temperaturas são amenas e agradáveis, com verões quentes e invernos suaves. A umidade é relativamente alta, favorecendo a vegetação exuberante e os ecossistemas aquáticos.</li>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistemas Solares:</strong> Naboo orbita um único sol, o que resulta em uma temperatura equilibrada e uma luz solar suave, ideal para o crescimento da vegetação e a manutenção de um ecossistema sustentável.</li>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">Precipitação e Águas:</strong> O planeta possui grandes reservas de água doce, com uma rede de rios, lagos e até oceanos. A precipitação é frequente, contribuindo para a fertilidade do solo e o desenvolvimento de uma rica flora.
        </li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">3. Geografia e Terreno</p>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">FLorestas e Planícies:</strong> Naboo é conhecido por suas vastas planícies cobertas por campos verdes e suaves, com vegetação densa e florestas escuras, habitadas por uma grande variedade de fauna. As planícies são pontuadas por colinas e montanhas baixas que oferecem uma vista deslumbrante das vastas terras e oceanos.</li>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">Lagos e Áreas Aquáticas:</strong> O planeta é salpicado por lagos tranquilos e uma grande rede de rios e córregos. Os famosos lagos de Naboo são um dos maiores atrativos naturais, proporcionando um ambiente pacífico e ideal para muitas formas de vida. Esses corpos d'água são interconectados por uma densa vegetação que embeleza ainda mais o território.</li>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">Cidades e Arquitetura:</strong> A arquitetura de Naboo é notável, com construções elegantes e refinadas, muitas das quais foram feitas para se integrar à paisagem natural do planeta. A cidade de Theed, a capital de Naboo, é um exemplo impressionante disso, com suas grandes praças, colunas esculpidas e palácios majestosos que refletem a história cultural e política do planeta.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">4. Ecossistema e Vida Selvagem</p>
        <li style="font-weight: 500;"><strong class="font-weight text-yellow">Espécies Nativas:</strong> O ecossistema de Naboo é diversificado, com muitas espécies nativas adaptadas ao ambiente tranquilo do planeta. Entre os habitantes mais conhecidos estão os Gungans, uma raça anfíbia que vive em cidades subaquáticas e que, embora tecnologicamente menos avançada que os humanos de Naboo, são habilidosos e ferozes guerreiros. Além dos Gungans, o planeta abriga diversas criaturas, como o Bantha, o Kaadu (um animal usado para transporte), o Opee Sea Killer (uma criatura aquática do pântano) e o Nysillin, uma espécie de anfíbio raro.</li>
      </v-card-text>

      <v-card-actions>
        <v-btn
          text="Fechar"
          @click="isActive.value = false"
        ></v-btn>
      </v-card-actions>
    </v-card>
  </template>
  </v-dialog>
            </v-card-actions>
          </v-card>
        </v-col>
  
        <v-col cols="12" sm="6" md="4" lg="3">
            <v-card class="card-fixed-size d-flex flex-column">
            <v-img
              class="align-end text-white" id="image"
              src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRHjRsM1LwX7EIaNIRyeDHD54mCQ7H0GmnMjw&s"> </v-img>
            <v-card-subtitle class="pt-3">Mustafar</v-card-subtitle>
            <v-card-text>
              <div>
                Mustafar é um planeta vulcânico, conhecido por suas paisagens de lava, erupções vulcânicas e um clima extremamente hostil. 
                O planeta é coberto por rios de lava e possui uma atmosfera densa, com fumaça e cinzas.<br><br>Mustafar simboliza a queda de Anakin para o lado sombrio da Força e sua transformação em Darth Vader, 
                marcando um ponto de virada importante na saga "Star Wars".
              </div>
            </v-card-text>
  
            <v-card-actions>
              <v-dialog max-width="500">
  <template v-slot:activator="{ props: activatorProps }">
    <v-btn
      v-bind="activatorProps"
      color="surface-variant"
      text="VER MAIS"
      variant="flat"
    ></v-btn>
  </template>

  <template v-slot:default="{ isActive }">
    <v-card title="Mustafar">
      <v-card-text>
        <p style="font-weight: 700; color: yellow;">1. Localização e tipo</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Região:</strong> Região Leste da galáxia</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistema:</strong>Sistema Mustafar</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Tipo de planeta:</strong> Planeta vulcânico e inóspito</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Atmosfera:</strong> A atmosfera de Mustafar é densa, composta principalmente por dióxido de enxofre e outros gases tóxicos, tornando-a extremamente perigosa para a maioria das formas de vida sem equipamentos adequados. A respiração direta sem proteção é quase impossível.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">2. Clima e Ambiente</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Clima:</strong> Em Mustafar é um planeta com temperaturas extremamente altas devido à sua atividade vulcânica intensa. A maior parte de sua superfície está coberta por rios de lava e colunas de fogo, criando um ambiente infernal.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistemas Solares:</strong> Mustafar orbita um único sol, mas a principal característica climática é sua atividade geotérmica constante, que torna a temperatura do planeta muito elevada o tempo todo, com zonas de calor extremo.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">3. Geografia e Terreno</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Vulcões e Rios de Lava:</strong> O terreno de Mustafar é dominado por vastos campos de lava, com vulcões ativos espalhados pela sua superfície. Os rios de lava serpenteiam pelo planeta, formando redes de calor intenso e se espalhando por quase toda a superfície.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Cânions e Fendas:</strong> As erupções vulcânicas e os processos geológicos constantes criam enormes fendas e cânions, que são muito profundos e perigosos. Essas fissuras, às vezes, são preenchidas com lava líquida que corre para os vales abaixo.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Oásis Raros:</strong> Possui vastas áreas de dunas de areia, que dominam o terreno</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">4. Ecossistema e Vida Selvagem</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Espécies Nativas:</strong> A espécie nativa mais conhecida de Mustafar são os Mustafarianos, uma raça de seres que se adaptaram às condições extremas do planeta. Eles possuem pele resistente ao calor e são frequentemente vistos trabalhando nas minas ou em instalações de processamento de minerais.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Flora:</strong> A vegetação em Mustafar é praticamente inexistente, exceto por algumas plantas resistentes ao calor e musgos que podem ser encontrados em áreas mais protegidas. Estas plantas são adaptadas a sobreviver em solos extremamente ricos em minerais e gases vulcânicos.</li>
      </v-card-text>

      <v-card-actions>
        <v-spacer></v-spacer>

        <v-btn
          text="Fechar"
          @click="isActive.value = false"
        ></v-btn>
      </v-card-actions>
    </v-card>
  </template>
</v-dialog>
            </v-card-actions>
          </v-card>
        </v-col>
  
        <v-col cols="12" sm="6" md="4" lg="3">
            <v-card class="card-fixed-size d-flex flex-column">
            <v-img
              class="align-end text-white" id="image"
              src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTiPDrYOT5OyqcdYwncRABiWHI1_DRGu2NqZg&s"
            >
            </v-img>
            <v-card-subtitle class="pt-3">Coruscant</v-card-subtitle>
            <v-card-text>
              <div>
                Coruscant é um planeta totalmente urbano, coberto por uma imensa cidade que se estende por toda a sua superfície. A cidade é composta por arranha-céus, infraestruturas avançadas e um sistema de transporte muito desenvolvido. 
                O planeta não possui áreas naturais significativas, pois toda a sua superfície é dominada pela urbanização.
              </div>
            </v-card-text>
  
            <v-card-actions>
              <v-dialog max width = "500">
  <template v-slot:activator="{props:activatorProps}">
    <v-btn
      v-bind="activatorProps"
      color="surface-variant"
      text="VER MAIS"
      variant="flat"
    ></v-btn>
  </template>

  <template v-slot:default="{ isActive }">
    <v-card title="Coruscant">
      <v-card-text>
        <p style="font-weight: 700; color: yellow;">1. Localização e tipo</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Região:</strong> Centro da galáxia</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistema:</strong>Sistema Coruscant</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Tipo de planeta:</strong> Planeta urbano</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Atmosfera:</strong> A atmosfera de Coruscant é composta principalmente por oxigênio e nitrogênio, sendo compatível com a vida humana e diversas outras espécies. No entanto, devido à imensa urbanização, a qualidade do ar é prejudicada pela poluição das incontáveis indústrias e transportes, embora o sistema de purificação de ar seja eficiente.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">2. Clima e Ambiente</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Clima:</strong> Coruscant tem um clima temperado e relativamente estável, com a temperatura controlada artificialmente em muitas áreas. A enorme urbanização e os sistemas tecnológicos avançados permitem que o clima seja ajustado para conforto humano. Entretanto, a poluição e o calor gerado pela constante atividade industrial podem resultar em variações climáticas locais.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">3. Geografia e Terreno</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Cidade-Planeta:</strong> Coruscant é um planeta completamente coberto por uma imensa cidade que ocupa toda a sua superfície. Ao longo dos milênios, as áreas naturais foram progressivamente substituídas por arranha-céus, edifícios e complexos urbanos, com camadas que se estendem até as profundezas do planeta. Não há mais florestas, oceanos ou desertos naturais em Coruscant.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">4. Ecossistema e Vida Selvagem</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Espécies Nativas:</strong> Coruscant não possui muitas espécies nativas devido à total urbanização. As formas de vida nativas foram, em grande parte, substituídas por animais e plantas trazidas de outros planetas. Algumas espécies adaptadas à vida em ambientes urbanos, como aves exóticas e roedores, podem ser encontradas em áreas mais remotas da cidade.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Flora:</strong> O ecossistema de Coruscant foi drasticamente modificado pela urbanização. A vegetação natural praticamente desapareceu, sendo substituída por áreas verdes artificiais, como jardins em telhados e parques urbanos. Algumas plantas são cultivadas em estufas para fornecer recursos naturais para os habitantes da cidade, mas a vegetação original não existe mais.</li>
      </v-card-text>

      <v-card-actions>
        <v-spacer></v-spacer>

        <v-btn
          text="Fechar"
          @click="isActive.value = false"
        ></v-btn>
      </v-card-actions>
    </v-card>
  </template>
</v-dialog>

            </v-card-actions>
          </v-card>
        </v-col>
  
  
        <v-col cols="12" sm="6" md="4" lg="3">
            <v-card class="card-fixed-size d-flex flex-column">
            <v-img
              class="align-end text-white" id="image"
              src="https://swrpggm.com/wp-content/uploads/2024/06/Ahch-To_FE.jpg"
            >
            </v-img>
            <v-card-subtitle class="pt-3">Ahch-to</v-card-subtitle>
            <v-card-text>
              <div>
                Ahch-To é um planeta oceânico com diversas ilhas rochosas, cercadas por águas azuis e profundas. 
                A paisagem é marcada por montanhas escarpadas, praias e uma vegetação exuberante. 
                O clima é geralmente úmido, refletindo seu ambiente costeiro.
              </div>
            </v-card-text>
  
            <v-card-actions>
              <v-dialog max-width="500">
  <template v-slot:activator="{props:activatorProps}">
    <v-btn
      v-bind="activatorProps"
      color="surface-variant"
      text="VER MAIS"
      variant="flat"
    ></v-btn>
  </template>

  <template v-slot:default="{ isActive }">
    <v-card title="Ahch-to">
      <v-card-text>
        <p style="font-weight: 700; color: yellow;">1. Localização e tipo</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Região:</strong> Região Oeste da galáxia</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistema:</strong>Sistema Ahch-to</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Tipo de planeta:</strong> Planeta isolado e místico</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Atmosfera:</strong> A atmosfera de Ahch-To é respirável para muitas formas de vida, composta principalmente por oxigênio e nitrogênio, com uma mistura equilibrada de gases. Embora o clima seja agradável, a umidade constante e a proximidade do oceano fazem com que o ar seja denso e um pouco pesado em algumas áreas. O planeta tem um ambiente calmo e natural, com pouca poluição.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">2. Clima e Ambiente</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Clima:</strong> Ahch-To tem um clima temperado e subtropical, com altas taxas de umidade e chuvas frequentes, criando uma paisagem exuberante. O planeta é caracterizado por suas ilhas rochosas e vastos oceanos, com brisas suaves e um ambiente muito mais ameno comparado a outros planetas mais áridos da galáxia. Tempestades são comuns em algumas partes, mas em geral, o clima é tranquilo e sereno.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistemas Solares:</strong> Ahch-To orbita uma única estrela, sendo um planeta mais distante do centro galáctico. Sua principal característica climática é o ambiente isolado, sem grandes interferências externas. Sua tranquilidade e beleza natural tornam-no um lugar de retiro para aqueles que buscam paz e meditação.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">3. Geografia e Terreno</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Ilhas e Oceano:</strong> Ahch-To é composto principalmente por vastas ilhas rochosas e oceano profundo, com grandes falésias e penínsulas que se projetam para o mar. As ilhas são cobertas por vegetação tropical e densa, com muitas cavernas e áreas protegidas que servem como habitat para diversas espécies nativas.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Ruínas Jedi:</strong> O planeta é famoso pelas antigas Ruínas Jedi, que estão espalhadas pelas ilhas. Essas ruínas são locais sagrados, com templos e bibliotecas escondidos entre montanhas e florestas, e são uma das principais atrações do planeta. O Templo Jedi em Ahch-To é considerado um dos mais antigos e importantes locais para os praticantes da Força.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">4. Ecossistema e Vida Selvagem</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Espécies Nativas:</strong> Ahch-To abriga várias espécies únicas, incluindo os Porgs, aves pequenas e fofas que habitam as ilhas, além dos Caretakers, uma espécie nativa de habitantes que cuidam dos templos e mantêm uma vida simples e tranquila. O planeta também possui outros animais e aves marinhas que se adaptaram bem ao clima úmido e ao ambiente isolado.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Flora:</strong> A vegetação em Ahch-To é bastante variada, com florestas tropicais e densas, além de grandes árvores antigas que formam uma parte importante da paisagem do planeta. As plantas são robustas e adaptadas à umidade constante e ao solo rico em nutrientes. Existem também muitas plantas medicinais e outros tipos de flora que podem ser encontrados ao longo das praias e nas cavernas do planeta.</li>
      </v-card-text>

      <v-card-actions>
        <v-spacer></v-spacer>

        <v-btn
          text="Fechar"
          @click="isActive.value = false"
        ></v-btn>
      </v-card-actions>
    </v-card>
  </template>
</v-dialog>
            </v-card-actions>
          </v-card>
        </v-col>
        <v-col cols="12" sm="6" md="4" lg="3">
            <v-card class="card-fixed-size d-flex flex-column">
            <v-img
              class="align-end text-white" id="image"
              src="https://castwars.com/wp-content/uploads/2013/02/Geonosis-1-.jpg"
            >
            </v-img>
            <v-card-subtitle class="pt-3">Geonosis</v-card-subtitle>
            <v-card-text>
              <div>
                Geonosis é um planeta árido e rochoso, caracterizado por vastas planícies desérticas, formações rochosas imponentes e cavernas subterrâneas. 
                O clima é seco e quente, com pouca vegetação, o que torna o ambiente hostil para a vida.
                Geonosis é famoso por sua produção de droides e armas, especialmente durante as Guerras Clônicas. 
                As fábricas subterrâneas de Geonosis foram utilizadas para criar droides para o exército separatista.
              </div>
            </v-card-text>
            <v-card-actions>
              <v-dialog max-width="500">
  <template v-slot:activator="{props:activatorProps}">
    <v-btn
      v-bind="activatorProps"
      color="surface-variant"
      text="VER MAIS"
      variant="flat"
    ></v-btn>
  </template>

  <template v-slot:default="{ isActive }">
    <v-card title="Geonosis">
      <v-card-text>
        <p style="font-weight: 700; color: yellow;">1. Localização e tipo</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Região:</strong> Periferia da galáxia</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistema:</strong>Sistema Geonosis</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Tipo de planeta:</strong> Planeta desértico e rochoso</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Atmosfera:</strong> A atmosfera de Geonosis é composta principalmente por dióxido de carbono, o que torna o ar impróprio para a maioria das espécies, exceto para aquelas adaptadas a condições extremas. A atmosfera também contém grandes quantidades de poeira e areia devido ao clima árido, o que contribui para a aridez do planeta.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">2. Clima e Ambiente</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Clima:</strong> Geonosis é um planeta árido e desértico, com temperaturas extremamente altas durante o dia e frias à noite. O clima é marcado por vastos desertos, planícies de areia e dunas, além de tempestades de areia que são comuns. A pouca vegetação e a grande quantidade de rochas fazem o planeta parecer um deserto inóspito e implacável.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistemas Solares:</strong> Geonosis orbita um único sol, e sua principal característica climática é a escassez de água e a intensidade de calor. A exposição constante ao sol cria uma atmosfera hostil e difícil para muitas formas de vida que não são adaptadas ao calor extremo.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">3. Geografia e Terreno</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Desertos e Cavernas:</strong> Geonosis é dominado por vastos desertos e áreas rochosas. O terreno é árido e marcado por formações rochosas espetaculares, como penhascos e montanhas que se erguem das vastas planícies. A maior parte da vida em Geonosis se concentra em cavernas subterrâneas e estruturas debaixo da terra, onde temperaturas mais amenas podem ser encontradas.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Colonias e Fábricas:</strong> O planeta é famoso por suas grandes fábricas e instalações subterrâneas, usadas pelos Geonosianos, nativos do planeta, para fabricar droides de batalha e outras tecnologias militares. Essas fábricas estão localizadas em cavernas e regiões montanhosas, longe da vista de forasteiros, tornando Geonosis um lugar estratégico para os Confederados de Sistemas Independentes durante as Guerras Clônicas.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">4. Ecossistema e Vida Selvagem</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Espécies Nativas:</strong> Geonosis é habitado pelos Geonosianos, uma espécie insectoide altamente inteligente e com uma sociedade avançada em engenharia e construção. Os Geonosianos vivem em grandes colônias subterrâneas e têm uma grande habilidade para a construção de tecnologia militar e droides. Além deles, o planeta também abriga várias outras espécies adaptadas ao calor extremo, como criaturas subterrâneas e insetos gigantes.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Flora:</strong> A vegetação em Geonosis é praticamente inexistente devido ao clima desértico, mas em algumas regiões mais isoladas podem ser encontrados pequenos arbustos e plantas xerófitas, adaptadas para sobreviver com pouca água. A maior parte da fauna, no entanto, depende de fontes de água subterrâneas e de formas de vida adaptadas às cavernas.</li>
      </v-card-text>

      <v-card-actions>
        <v-btn
          text="Fechar"
          @click="isActive.value = false"
        ></v-btn>
      </v-card-actions>
    </v-card>
  </template>
</v-dialog>
            </v-card-actions>
          </v-card>
        </v-col>
  
        <v-col cols="12" sm="6" md="4" lg="3">
            <v-card class="card-fixed-size d-flex flex-column">
            <v-img
              class="align-end text-white" id="image"
              src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSJOlrC0x1Y5s_88RiMSMW-BNjq3fXEwZoUhg&s"> </v-img>
            <v-card-subtitle class="pt-3">Dagobah</v-card-subtitle>
            <v-card-text>
              <div>
                Dagobah é um planeta pantanoso e denso em vegetação, coberto por pântanos, árvores grandes e uma vasta variedade de fauna. 
                O clima é úmido e quente, com uma atmosfera rica em vida, mas também envolta em névoas e trevas, o que o torna um lugar isolado e misterioso.
                O planeta não possui habitantes nativos significativos, mas é habitado por várias criaturas, como crocodilos Dagobah e outros seres que se adaptaram ao ambiente pantanoso. 
                Yoda vive em um pequeno abrigo em uma árvore, onde se esconde da perseguição do Império.
              </div>
            </v-card-text>

            <v-card-actions>
              <v-dialog max-width="500">
  <template v-slot:activator="{props:activatorProps}">
    <v-btn
      v-bind="activatorProps"
      color="surface-variant"
      text="VER MAIS"
      variant="flat"
    ></v-btn>
  </template>

  <template v-slot:default="{ isActive }">
    <v-card title="Dagobah">
      <v-card-text>
        <p style="font-weight: 700; color: yellow;">1. Localização e tipo</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Região:</strong> Periferia da galáxia</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistema:</strong>Sistema Dagobah</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Tipo de planeta:</strong> Planeta pantanoso e isolado</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Atmosfera:</strong> A atmosfera de Dagobah é rica em oxigênio, tornando-a respirável para as formas de vida comuns. No entanto, a alta umidade e as grandes quantidades de neblina e gases de pântano podem tornar o ar pesado e desconfortável para quem não está acostumado com esse ambiente úmido e pantanoso. As tempestades são comuns, o que contribui para um clima instável e imprevisível.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">2. Clima e Ambiente</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Clima:</strong> O clima de Dagobah é caracterizado por uma alta umidade e temperaturas amenas, mas abafadas. A maior parte do planeta é coberta por pântanos, pântanos densos e florestas que criam um ambiente sombrio e misterioso. O clima instável e as frequentes chuvas contribuem para o crescimento abundante de plantas e vegetação. Além disso, o planeta é frequentemente envolto em uma espessa neblina, dificultando a visibilidade e criando uma sensação de isolamento.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistemas Solares:</strong> Dagobah orbita um único sol, mas sua localização remota e sua vegetação densa significam que a luz solar não penetra facilmente nas áreas de pântano mais densas, resultando em uma atmosfera sombria e misteriosa. O planeta tem uma pouca atividade externa, o que o torna um lugar isolado e sem grande interferência de outras forças galácticas.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">3. Geografia e Terreno</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Pântanos e Florestas:</strong> O terreno de Dagobah é dominado por vastos pântanos, áreas alagadas e florestas densas de vegetação tropical. O planeta é coberto por árvores de grande porte, arbustos e musgos que criam um ambiente quase impenetrável em algumas regiões. Existem também áreas pantanosas de águas turvas, cobertas por lama e vegetação aquática, tornando a locomoção difícil em muitas partes do planeta.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Lago e Cavernas:</strong> Entre as características geográficas de Dagobah estão vários lagos e corpos d'água, muitas vezes ocultos por densas camadas de vegetação. O planeta é também famoso por suas cavernas misteriosas e regiões isoladas, como a famosa Caverna da Força, que tem uma grande conexão com a Força, sendo um local importante para os Jedi.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">4. Ecossistema e Vida Selvagem</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Espécies Nativas:</strong> A vida selvagem de Dagobah é adaptada ao seu ambiente úmido e pantanoso. Embora o planeta não seja densamente povoado por espécies inteligentes, ele abriga uma grande diversidade de fauna. Entre as espécies nativas estão grandes serpentes, lagartos gigantes, e várias formas de criaturas aquáticas, incluindo sapos gigantes e insetos. A fauna tende a ser muito adaptada a ambientes úmidos e venenosos.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Flora:</strong> A vegetação de Dagobah é densa e bastante variada, com árvores altas, arbustos espessos e plantas aquáticas em abundância. Muitas dessas plantas possuem uma aparência exótica e são altamente adaptadas ao ambiente pantanoso. A vegetação de Dagobah é uma mistura de espécies tropicais e outras mais resistentes, que sobrevivem nas condições úmidas e alagadas do planeta.</li>
      </v-card-text>

      <v-card-actions>
        <v-btn
          text="Fechar"
          @click="isActive.value = false"
        ></v-btn>
      </v-card-actions>
    </v-card>
  </template>
</v-dialog>
            </v-card-actions>
          </v-card>
        </v-col>
  
        <v-col cols="12" sm="6" md="4" lg="3">
            <v-card class="card-fixed-size d-flex flex-column">
            <v-img
              class="align-end text-white" id="image"
              src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQvNpdlsWnAEdtYLuieJVsNUE339uOy5VHttQ&s"> </v-img>
            <v-card-subtitle class="pt-3">Endor</v-card-subtitle>
            <v-card-text>
              <div>
                Endor é um planeta florestal, coberto por densas florestas de árvores altas e exuberantes, com uma fauna diversificada. 
                O clima é geralmente temperado, proporcionando um ambiente favorável para a vida.
                A espécie mais notável de Endor são os Ewoks, pequenas criaturas bípedes que vivem em tribos e constroem suas casas nas árvores. 
                Eles são conhecidos por sua natureza curiosa, habilidades de sobrevivência e guerreiros formidáveis, apesar de sua estatura pequena.
              </div>
            </v-card-text>
            <v-spacer></v-spacer>
            <v-card-actions>
              <v-dialog max-width="500">
  <template v-slot:activator="{props:activatorProps}">
    <v-btn
      v-bind="activatorProps"
      color="surface-variant"
      text="VER MAIS"
      variant="flat"
    ></v-btn>
  </template>

  <template v-slot:default="{ isActive }">
    <v-card title="Endor">
      <v-card-text>
        <p style="font-weight: 700; color: yellow;">1. Localização e tipo</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Região:</strong> Borda Exterior</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistema:</strong>Sistema Endor</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Tipo de planeta:</strong> Planeta florestal</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Atmosfera:</strong> A atmosfera de Endor é composta principalmente por oxigênio e nitrogênio, tornando-a perfeitamente respirável para seres humanos e muitas outras espécies. A qualidade do ar é muito boa, com um clima ameno e condições favoráveis à vida. O planeta é coberto em grande parte por florestas densas e vegetação abundante, e possui uma atmosfera relativamente tranquila, sem grandes variações climáticas extremas.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">2. Clima e Ambiente</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Clima:</strong> O clima de Endor é temperado, com verões moderadamente quentes e invernos suaves. A maior parte do planeta é coberta por florestas densas, com uma grande variedade de fauna e flora nativas. O ambiente é bastante natural, com pouca influência de civilizações avançadas, embora as florestas sejam frequentemente envoltas por neblinas e nuvens que criam uma atmosfera misteriosa e mágica. Durante o dia, o clima tende a ser agradável, mas as noites podem ser frescas.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Sistemas Solares:</strong> Endor também possui áreas montanhosas esparsas, que se elevam suavemente a partir das florestas. Além disso, o planeta tem diversos lagos e corpos de água doce, que são vitais para o ecossistema local. O terreno, embora predominantemente florestal, inclui várias áreas de prados e clareiras.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">3. Geografia e Terreno</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Florestas:</strong> O terreno de Endor é principalmente coberto por vastas florestas de árvores grandes e antigas, como os árvores de Endor, que são conhecidas por sua imponência e tamanho. As florestas são densas e formam um ambiente fechado, onde as luzes solares têm dificuldades para penetrar, criando uma paisagem escura e mística no sub-bosque. As árvores abrigam uma grande variedade de vida selvagem e, em algumas áreas, formam passagens naturais através do terreno.</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Montanhas e Lagos:</strong> Entre as características geográficas de Dagobah estão vários lagos e corpos d'água, muitas vezes ocultos por densas camadas de vegetação. O planeta é também famoso por suas cavernas misteriosas e regiões isoladas, como a famosa Caverna da Força, que tem uma grande conexão com a Força, sendo um local importante para os Jedi.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">4. Ecossistema e Vida Selvagem</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Espécies Nativas:</strong> Endor é mais conhecida por ser o lar dos Ewoks, uma espécie de pequenas criaturas peludas, semelhantes a ursinhos, com uma cultura tribal e uma inteligência notável para a construção de abrigos e o uso de ferramentas rudimentares. Os Ewoks vivem em grandes árvores e têm uma forte ligação com a natureza. Eles são conhecidos por sua bravura e desempenham um papel central na Batalha de Endor, ajudando os Rebeldes a derrotar o Império Galáctico. Além dos Ewoks, Endor é lar de uma diversidade de criaturas selvagens, incluindo carnívoros e herbívoros adaptados às florestas densas e montanhosas.</li>
      </v-card-text>

      <v-card-actions>
        <v-btn
          text="Fechar"
          @click="isActive.value = false"
        ></v-btn>
      </v-card-actions>
    </v-card>
  </template>
</v-dialog>
            </v-card-actions>
          </v-card>
        </v-col>

        <v-col cols="12" sm="6" md="4" lg="3">
            <v-card class="card-fixed-size d-flex flex-column">
            <v-img
              class="align-end text-white" id="image"
              src="https://classic.exame.com/wp-content/uploads/2016/09/size_960_16_9_estrela_da_morte2.jpg?quality=70&strip=info&w=960"
            >
            </v-img>
            <v-card-subtitle class="pt-3">Estrela da morte</v-card-subtitle>
            <v-card-text class="flex-grow-1">
              <div>
                A Estrela da Morte é uma imensa estação espacial esférica, com um diâmetro que varia dependendo da versão. A primeira versão possui cerca de 160 km de diâmetro, enquanto a segunda versão é ainda maior. 
                A estrutura é equipada com tecnologia avançada, incluindo um superlaser capaz de destruir planetas inteiros.
                Projetada como uma arma de destruição em massa, a Estrela da Morte serve como um símbolo do poder do Império Galáctico. O seu principal objetivo é intimidar e controlar sistemas estelares, mostrando a força do Império e dissuadindo qualquer resistência.
              </div>
            </v-card-text>
  
            <v-card-actions>
              <v-dialog max-width="500">
  <template v-slot:activator="{props:activatorProps}">
    <v-btn
      v-bind="activatorProps"
      color="surface-variant"
      text="VER MAIS"
      variant="flat"
    ></v-btn>
  </template>

  <template v-slot:default="{ isActive }">
    <v-card title="Estrela da morte">
      <v-card-text>
        <p style="font-weight: 700; color: yellow;">1. Localização e tipo</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Região:</strong> Conforme a localização do império galáctico</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Tipo de planeta:</strong> Não planeta, estação espacial, superarma</li>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">construção:</strong>  Estrela da Morte é uma estação espacial artificial de enormes dimensões, construída para servir como uma superarma capaz de destruir planetas inteiros com um único disparo de seu superlaser. Foi projetada e construída pelo Império Galáctico como parte de sua estratégia para manter o controle sobre a galáxia e eliminar a resistência rebelde.
          </li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">2. Clima e Ambiente</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Clima:</strong> Como uma estação espacial, a Estrela da Morte não tem um clima ou ambiente planetário tradicional. Ela é equipada com toda a infraestrutura necessária para abrigar suas forças imperiais, cientistas e engenheiros, mas o ambiente dentro da estação pode variar, com áreas de alta segurança, hangares, áreas de comando e até áreas de reclusão para prisioneiros. Sua superfície externa é fria e metálica, refletindo a natureza fria e impessoal da arma que representa.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">3. Geografia e Terreno</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Tamanho e estrutura:</strong> A Estrela da Morte tem uma aparência semelhante a uma gigantesca esfera com aproximadamente 160 km de diâmetro em sua versão mais famosa (a Primeira Estrela da Morte), e cerca de 200 km de diâmetro na Segunda Estrela da Morte. A estação possui vários níveis internos, incluindo áreas de comando, hangares para naves, câmaras de controle de superlaser, e instalações de defesa e produção de TIE Fighters. Ela também contém um sistema de alimentação e propulsão para se mover através do espaço.</li><br>
        <v-spacer></v-spacer>
        <p style="font-weight: 700; color: yellow;">4. Ecossistema e Vida Selvagem</p>
          <li style="font-weight: 500;"><strong class="font-weight text-yellow">Vida a bordo:</strong> Embora a Estrela da Morte seja principalmente uma base militar e de construção, ela abriga uma variedade de seres humanos e droides. Ela contém uma grande frota de soldados imperiais, cientistas, engenheiros, técnicos e pessoal de apoio, todos dedicados a manter a operação da estação e sua função de destruição planetária. Não há vida selvagem nativa ou ecossistemas naturais na Estrela da Morte. Sua estrutura é impessoal, fria e funcional, refletindo a natureza de uma arma de destruição em massa.</li>
      </v-card-text>

      <v-card-actions>
        <v-btn
          text="Fechar"
          @click="isActive.value = false"
        ></v-btn>
      </v-card-actions>
    </v-card>
  </template>
</v-dialog>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </div>
  </template>

<style scoped>
      #image {
        height: 200px;
        width: 100%;
        object-fit: ontain;
      } 

      .card-fixed-size{
        height: 700px;
      }
</style>