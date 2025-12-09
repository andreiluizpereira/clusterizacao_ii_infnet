# Validação de modelos de clusterizaçã - INFNET

Projeto da Disciplina Validação de modelos de clusterizaçã - INFNET <br>
Professor: Gesiel Rios Lopes

## Requisitos
Python 3.13.7 ou superior

## Como baixar e executar o projeto no `Windows`
Clone o repositório para seu computador e acesse a pasta:
```powershell
git clone https://github.com/andreiluizpereira/clusterizacao_ii_infnet.git
cd clusterizacao_i_infnet
```

Crie um ambiente virtual:
```powershell
python -m venv .venv
```

Ative o ambiente virtual:
```powershell
.venv/Scripts/activate
```

Baixe as dependências do projeto:
```powershell
pip install -r requirements.txt
```

Executar o projeto no Jupyter:
```powershell
jupyter notebook pd.ipynb
```

Executar o projeto no VSCode:  
- Use o atalho **Ctrl + Shift + P** → digite **"Run All"** → selecione **"Notebook: Run All"**  
- Ou clique no botão **"Run All" (▶▶)** na barra superior do notebook  
- Ou use **Shift + Enter** para executar célula por célula  


# Instruções do projeto

Chegamos na hora de validar nosso conhecimento. As questões teóricas podem ser respondidas em slides ou doc em formato .PDF e devem ser disponibilizadas junto com o código (ver questão 6).

O trabalho está dividido em 4 partes, como você pode observar a seguir.

## Infraestrutura
Para as questões a seguir, você deverá executar códigos em um notebook Jupyter, rodando em ambiente local, certifique-se que:  

1. Você está rodando em Python 3.9+
2. Você está usando um ambiente virtual: Virtualenv ou Anaconda
3. Todas as bibliotecas usadas nesse exercícios estão instaladas em um ambiente virtual específico
4. Gere um arquivo de requerimentos (requirements.txt) com os pacotes necessários. É necessário se certificar que a versão do pacote está disponibilizada.
5. Tire um printscreen do ambiente que será usado rodando em sua máquina.
6. Disponibilize os códigos gerados, assim como os artefatos acessórios (requirements.txt) e instruções em um repositório GIT público. (se isso não for feito, o diretório com esses arquivos deverá ser enviado compactado no moodle).
Dica: Gere um relatório rico em gráficos que dêem respaldo aos resultados

## Escolha de base de dados
Para as questões a seguir, usaremos uma base de dados e faremos a análise exploratória dos dados, antes da clusterização.

1. Escolha uma base de dados para realizar o trabalho. Essa base será usada em um problema de clusterização.
2. Escreva a justificativa para a escolha de dados, dando sua motivação e objetivos.
3. Mostre através de gráficos a faixa dinâmica das variáveis que serão usadas nas tarefas de clusterização. Analise os resultados mostrados. O que deve ser feito com os dados antes da etapa de clusterização?
4. Realize o pré-processamento adequado dos dados. Descreva os passos necessários.  

## Clusterização
Para os dados pré-processados da etapa anterior você irá:

1. Realizar o agrupamento dos dados, escolhendo o número ótimo de clusters. Para tal, use o índice de silhueta e as técnicas:
a. K-Médias
b. DBScan
2. Com os resultados em mão, descreva o processo de mensuração do índice de silhueta. Mostre o gráfico e justifique o número de clusters escolhidos.
3. Compare os dois resultados, aponte as semelhanças e diferenças e interprete.
4. Escolha mais duas medidas de validação para comparar com o índice de silhueta e analise os resultados encontrados. Observe, para a escolha, medidas adequadas aos algoritmos.
5. Realizando a análise, responda: A silhueta é um o índice indicado para escolher o número de clusters para o algoritmo de DBScan?  

## Medidas de similaridade
1. Um determinado problema, apresenta 10 séries temporais distintas. Gostaríamos de agrupá-las em 3 grupos, de acordo com um critério de similaridade, baseado no valor máximo de correlação cruzada entre elas. Descreva em tópicos todos os passos necessários.
2. Para o problema da questão anterior, indique qual algoritmo de clusterização você usaria. Justifique.
3. Indique um caso de uso para essa solução projetada.
4. Sugira outra estratégia para medir a similaridade entre séries temporais. Descreva em tópicos os passos necessários.
