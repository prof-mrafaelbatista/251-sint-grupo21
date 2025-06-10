# PythonInfo
O PythonInfo é um site fictício desenvolvido com o Flask, um microframework do Python para criação de aplicações web. Ele serve como uma plataforma educativa, onde os usuários aprendem lógica de programação e conceitos básicos de Python de forma interativa onde apresento:
Estruturas de Seleção que
permitem ao programa tomar decisões com base em condições, executando diferentes blocos de código conforme o resultado (verdadeiro ou falso) dessas condições.

Estruturas de Repetição que são utilizadas para repetir um bloco de código várias vezes, seja por um número determinado de vezes ou enquanto uma condição for verdadeira.

Vetores e Matrizes que são formas de armazenar coleções de dados. Vetores armazenam dados em uma única dimensão, enquanto matrizes organizam os dados em duas ou mais dimensões.

Funções e Procedimentos onde permitem organizar o código em blocos reutilizáveis. Funções retornam valores, enquanto procedimentos executam tarefas sem retornar necessariamente um valor.

Tratamento de Exceções que serve para lidar com erros de forma controlada, evitando que o programa pare de funcionar inesperadamente.


Foi utilizado no site o HTML que foi usada para estruturar o conteúdo das páginas web. Com ela, definimos textos, imagens, botões, dicionário de termos e outros elementos visuais do site e tambem o Python, usado para controlar a lógica do site. No caso do PythonInfo, é usado junto com o framework Flask para implementar as rotas.


O site PythonInfo utiliza a API do Gemini (uma inteligência artificial do Google) para oferecer respostas automáticas e explicações de código.
Como a integração foi feita:

Chave de API: Foi gerada uma chave de acesso na plataforma da Google para permitir o uso da API do Gemini.

Instalação de biblioteca: A biblioteca oficial do Gemini (como google.generativeai) foi instalada no projeto para facilitar a comunicação com a API.

Configuração no Flask: No backend em Python/Flask, foi criada uma rota que recebe perguntas dos usuários, envia para a API do Gemini e retorna a resposta.

Comunicação com o Frontend: O HTML do site possui campos onde o usuário digita sua dúvida. Ao enviar, o Flask envia a pergunta à API e exibe a resposta no navegador.

Essa integração torna o site mais interativo, acessivel e inteligente, ajudando os usuários a aprender Python com apoio de uma IA.



Para executar minha aplicação Flask localmente, primeiro eu instalei o Flask na minha ide, depois, entrei na pasta do projeto onde está o código do site PythonInfo.

Em seguida, configurei a variável de ambiente informando qual é o arquivo principal da aplicação. Depois disso, iniciei o servidor Flask e abri o navegador para acessar o endereço local, onde o site ficou disponível para eu testar e fazer ajustes.



No arquivo app.py, está toda a lógica principal do site usando Flask, nele foi definido:

As rotas que indicam quais páginas devem ser carregadas quando o usuário acessa determinados links;

A conexão com as páginas HTML, onde o Flask renderiza os arquivos HTML e envia dados para eles, se necessário;

A lógica do servidor onde acontecem os dicionario de termos, integração com APIs (como a do Gemini) e regras de funcionamento do site.
E também as páginas HTML que formaram a interface do site, o que o usuário vê e nelas estão:
A estrutura do conteúdo como textos, botões, glossário, códigos de exemplos, os links.

