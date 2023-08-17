# Leaflet
O Leaflet é a principal biblioteca JavaScript de código aberto para mapas interativos compatíveis com dispositivos móveis. Pesando apenas cerca de 42 KB de JS
## Quick Start
### 1. Antes de escrever o código para o mapa:
   #### Inclua o arquivo CSS do folheto na seção de cabeçalho do seu documento:
         <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" 
         integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>
   #### Inclua o arquivo Leaflet JavaScript após o CSS do Leaflet:
         <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" 
         crossorigin=""></script>"
   #### Coloque um elemento div com um idlocal onde você deseja que seu mapa esteja:
         <!-- criando a div e atribuindo o id "map" mas pode ser o id que quiser -->
         <div id="map">
         </div>
   #### Certifique-se de que o container do mapa tenha as configurações desejadas definidas no arquivo do CSS:
         /*  estilo que terá a div com o id map criado acima */
         #map { 
             padding: 20px;
             height: 600px;
             width: 900px;
             margin: auto;
             border: solid 1px black;
             }
### 2. Criando o mapa desejeado:
   #### Incluir um mapa usandi coordenadas centralizadas
         
   #### Inicialize o mapa e defina a visualização para as coordenadas geográficas escolhidas e um nível de zoom
         // Criando uma variável e chamando-a de "map". Depois atribuindo a longitude, latitude do local que desejamos centralizar e
         // também o nível de zoom através do "L.map(nome do já id criado com aspas simples) 
         var map = L.map('map').setView([51.505, -0.09], 13);
        
