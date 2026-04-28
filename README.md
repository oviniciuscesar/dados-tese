# Dados de pesquisa - doutorado

Este repositório agrega códigos-fonte, algoritmos, materiais de apoio e arquivos multimodais produzidos no contexto de uma pesquisa de doutorado sobre a apropriação crítica e criativa de técnicas de machine learning e machine listening voltadas à prática composicional de live-electronics. O material foi organizado para favorecer reprodutibilidade e exploração por compositores, performers, artistas e pesquisadores.

## Estrutura de diretorios (visao geral)

/
|-- 1-algoritmos/
| |-- dastgah_analysis/
| |-- mlperceptron/
| |-- pd-euclidiana/
| |-- pd-perceptron/
| |-- pd-som/
| `-- searchA-Star/
|-- 2-material-apoio/
|   `-- exemplos-cap3-tese/
`-- 3-materiais-composicionais/
    |-- EutrpoiaIII_2025/
    |-- LSTM_Spat_Trajectories/
    |-- PQMF/
    |-- gaitacol/
    `-- transformer/

## O que este repositório contém:

### 1) Ecossistema de algoritmos

- Objetos para Pure Data (linguagem C): implementações puras (sem dependencias externas) de algoritmos clássicos de aprendizado de maquina e redes neurais para composição em tempo real. Inclui perceptron, mlperceptron (redes neurais multicamadas totalmente conectadas), SOM (Mapas Auto-Organizaveis de Kohonen), searchA-Star (busca heurística em grafos) e objetos auxiliares como euclidiana.
- Ferramentas adicionais de acústica e análise: scripts em Python (dastgah_analysis) para análise computacional e musicologica, focada em perfil melódico e precisão de afinação da música tradicional persa. Algoritmos em C/C++ incluem arquivos CMakeLists.txt para reprodução em multiplas plataformas.

### 2) Material de apoio e exemplos matematicos

- Jupyter Notebooks: colecao de códigos interativos que demonstram operacoes matemáticas discutidas no Capítulo 3 da tese. Exemplos para Busca A\*, Adaline, modelo MCP, Perceptron e processos de Feedforward e Backpropagation em redes neurais profundas.

### 3) Materiais composicionais de Eutrópia III (2025)

- Modelos de redes neurais (Python/PyTorch): modelos usados no processo composicional de Eutrópia III, incluindo Transformer Conditional Variational Autoencoder (T-CVAE) para mapeamento de gestos/aticulações da flauta em parâmetros de síntese, LSTM para reconstrução de trajetorias espaciais em coordenadas polares e filtros Pseudo-Quadrature-Mirror-Filter (PQMF) para processamento em sub-bandas.
- Ferramentas adicionais: adaptação do objeto gaitacol~ para Pure Data, que modela computacionalmente as gaitas colombianas.
- Dados da composição: partitura (PDF), gravação referencial em audio espacializado (binaural) e patches em Pure Data para performance da eletrônica em tempo real.

## Notas importantes

- Este repositório é um agregador com submodulos Git. Para clonar todos os diretórios e submódulos de uma vez:

  git clone --recurse-submodules <https://github.com/oviniciuscesar/dados-tese.git>

- Para atualizar os submodulos:

  git submodule update --init --recursive
