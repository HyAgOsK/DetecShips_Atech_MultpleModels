# DetecShips_Atech_MultpleModels
Detecção de objetos para empresa ATECH, com modelos Mobilev2 ssd fpn lite 320x320, Yolov5n, EfficientDet0 e Fomo, destacando um relatório sobre o desempenho destes.

**Cada diretório contem o notebook e os resultados obtidos**

- Fomo no caso é de propriedade do edge impulse então o notebook contém informações sobre resutados obtidos e um txt contem o link do projeto do FOMO
- MobileNet SSD FPN LITE 320x320 contém o Notebook que é basicamente o passo a passo inteiro para executar tudo que foi feito, comentado, em inglês, algumas alterações foram necessárias serem feitas em códigos de outras pessoas para que funcione corretamente todo notebook, isto também está comentado
- Yolov5n também contém todo passo a passo para execução do modelo com os resultados e como foi obtido.
- EfficientDet0 também contém todo passo a passo para execução do modelo com resultados obtidos e o modelo tflite


> Observação: Até o momento o melhor modelo é o Yolov5n float32 ou float16, que obteve o melhor resultado
> 
> Foi feito um dashboard com Flask, todos as bibliotecas necessárias para implementação do dashboard estão em um arquivo txt, requirements.txt, algumas que derem problema podem ser instaladas manualmente sem o versionamento, basta instalar a versão mais recente.
- A base de dados vem do roboflow, basta exportar como jupyter que é gerado um link e assim conseguimos ter a base de dados no notebook colaboratory.
> https://universe.roboflow.com/hyago-vieira/detectionship

- As classes estão organizadas da seguinte maneira:
  
        "BACKGROUND": 0,
        "BULK-CARRIER": 1,
        "CONTAINER-SHIP": 2,
        "GENERAL-CARGO": 3,
        "OIL-PRODUCTS-TANKER": 4,
        "PASSENGERS-SHIP": 5,
        "TANKER": 6,
        "TRAWLER": 7,
        "TUG": 8,
        "VEHICLES-CARRIER": 9,
        "YACHT": 10
