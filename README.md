# strabismus_detection_with_sam3

Este repositório foi organizado para apresentar **6 vídeos** de visualização do método proposto no artigo submetido para a *Discover Artificial Intelligence*:

- 3 pacientes com estrabismo diagnosticado
- 3 pacientes diagnosticados como ORTO (sem desvio ocular)

## Estrutura do repositório

```text
.
├── README.md
├── assets/
│   └── illustrations/
│       └── métodoproposto.png
└── videos_anonimizados_artigo/
    └── estrabismo/
        └── video_01_estrabismo.mp4
        └── video_01_estrabismo.mp4
        └── video_01_estrabismo.mp4
    └── orto/
        └── video_01_orto.mp4
        └── video_02_orto.mp4
        └── video_03_orto.mp4
```


## Descrição dos vídeos disponibilizados

Cada vídeo apresenta a realização do exame de **Cover Test Alternado**. Para preservar a anonimização dos pacientes, foi aplicado um **desfoque gaussiano** em toda a extensão dos vídeos. Além disso, foram adicionadas **bordas pretas nas regiões superior e inferior**, de modo a restringir a visualização às regiões de interesse, que compreendem os olhos e o objeto oclusor.

Durante a execução do método, as detecções são apresentadas visualmente sobre os vídeos da seguinte forma:

- **Região ocular:** representada por uma *bounding box* (caixa delimitadora) na cor vermelha.
- **Centroide da máscara gerada pelo modelo SAM3:** representado por um círculo azul.
- **Objeto oclusor:** representado por uma *bounding box* na cor verde.
- **Centroide do objeto oclusor:** representado por um ponto em tom de verde mais escuro.

Cada vídeo contém **cinco passagens do objeto oclusor sobre cada olho do paciente**, permitindo a visualização das detecções realizadas pelo método ao longo da execução do exame.

## Ilustração do método (futuro)

`/assets/illustrations/`
