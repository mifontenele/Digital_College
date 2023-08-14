# Como utilizar o Leaflet

## Preparando sua página

### Antes de escrever qualquer código para o mapa, você precisa fazer as seguintes etapas de preparação em sua página:

    * Inclua o arquivo CSS do folheto na seção de cabeçalho do seu documento:

        #### "<link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
   integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY="
   crossorigin=""/>"

    * Incluir o arquivo Leaflet JavaScript após o CSS do Leaflet:

        #### "<script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
   integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo="
   crossorigin=""></script>"

    * Coloque um divelemento com um determinado idlocal onde você deseja que seu mapa esteja:

        #### "<div id="map"></div>"

    * Certifique-se de que o contêiner do mapa tenha uma altura definida, por exemplo, definindo-a em CSS:

        #### "#map { height: 180px; }"

Agora você está pronto para inicializar o mapa e fazer algumas coisas com ele.

## Configurando o mapa

### Vamos criar um mapa do centro de Londres.

    * Inicializar o mapa e definir sua visualização para as coordenadas geográficas escolhidas e um nível de zoom:

        #### "var map = L.map('map').setView([51.505, -0.09], 13);"
        