<p align="center">
  <img title="a title" alt="Alt text" src="https://media.licdn.com/dms/image/D4E16AQGjCVuzlCthvg/profile-displaybackgroundimage-shrink_200_800/0/1690574706700?e=2147483647&v=beta&t=zlY1Mc10yQ3gA9qiZ4sZ7m8PkE-HIu8Haa1fUyKb_fU">
</p>

# Desafio Engenheiro de Dados | Pyspark

Olá, candidato! Se você chegou até aqui, é porque demonstrou interesse em fazer parte do nosso time. Preparamos um desafio para entendermos um pouco mais sobre suas habilidades como engenheiro de dados.

## 🚀 Objetivo:

Resolver as questões propostas para cada dataset disponibilizado com spark DataFrame.

## 📜 Requisitos:

### 1. Configuração Inicial:

- Configurar um ambiente Spark:

Você pode usar o código abaixo para simular um ambiente pyspark no Colab:
```
!apt-get install openjdk-8-jdk-headless -qq > /dev/null
!wget -q http://archive.apache.org/dist/spark/spark-3.1.1/spark-3.1.1-bin-hadoop3.2.tgz
!tar xf spark-3.1.1-bin-hadoop3.2.tgz
!pip install -q findspark

import os
os.environ["JAVA_HOME"] = "/usr/lib/jvm/java-8-openjdk-amd64"
os.environ["SPARK_HOME"] = "/content/spark-3.1.1-bin-hadoop3.2"

import findspark
findspark.init()
```

### 2. Download dos datasets:

Baixe os datasets no seu ambiente Colab:
- Dataset Ocupações: https://raw.githubusercontent.com/justmarkham/DAT8/master/data/u.user
- Dataset Carros 1: https://raw.githubusercontent.com/guipsamora/pandas_exercises/master/05_Merge/Auto_MPG/cars1.csv
- Dataset Carros 2: https://raw.githubusercontent.com/guipsamora/pandas_exercises/master/05_Merge/Auto_MPG/cars2.csv

### 3. Instruções de desenvolvimento:

- Com o dataset de Ocupações:
  - Mostre um resumo do dataset com contagem, média, desvio padrão, mínimo, máximo e os quartis para cada coluna.
  - Mostre somente a(s) idade(s) com menor ocorrência.
  - Mostre a média de idade por ocupação e a frequência dela no dataset.
  - Mostre a proporcão (em %) de homens e mulheres por ocupação. Faça o mesmo para o público masculino e feminino.

- Com o dataset de Carros (1 e 2):
  - Ajuste o dataset e faça o merge entre os dois.
  - Adicione uma coluna "Owners" que contenha o ID único de proprietários (gerado aleatoriamente entre 1 e 100).
  - Crie uma coluna "Custo-Benefício" que aplique o conceito a seguir:
    - Some o peso com a cilindrada dividida pela quantidade de cilindros.
    - Subtraia o valor acima pela aceleração multiplicada pela quantidade de cavalos.
   
- Não esqueça de salvar o DataFrame final.

### 4. Validações e Erros:

- Implemente validações para garantir a integridade dos dados.
- Inclua um log com mensagens de erro claras.

## 🗳️ Instruções de Submissão:

1. Faça o download do script com extensões .ipynp e .py.
2. Envie um e-mail para [alexandre.godoy@khipo.com.br] com os 2 arquivos e suas observações.

## 🧪 Avaliação:

- Estrutura do código e organização.
- Uso adequado das tecnologias.
- Implementação dos requisitos.
- Funcionalidades extras (diferenciais).

Boa sorte com o desafio! Estamos ansiosos para ver sua solução.
