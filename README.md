# Painel 2022 COVID-19 - Informações sobre mortes e vacinação: Perfil por raça/cor.

### Autores: Natacha Stephany Sousa da Silva (nstephany1@gmail.com)
###         Raphael Caetano da Silva (raphael.bol@gmail.com)
###         Thammyres Valéria Batista Xavier Aragão (thammyresvaleria@hotmail.com)


Trabalho de Técnicas de Programação I - Let's Code from ADA. 
Programa Suzano <'Div'>ersidade Tech - 2022

Professor: Alex Lima 

Trabalho de Análise de Dados relacionado a COVID-19

Tema: Painel COVID-19 - Informações sobre mortes e vacinação: Perfil por raça/cor.

Análise de dados exploratória do DataSet do SIVEP-GRIPE, com o objetivo de evidenciar os perfis de mortalidade, infecção e vacinação até a última semana de 2022 verificada (Semana Epidemiológica 44).

Utilizar o Dataset do SIVEP-GRIPE
https://s3.sa-east-1.amazonaws.com/ckan.saude.gov.br/SRAG/2022/INFLUD22-14-11-2022.csv

Informações adicionais

Este projeto visa responder 3 questionamentos base: 
1) Qual o índice de mortalidade da COVID-19 para cada raça/cor no ano de 2022? 
2) Qual raça/cor mais infectada pela COVID-19 em 2022?
3) Qual raça/cor possui o maior índice de vacinação?

Para tanto, fez-se necesário algumas tratativas no Dataset do SIVEP-GRIPE, como a definição das colunas a serem utilizadas e o tratamento dos dados para análise.
No diretório de PDFs encontra-se o dicionário de Dados, o último Boletim Epidemiológico (que utilizamos como fonte de consulta apenas) e a ficha de preenchimento de SRAG.

As colunas que utilizamos para a nossa análise foram:

  DT_NOTIFIC - Data do preenchimento da ficha de notificação
  SEM_NOT - Semana Epidemiológica do preenchimento da ficha de notificação
  SG_UF_NOT - Unidade Federativa onde está localizada a Unidade Sentinela que realizou a notificação.
  CS_SEXO - Sexo do paciente.
  DT_NASC - Data de nascimento do paciente.
  NU_IDADE_N - Idade calculada após o preenchimento da DT_NASC, ou idade informada pelo paciente quando não se sabe a data de nascimento. Na falta desse dado é   registrada a idade aparente.
  CS_GESTANT - Idade gestacional da paciente.
  CS_RACA - Cor ou raça declarada pelo paciente:
  CS_ESCOL_N - Nível de escolaridade do paciente. Para os níveis fundamental e médio deve ser considerada a última série ou ano concluído.
  SG_UF - Unidade Federativa de residência do paciente.
  VACINA_COV - Informa se o paciente recebeu vacina COVID-19.
  MAE_VAC - Se paciente < 6 meses, a mãe recebeu vacina
  CLASSI_FIN - Diagnóstico final do caso
  EVOLUCAO - Evolução do caso

O tratamento dos dados foram variados, especificados caso à caso no Notebook, foram aplicadas as técnicas de programação para análise de dados para seleção de colunas, deleção de colunas, deleção de linhas inválidas, replace de valores, criação de novos dataframes, criação de gráficos e funções para automatizar alguns processos.
