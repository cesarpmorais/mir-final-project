# Projeto MIR Final - Análise de Covers com DTW e Mapa de Constelações

Este trabalho investiga métodos para a identificação de covers musicais utilizando mapas de constelação e DTW (Dynamic Time Warping) aberto, realizando uma análise comparativa das duas abordagens.

### Informações do Grupo
  
  Cesar de Paula  / cesarpmorais@hotmail.com  
  Filipe Pirola Santos  / filipepirolasantos@hotmail.com  
  Julia Paes de Viterbo  / juliapaesv@gmail.com
  
## Estrutura do Projeto

- **LICENSE**  
  Arquivo contendo a licença do projeto.

- **README.md**  
  Este arquivo, que documenta o projeto e explica como utilizá-lo.

- **dtw_analysis.ipynb**  
  Notebook que contém a análise dos dados gerados pelo DTW. Nele são apresentados gráficos comparativos, métricas de desempenho e a otimização do threshold utilizado para a classificação dos covers (baseado na maximização do F1-score).

- **dtw_code.ipynb**  
  Notebook que contém a obtenção dos dados usando o algoritmo DTW. Os valores calculados aqui, são salvos no arquivo dtw_results.json no final.
  
- **dtw_results.json**  
  Arquivo JSON que armazena os resultados da análise DTW, ou seja, os valores de distância entre as faixas.

- **mir_final_project.ipynb**  
  Notebook que realiza o tratamento inicial dos dados. Este notebook gera os mapas de constelação e os cromagramas das músicas, que são posteriormente utilizados na análise com DTW.

- **songs_labels.json**  
  Arquivo JSON que contém as informações das músicas e os respectivos covers (ground truth), utilizado para validar os resultados da análise.

## Dados Adicionais

Além dos dados processados e analisados no projeto, também disponibilizamos um drive contendo as transformadas de Fourier das músicas e covers. Esses dados podem ser úteis para outras análises e são usados para o cálculo tanto do mapa de constelação, como para o DTW no nosso projeto.

- [Link do drive](https://drive.google.com/drive/folders/1-3pryJxQQ0vU-E4AYu_37qC6-tl44M-h?usp=sharing)

## Requisitos

Para executar os notebooks, certifique-se de ter instalado os seguintes pacotes:

- Python 3.x
- [librosa](https://librosa.org/)
- [fastdtw](https://github.com/slaypni/fastdtw)
- [numpy](https://numpy.org/)
- [pandas](https://pandas.pydata.org/)
- [matplotlib](https://matplotlib.org/)
- [seaborn](https://seaborn.pydata.org/)
- [scikit-learn](https://scikit-learn.org/)

Você pode instalar todas as dependências utilizando o `pip`:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn librosa fastdtw
```

## Licença

Este projeto está licenciado sob os termos descritos no arquivo [LICENSE](./LICENSE).
