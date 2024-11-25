# Redução de Dimensionalidade em Imagens para Redes Neurais

Este projeto demonstra como realizar a redução de dimensionalidade de imagens utilizando Python, convertendo imagens coloridas para tons de cinza e, em seguida, para uma versão binarizada. O foco é entender como essas transformações podem simplificar a representação de uma imagem, o que pode ser útil em diversas aplicações, como redes neurais e sistemas de visão computacional.

## Objetivo

O principal objetivo desse projeto é implementar, do zero, funções para:

1. **Converter imagens coloridas para tons de cinza**: Esta conversão é feita utilizando uma fórmula ponderada que leva em consideração a luminância (brilho) da imagem.
   
2. **Binarizar a imagem**: Transformar a imagem para uma versão com apenas duas cores (preto e branco), usando um limiar de intensidade. 

Essas transformações ajudam a reduzir a quantidade de informações que precisam ser processadas, mantendo o essencial para a análise.

## Funcionalidades

- **Conversão para Tons de Cinza**: A função `converter_para_cinza` transforma uma imagem colorida (RGB) para um formato de imagem com um único canal de intensidade.
  
- **Binarização de Imagem**: A função `binarizar_imagem` converte a imagem em tons de cinza para uma versão binária (preto e branco) com base em um valor de limiar.

- **Exibição das Imagens**: O projeto exibe as imagens processadas, mostrando a imagem original, a versão em tons de cinza e a versão binarizada.

## Pré-requisitos

Para executar este projeto, é necessário ter o Python 3 e as seguintes bibliotecas instaladas:

- **Pillow**: Para manipulação de imagens.
- **Google Colab** (se você for utilizar diretamente no ambiente de nuvem).

## Como usar

1. Clone este repositório:

```bash
git clone https://github.com/seu-usuario/repo-nome.git
cd repo-nome
```

2. Carregue a imagem de sua escolha ou utilize o caminho correto no Google Drive.

3. Execute o código para carregar a imagem e realizar as transformações:

```python
from PIL import Image

# Carregar a imagem
imagem_original = Image.open("caminho/da/imagem.jpg")

# Converter para tons de cinza
imagem_cinza = converter_para_cinza(imagem_original)

# Binarizar a imagem
imagem_binaria = binarizar_imagem(imagem_cinza)

# Exibir as imagens
imagem_original.show()
imagem_cinza.show()
imagem_binaria.show()
```

4. As imagens convertidas serão exibidas e salvas como arquivos de saída.

## Contribuição

Se você deseja contribuir com melhorias para este projeto, fique à vontade para abrir uma *issue* ou enviar um *pull request*.
