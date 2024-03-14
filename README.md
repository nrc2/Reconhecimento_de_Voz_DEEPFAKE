# Reconhecimento_de_Voz_DEEPFAKE
Projeto da cadeira de Sinais e Sistemas do CIn UFPE - COnstrução e apresentação, a partir de sinais de áudio, um modelo para reconhecimento de voz DEEPFAKE.

## Introdução
A inteligência artificial generativa está redefinindo as fronteiras do possível, abrindo
novos horizontes para a comunicação humana. A capacidade de clonar e converter vozes em
tempo real não é apenas um testemunho do avanço tecnológico, mas também um campo minado
ético, repleto de potenciais violações de privacidade e a propagação de desinformação. A
emergência de declarações falsas, impulsionadas por vozes sintetizadas indistinguíveis das reais,
acendeu um alerta sobre a urgência de desenvolver mecanismos de detecção eficazes.
Nesse cenário, o conjunto de dados DEEP-VOICE servirá como base de dados para
o projeto inicial de combate a crescente ameaça das DeepFakes de voz. O DEEP-VOICE é
constituído por amostras de fala autêntica de oito personalidades notáveis, juntamente com suas
respectivas vozes transformadas por meio de técnicas avançadas de conversão de voz baseada
em recuperação. Esta compilação não só oferece uma plataforma para o aprimoramento e teste
de algoritmos de detecção de DeepFake de voz, mas também contribui para a compreensão mais
ampla das complexidades envolvidas na distinção entre fala real e sintetizada.

## Sobre o conjunto dados
Para cada amostra de fala incluída no DEEP-VOICE, um procedimento meticuloso foi
adotado para a remoção do ruído de fundo antes da execução da conversão de voz, seguido pela
reinserção do acompanhamento original no discurso DeepFake resultante. Esse processo garante
a integridade dos dados e facilita uma análise mais precisa, sublinhando o compromisso com a
qualidade e a aplicabilidade do conjunto de dados no desenvolvimento de soluções eficazes para
a detecção de falsificações de voz.
Existem dois formulários para o conjunto de dados que são disponibilizados:

Primeiro, o áudio bruto pode ser encontrado no diretório “AUDIO”. Eles estão organi-
zados nos diretórios de classes "REAL"e "FAKE". Os nomes dos arquivos de áudio indicam

quais alto-falantes forneceram a fala real e para quais vozes foram convertidos. Por exemplo,
"Obama-to-Biden"denota que o discurso de Barack Obama foi convertido para a voz de Joe
Biden.
Segundo, os recursos extraídos podem ser encontrados no arquivo "DATASET-balanced.csv".
Estes são os dados que foram utilizados no estudo abaixo. O conjunto de dados tem cada recurso
extraído de janelas de áudio de um segundo e é balanceado por meio de amostragem aleatória.
Todos os dados experimentais são encontrados no diretório "KAGGLE". O diretório
"DEMONSTRATION"é usado para reproduzir demos cortadas e compactadas em notebooks
devido às limitações do Kaggle no tamanho do arquivo.

## Acesso aos dados
Este conjunto de dados foi produzido a partir do estudo "Detecção em tempo real de fala
gerada por IA para conversão de voz DeepFake"
Bird, JJ e Lotfi, A., 2023. Detecção em tempo real de fala gerada por IA para
conversão de voz DeepFake. Pré-impressão do arXiv arXiv:2308.12734.
Este conjunto de dados pode ser encontrado aqui: [Base de Dados: DEEP-VOICE](https://www.kaggle.com/datasets/birdy654/deep-voice-deepfake-voice-recognition/data)
