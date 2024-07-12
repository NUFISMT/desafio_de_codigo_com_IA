# desafio_de_codigo_com_IA

Descrição
Você está desenvolvendo um sistema de geração de sugestões de tópicos para um blog de tecnologia. O objetivo é associar características específicas dos modelos Claude 3 da Anthropic às palavras-chave fornecidas e fornecer o nome do modelo correspondente como saída.
Entrada
Uma descrição correspondente a um dos modelos Claude 3 da Anthropic, como "automatizar tarefas" ou "equilíbrio ideal entre inteligência e velocidade".
Saída
O nome do modelo Claude 3 que melhor corresponde à característica fornecida na entrada, como "Claude 3 Opus", "Claude 3 Sonnet" e "Claude 3 Haiku". Caso a entrada não possua características dos modelos citados acima, o programa deve retornar uma mensagem: "Modelo não encontrado."
Exemplos
A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.
Entrada	Saída
Automatizar tarefas, criar aplicações voltadas para o usuário que geram receita e acelerar a pesquisa e o desenvolvimento em diversos setores.	Claude 3 Opus
Equilíbrio ideal entre inteligência e velocidade, especialmente para workloads corporativas. Ele se destaca em raciocínio complexo, criação de conteúdo diferenciado, consultas científicas, matemática e codificação.	Claude 3 Sonnet
Resposta rápida e capacidade de resposta quase instantânea, imitação das interações humanas, moderar conteúdo, otimizar gerenciamento de inventário, produzir traduções rápidas e precisas, resumir dados não estruturados.	Claude 3 Haiku

Observação :O código deve seguir a seguinte estrutura no ambiente de execução:
# Dicionário associando características aos modelos Claude 3
caracteristicas_modelos = {
    "automatizar tarefas": "Claude 3 Opus",
    "pesquisa e desenvolvimento": "Claude 3 Opus",
    "resposta rápida e capacidade de resposta quase instantânea": "Claude 3 Haiku",
    "motores de chatbots de lojas": "Claude 3 Haiku",
    "moderação de conteúdo": "Claude 3 Haiku",
    "processamento de tarefas mais básicas": "Claude 3 Haiku",
    "raciocínio cuidadoso": "Claude 3 Sonnet",
    "processamento de dados": "Claude 3 Sonnet",
    "aplicações de vendas": "Claude 3 Sonnet",
    "extração de texto de imagens": "Claude 3 Sonnet",
    "equilíbrio ideal entre inteligência e velocidade": "Claude 3 Sonnet",
   
}

# TODO: Crie uma função 'encontrar_modelo' para encontrar o modelo correspondente à característica fornecida: 

# TODO: Itere sobre cada chave e valor no dicionário caracteristicas_modelos:
   
# TODO: Verifique se a palavra-chave (característica) está contida na característica fornecida (ignorando maiúsculas/minúsculas):
        
# TODO: Se encontrada, retorne o modelo correspondente:
           
# TODO: Se não encontrada, retorne uma mensagem indicando que o "Modelo não encontrado.":
 

# Entrada do usuário
caracteristica_fornecida = input()

# Encontrar e imprimir o modelo correspondente
modelo_correspondente = encontrar_modelo(caracteristica_fornecida)
print(modelo_correspondente)


# Desafio 2

Descrição

Neste desafio, o objetivo ajudar na escolha do modelo de inteligência artificial mais adequado com base em critérios específicos definidos pelo cliente, utilizando as inovações recentemente anunciadas pela Amazon Web Services (AWS). Os modelos de IA disponíveis são da família Claude 3, desenvolvidos pela Anthropic, que foram anunciados como disponíveis na plataforma Amazon Bedrock. Esses modelos de última geração foram projetados para oferecer um equilíbrio entre precisão, desempenho, velocidade e custo, atendendo às demandas de clientes de todos os tamanhos.

Atenção:
Alguns dados que utilizados são simulados e podem não representar situações reais.
Entrada

A entrada consiste em quatro linhas, cada uma representando uma característica do modelo de inteligência artificial:

1. Desempenho: um número inteiro indicando a capacidade de desempenho do modelo.
2. Velocidade: um número inteiro representando a velocidade de processamento do modelo.
3. Custo: um número inteiro que reflete o custo associado ao modelo.
4. Capacidades: uma lista de capacidades específicas separadas por vírgulas.
Saída

O programa fornecerá a recomendação do modelo mais adequado com base nas características fornecidas. A saída incluirá uma explicação detalhada sobre por que esse modelo específico foi escolhido com base nos critérios estabelecidos pelo cliente, utilizando informações sobre os modelos Claude 3 disponíveis na plataforma Amazon Bedrock. Se nenhum modelo atender aos critérios, o programa informará que nenhum modelo foi encontrado.
Exemplos

