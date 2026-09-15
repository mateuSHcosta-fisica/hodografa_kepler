#  Hodógrafa de Hamilton: Laboratório Virtual para Mecânica Orbital

[![Open In Colab][(https://colab.research.google.com/assets/colab-badge.svg](https://colab.research.google.com/drive/1zXxVV2EYAurAkbrpkszD0RScOSWrhPNj#scrollTo=uNUTpi_NbScd))]
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXXX)

Este repositório contém o material suplementar e os códigos-fonte das simulações interativas descritas no artigo **"A Hodógrafa de Hamilton como Ferramenta Didática para o Ensino de Mecânica Orbital e Analítica"** (submetido à *Revista Brasileira de Ensino de Física - RBEF*).

O objetivo deste projeto é fornecer uma ferramenta baseada na **Teoria das Múltiplas Representações**, permitindo que estudantes e professores explorem o Problema de Kepler de forma dinâmica, transitando fluidamente entre o Espaço de Posições (órbita física) e o Espaço de Velocidades (Hodógrafa).

---

## O que você encontrará neste laboratório?

O repositório disponibiliza simulações interativas desenvolvidas em Python (via Jupyter Notebook / Google Colab), divididas em duas abordagens pedagógicas:

1. **A Geometria da Órbita (Simulação Estática/Interativa):**
   - O usuário controla as velocidades absidais: no periastro ($v_p$) e no apoastro ($v_a$).
   - A simulação calcula instantaneamente o raio da hodógrafa ($R_h$), o deslocamento do seu centro ($d$) e a excentricidade ($e$).
   - Visualização em painel duplo mostrando que, independentemente da excentricidade geométrica da órbita, a trajetória da velocidade é sempre um círculo sob uma força central do tipo inverso-quadrática.

2. **A Evolução Cinética (Simulação Animada):**
   - Resolve a Equação de Kepler por métodos numéricos (Newton-Raphson) para avançar a órbita no "tempo real" da física.
   - Demonstra a Segunda Lei de Kepler (Lei das Áreas) revelando que o vetor velocidade não percorre a hodógrafa de forma uniforme, acelerando no periastro e retardando no apoastro.

---

## Como Executar as Simulações

A maneira mais rápida e recomendada para uso em sala de aula é através do **Google Colab**, pois não requer nenhuma instalação local.

### Opção A: Execução via Google Colab (Recomendado)
1. Clique no botão **Open in Colab** no topo desta página.
2. Com o notebook aberto, vá no menu superior e clique em `Ambiente de Execução > Executar Tudo` (ou `Runtime > Run All`).
3. Uma mensagem de alerta do Google pode aparecer. Clique em "Executar assim mesmo".
4. Utilize os controles deslizantes (*sliders*) gerados abaixo das células de código para interagir com a física do sistema.

### Opção B: Execução Local (Jupyter Notebook)
Para executar o laboratório na sua própria máquina, você precisará ter o Python instalado com as seguintes dependências:
```bash
pip install numpy matplotlib plotly ipywidgets
