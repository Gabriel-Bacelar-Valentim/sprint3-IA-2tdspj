# sprint3-IA-2tdspj

Integrantes:

Maria Luiza de Oliveira Lobo - 552169

Gabriel Bacelar Valentim - 97901

Luana Duque - 550813

Leonardo Shoiti Araki - 98587

1. Camadas Convolucionais
   
No meu modelo, que eu carreguei no Google Colab, eu usei camadas convolucionais para extrair características das imagens. Essas camadas aplicam filtros para detectar padrões como bordas e texturas. Elas são fundamentais para processar a imagem e gerar mapas de características que são passados para as camadas seguintes.

2. Camadas de Pooling
   
Após as camadas convolucionais, eu adicionei camadas de pooling, como MaxPooling, para reduzir a resolução dos mapas de características. Isso ajuda a diminuir a complexidade do modelo e a prevenir o overfitting, preservando as características mais importantes enquanto reduz a dimensionalidade dos dados.

3. Camadas Densas
   
Depois do processamento pelas camadas convolucionais e de pooling, eu incluo camadas densas no meu modelo. Essas camadas totalmente conectadas combinam as características extraídas para fazer a previsão final. A camada densa final usa a função de ativação Softmax para gerar probabilidades para cada classe. Essa função é crucial para converter as saídas do modelo em uma distribuição de probabilidade, mostrando a confiança do modelo em cada classe.

4. Preparação e Execução
   
Com as funções load_model_from_h5 e load_class_names, eu carrego o modelo e os nomes das classes. A função prepare_image ajusta a imagem para o formato esperado pelo modelo, e a função classify_and_display_image usa o modelo para prever a classe da imagem e exibir o resultado. Essas funções dependem da arquitetura definida no arquivo .h5 que eu treinei anteriormente.

Por quê?

Escolhi essas arquiteturas porque as camadas convolucionais são ótimas para extrair características das imagens, as camadas de pooling reduzem a complexidade e evitam o overfitting, e as camadas densas combinam essas características para a classificação final usando Softmax. Essas escolhas garantem que o modelo seja eficiente e preciso na tarefa de classificação de imagens.
