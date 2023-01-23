# 📆 Extrator de Consultas - Livro Caixa

Esse Notebook tem como função extrair eventos do Google Calendar e salvá-los em um livro caixa em formato de arquivo Excel.

Nesse projeto é usado o Google Calendar API para extrair do calendário eventos com o nome dos pacientes, esses eventos são tratados e agrupados por recorrência e mês, e são exportados para o livro caixa.


A ideia desse projeto é facilitar a vida do excelente psicólogo [Jean Ghissoni](https://psicologojeanghissoni.negocio.site).


## Primeiros Passos

Para rodar o script basta rodar linha a linha desse notebook, excecutando em ordem cada etapa do código.

## Tabela de conteúdos:
1. [Configuração de ambiente](#setup)<br>
    1.1 [Instalando o Cliente Python do Google API](#setup1)<br>
    1.2 [Importando bibliotecas e métodos usandos no notebook](#setup2)<br>
    1.3 [Iniciando variáveis](#setup3)<br>
2. [Autenticando com a API do Google](#auth)<br>
    2.1 [Gerando o arquivo client_secrets.json](#auth1)<br>
    2.2 [Iniciando o Cliente do Google e Autorizando conta Google](#auth2)<br>
3. [Carregando e formatando os dados](#load)<br>
    3.1 [Função de limpeza de Consulta](#load1)<br>
    3.2 [Chamando o serviço que retorna os eventos](#load2)<br>
    3.3 [Agrupando as consultas dos pacientes por mês](#load3)<br>
4. [Gerando o arquivo de Excel](#save)<br>
