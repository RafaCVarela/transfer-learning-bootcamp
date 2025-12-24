# Projeto de Classificação de Imagens com Transfer Learning

Este projeto Google Colab demonstra o poder do Transfer Learning para tarefas de classificação de imagens. Ele aproveita modelos de deep learning pré-treinados para alcançar alta precisão, mesmo com conjuntos de dados relativamente pequenos.

## Recursos:

*   **Transfer Learning/Fine-tuning**: Aprenda a usar modelos pré-treinados (especificamente VGG16 neste exemplo) como extratores de características ou para fine-tuning em um novo conjunto de dados.
*   **Integração de Dataset Personalizado**: Adapte facilmente o notebook para usar seus próprios conjuntos de dados de imagem. O notebook fornece orientação sobre como estruturar seus dados.
*   **Comparação de Abordagens**: Observe a melhoria significativa de desempenho de um modelo treinado com Transfer Learning em comparação com um modelo treinado do zero em um conjunto de dados limitado.
*   **Pronto para Google Colab**: Projetado para rodar perfeitamente no Google Colab, aproveitando seus recursos de GPU gratuitos.

## Como Usar:

1.  **Abrir no Colab**: Abra este notebook no Google Colab.
2.  **Preparar seu Dataset**:
    *   O notebook usa uma versão modificada do dataset Caltech-101 como exemplo.
    *   Se estiver usando seu próprio dataset, certifique-se de que ele esteja organizado em subpastas, com cada subpasta representando uma classe (ex: `meu_dataset/Dogs`, `meu_dataset/Cats`).
    *   Você pode carregar seu dataset para o Google Drive e montá-lo, ou carregá-lo diretamente para o ambiente do Colab.
3.  **Executar Células**: Execute as células do notebook sequencialmente.
    *   As células iniciais lidam com o carregamento de dados, pré-processamento e treinamento de um modelo de linha de base do zero.
    *   As células subsequentes demonstram a abordagem de Transfer Learning usando VGG16.
4.  **Analisar Resultados**: Compare a acurácia de validação e teste do modelo treinado do zero versus o modelo treinado com Transfer Learning.

## Estrutura do Projeto (após executar o notebook):

*   `meu_dataset/`: (Criado pelo notebook) Este diretório conterá seus dados de imagem, organizados por classe.
*   `README.md`: Este arquivo, fornecendo uma visão geral do projeto.
*   Gráficos de saída mostrando o histórico de treinamento e o desempenho do modelo.

## Dependências:

O projeto utiliza principalmente Keras (com backend TensorFlow) para construir e treinar as redes neurais, juntamente com bibliotecas Python padrão como NumPy e Matplotlib. Todas as bibliotecas necessárias estão disponíveis no ambiente Google Colab.

## Próximos Passos / Potenciais Melhorias:

*   **Aumento de Dados (Data Augmentation)**: Implementar técnicas de aumento de dados para melhorar ainda mais a generalização do modelo, especialmente com pequenos conjuntos de dados.
*   **Diferentes Arquiteturas**: Experimentar outros modelos pré-treinados (ex: ResNet, Inception) disponíveis no Keras Applications.
*   **Otimização de Hiperparâmetros**: Otimizar taxas de aprendizado, tamanhos de batch e outros hiperparâmetros para melhor desempenho.
*   **Fine-tuning de mais camadas**: Explorar o fine-tuning de mais camadas do modelo pré-treinado se seu conjunto de dados for grande e diversificado o suficiente.

## Feito por:

* Rafael Costa Varela
*  **email**: rafael.varela2220@gmail.com
