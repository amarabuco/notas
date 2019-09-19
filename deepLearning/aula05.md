### Aula 05 - Deep Learning

#### Redes Neurais Convolucionais (CNN)

redes baseadas em uma série de convoluções matemáticas

* campo receptivo: Ao invés da ligar pixels aos neurônios, a CNN trabalha de uma vez com um conjunto de pixels. é uma espécie de janela deslizante, que
inicia-se no começo da imagem e a percorre, capturando um conjunto de pixels diferente em cada percurso feito.

* convolução matemática com matrizes: consiste em uma operação matemática em que os elementos de uma matriz são multiplicados pelos elementos
de uma outra matriz (cada elemento é multiplicado pelo elemento correspondente da outra matriz), e as multiplicações são então somadas,

* feature map (ou mapa de características): resultado das convoluções dos campos receptivos de uma imagem produz uma outra matriz, menor que a original.

* camada de pooling: após cada camada convolucional uma camada especial para tornar as características das imagens invariantes à rotação e à translação

* função de ativação: as redes CNN utilizam uma função de ativação conhecida como ReLU

#### Redes Neurais Recorrentes

projetadas para realizar o processamento de informações que possuem uma sequência de acontecimentos e
que o resultado em um determinado ponto do tempo depende dos resultados nos tempos anteriores.

* Retropropagação Através do Tempo: ajuste de parâmetros baseado no algoritmo de retropropagação

#### Redes LSTM e GRU

* As redes LSTM introduziram o conceito conhecido como portão (gate, em inglês), que são estruturas que controlam o que fazer com determinada informação. 
1. portão do esquecimento (forget gate), que controla as informações que devem ser esquecidas; 
2. portão de entrada (input gate), indicando aquelas que devem entrar no fluxo de informações;
3. portão de saída (output gate), que indica quais informações devem ser propagadas. 

* Um tipo especial mais eficiente de LSTM são as redes do tipo GRU (do inglês, Gated Recurrent Unit).
1. portão de atualização (update gate), que indica quais informações passadas devem ser propagadas;
2. portão de reset (reset gate), que define quais informações passadas devem ser esquecidas.

#### Redes Neurais Recursivas

são utilizadas em problemas que apresentam algum tipo de hierarquia.

Uma aplicação em que redes recursivas apresentam bons resultados é o de processamento de linguagens naturais, que justamente tenta obter a semântica de uma frase ou sentença.

#### Redes GAN

A primeira classe de algoritmos (discriminativos) procura calcular a probabilidade do objeto pertencer a uma determinada classe, considerando que se conhece os dados X. Matematicamente, isso é representado por P(Y / X) (ou seja, a probabilidade de uma determinada classe dado o vetor de dados do objeto). Por outro lado, os algoritmos generativos buscam calcular o contrário: a probabilidade de um determinado vetor X, dado que se conhece a classe do objeto ( P(X /Y )).

Uma rede GAN possui duas redes neurais internamente, uma com caráter generativo e outra com caráter discriminativo. Basicamente, a rede se comporta como uma competição: a rede generativa tenta criar amostras falsas cada vez mais reais, enquanto a rede discriminativa tenta reconhecer essas amostras. 