A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.
Entrada 	Saída
9
10
5
Pesquisa, Desenvolvimento Acelerado 	O Claude 3 Opus é o modelo recomendado.
8
5
7
Codificação, Recuperação de informações 	O Claude 3 Sonnet é o modelo recomendado.
7
9
6
Velocidade, Resumo de dados não estruturados 	O Claude 3 Haiku é o modelo recomendado.
1
5
9
Viagem interplanetária, Autoconhecimento 	Nenhum modelo encontrado.

Informações sobre os Modelos Claude 3:

Os modelos Claude 3, recentemente disponibilizados pela Anthropic em parceria com a AWS, representam uma evolução significativa no campo da inteligência artificial, destacando-se em termos de:

    Inteligência Avançada: Os modelos Claude 3 demonstram níveis avançados de inteligência, aproximando-se dos níveis de resposta humana e superando outros modelos disponíveis em áreas como raciocínio, matemática e programação.

    Velocidade Aprimorada: Claude 3 Sonnet oferece uma combinação otimizada de habilidades e velocidade, sendo duas vezes mais rápido que modelos anteriores da família Claude em uma grande variedade de cargas de trabalho, enquanto mantém níveis mais altos de inteligência.

    Custo e Acessibilidade: Claude 3 Haiku, projetado para ser o modelo mais rápido e compacto do mercado, oferece uma das opções mais acessíveis para sua categoria de inteligência, mantendo uma responsividade próxima à interação humana.

    Capacidades de Visão Avançadas: Todos os modelos Claude 3 possuem capacidades avançadas de visão, permitindo o processamento de diversos formatos de dados e análise de imagens, atendendo à crescente demanda por modelos que compreendam melhor gráficos, diagramas técnicos, fotos e outros ativos visuais.

    


# Desafio 3
    
Descrição

Você foi contratado para desenvolver uma lista de dicionários chamado modelos_disponiveis contendo os modelos de inteligência artificial (IA) da Amazon Bedrock, dentro da lista crie três dicionários, sendo, nome, pontuacao_desempenho e preco_mensal, cada um deles representa um modelo disponível para recomendação e suas características.

Em seguida crie uma função chamada recomendar_modelo e receba dois parâmetros que será modelos e orçamento, que representa uma lista de modelos e o orçamento do usuário em unidades monetárias. Dentro da função recomendar_modelo verifique se o orçamento fornecido é suficiente para recomendar algum modelo. Se o orçamento for inferior a 250 unidades monetárias, a função retorna uma tupla com dois elementos:

1. "None": indicando que nenhum modelo pode ser recomendado.
2. Uma mensagem de aviso informando que o orçamento é muito baixo para recomendar um modelo adequado..

O objetivo geral do desafio é selecionar o melhor modelo que é escolhido com base no orçamento, priorizando modelos com preço mais próximo ao orçamento fornecido pelo usuário.

Detalhes dos Modelos:
- Modelo: Claude 3 Opus. Desempenho: 9. Preço mensal: $ 600;
- Modelo: Claude 3 Sonnet. Desempenho: 8. Preço mensal: $ 450;
- Modelo: Claude 3 Haiku. Desempenho: 7. Preço mensal: $ 350;

Atenção:
Alguns dados que utilizados são simulados e podem não representar situações reais.
Entrada

O usuário deve fornecer os detalhes seu orçamento para que seja avaliado o melhor modelo com base no seu orçamento pelo preço mensal e desempenho.
Saída

Com base nos modelos fornecidos e no orçamento especificado, a função deve recomendar o modelo adequado conforme o seu orçamento. O melhor modelo sugerido deve ser escolhido com base no orçamento, priorizando modelos com preço mais próximo ao orçamento fornecido pelo usuário. Caso o orçamento seja menor do que 250, retorne uma mensagem informando: "Se orçamento é muito baixo para recomendar um modelo adequado."
Exemplos

A tabela abaixo apresenta exemplos com alguns dados de entrada e suas respectivas saídas esperadas. Certifique-se de testar seu programa com esses exemplos e com outros casos possíveis.
Entrada 	Saída

300 	Claude 3 Haiku. Este modelo está mais próximo do seu orçamento.

700 	Claude 3 Opus. Melhor desempenho dentro do seu orçamento.

550 	Claude 3 Sonnet. Melhor desempenho dentro do seu orçamento.
249 	Seu orçamento é muito baixo para recomendar um modelo adequado.
Essas características tornam os modelos Claude 3 uma escolha preferencial para clientes em diversas indústrias que buscam desenvolver aplicações de IA generativa de ponta, impulsionando a inovação e reinventando experiências de usuário.

