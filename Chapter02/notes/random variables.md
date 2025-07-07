# Variável Aleatória em Imagens de Satélite

Em sensoriamento remoto, uma **variável aleatória** pode ser considerada o valor de um pixel em uma imagem de satélite. Esse valor é frequentemente chamado de Número Digital (DN - *Digital Number*).

### Exemplo

1.  **Imagem como uma Matriz:** Uma imagem de satélite é uma matriz (ou grade) de pixels.
2.  **Valor do Pixel (DN):** Cada pixel possui um valor numérico que representa a intensidade da radiação eletromagnética (luz) captada pelo sensor para uma determinada área na superfície terrestre.
3.  **Natureza Aleatória:** O valor de um pixel escolhido ao acaso na imagem não é determinístico. Ele é o resultado de um processo de medição influenciado por diversos fatores, como:
    *   O tipo de alvo na superfície (água, vegetação, solo, cidade).
    *   Condições atmosféricas (nuvens, aerossóis).
    *   Geometria de aquisição (ângulo do sol e do sensor).
    *   Ruído instrumental do sensor.

Por tratarmos o valor do pixel como uma variável aleatória, podemos usar a estatística para descrever e analisar as imagens. Por exemplo, podemos calcular a média, a variância e o histograma dos valores dos pixels para uma determinada classe (como "floresta") e usar essas informações para classificar a imagem inteira.