# LATAM-Challenge

# Funções de Análise de Tweets
Este repositório contém funções para analisar dados de tweets. As funções fornecem informações sobre datas com mais tweets, emojis mais usados e usuários mais mencionados.

# Instalação
Antes de começar, instale as dependências necessárias usando:

```pip install -r requirements.txt ```

## Funções
### 1. q1_time e q2_memory
Descrição: Retorna as 10 principais datas com mais tweets e o usuário com mais tweets em cada uma dessas datas.

#### Uso:

```from analysis_module import q1_time```

```result = q1_time("path_to_your_file.jsonl")```
#### Retorno:

```Returns: [(datetime.date(1999, 11, 15), "LATAM321"), (datetime.date(1999, 7, 15), "LATAM_CHI"), ...] ```

### 2. q2_time e q2_memory
Descrição: Retorna os 10 emojis mais usados nos tweets. A função q2_memory é otimizada para melhor uso da memória.

#### Uso:

```from analysis_module import q2_time```

```result = q2_time("path_to_your_file.jsonl")```

#### Retorno:

```Returns: [("✈", 6856), ("❤", 5876), ...]```

### 3. q3_time e q3_memory
Descrição: Retorna os 10 usuários históricos mais influentes (nome de usuário) com base na contagem de menções (@) que registram cada um deles.

#### Uso:

```from analysis_module import q3_time```

```result = q3_time("path_to_your_file.jsonl")```

#### Retorno:

```Returns: [("LATAM321", 387), ("LATAM_CHI", 129), ...]```
