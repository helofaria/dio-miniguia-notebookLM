# Miniguia de Introdução e Segurança de APIs com NotebookLM

## 📌 Contexto e Objetivos:
Este projeto consiste na criação de um caderno temático de estudos utilizando o NotebookLM. O objetivo principal é estruturar um material didático focado na **introdução às APIs e nas melhores práticas de segurança** para proteção de APIs.

---

## 📑 Curadoria das Fontes Iniciais

### 🔌 Introdução às APIs

#### Fontes em Texto:
*   [Introdução a APIs](https://experienceleague.adobe.com/pt-br/docs/platform-learn/data-collection/server-api/introduction)
*   [Introdução às Web APIs](https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Extensions/Client-side_APIs/Introduction)
*   [Introdução às APIs: Conceitos, Implementação e Boas Práticas - DIO](https://www.dio.me/articles/introducao-as-apis-conceitos-implementacao-e-boas-praticas)
*   [Entenda o que é uma API](https://www.alura.com.br/artigos/api?utm_term=&utm_campaign=&utm_source=google&utm_medium=cpc&campaign_id=23805973578__&utm_id=23805973578__&hsa_acc=7964138385&hsa_cam=&hsa_grp=&hsa_ad=&hsa_src=x&hsa_tgt=&hsa_kw=&hsa_mt=&hsa_net=google&hsa_ver=3&gad_source=1&gad_campaignid=23815806613&gclid=CjwKCAjw6MPRBhBTEiwAd-7Mr5RnVQbHivnM0zQ_aYoPM4lWX4vYd4OdF3G3b2_i5gEYKz87OMNeQxoCpuoQAvD_BwE)

#### Fontes em Vídeo:
*   [Design, Protocolos (REST, GraphQL, gRPC) e Segurança de APIs](https://www.youtube.com/watch?v=7iHl71nt49o) — *Abrange fundamentos e práticas essenciais.*
*   [Exemplo prático do que é uma API](https://www.youtube.com/watch?v=ZTz0xlCaIuw)
*   [API: Design e Arquitetura](https://www.youtube.com/watch?v=XvFmUE-36Kc&t=378s)
*   [Métodos de uma API](https://www.youtube.com/watch?v=viE7zOKoFOU)
  
---

### 🔒 Proteção e Segurança de APIs

#### Fontes em Texto:
*   [O que é segurança de API? - IBM](https://www.ibm.com/br-pt/think/topics/api-security)
*   [Segurança de APIs: como proteger seus dados?](https://transfeera.com/blog/seguranca-de-apis-proteger-dados/)
*   [10 práticas para proteger APIs - IBSEC](https://ibsec.com.br/10-praticas-para-proteger-apis/)
*   [Melhores práticas de segurança de APIs - IBM Insights](https://www.ibm.com/br-pt/think/insights/api-security-best-practices)


#### Fontes em Vídeo:
*   [Dicas Práticas de Segurança](https://www.youtube.com/watch?v=6WZ6S-qmtqY)
*   [Fundamentos da Segurança de APIs](https://www.youtube.com/watch?v=R-4_DbV1Su4&t=256s)
*   [O que é segurança em APIs](https://www.youtube.com/watch?v=FsB_nRGdeLs)
*   [Segurança no Desenvolvimento de APIs](https://www.youtube.com/watch?v=7oSEJ4BJhRo)

---

## 🧠 Engenharia de Prompts e "Cicatrizes"

Nesta seção, documento a estratégia utilizada para conduzir a Inteligência Artificial e extrair as respostas mais precisas com base nas fontes fornecidas.

### 👥 1. Definição de Persona
O primeiro passo foi definir um contexto para a IA:

* **Prompt de Contexto:** *"Assuma a postura de um educador especializado sobre a introdução à APIs e segurança delas, sem exagerar no uso de termos técnicos, é com objetivo de ajudar a alguém que está começando a entender sobre APIs."*

---

### 📥 2. Prompts

Aqui estão alguns exemplos de como as perguntas foram feitas para obter resultados para uma introdução a APIs e Segurança e Proteção de APIs:

#### 📤 Exemplos sobre uma Introdução a APIs 

*   **Exemplo 1: O que é API**
*   **Pergunta:** `Quais os principais assuntos introdutórios sobre APIs são importantes para quem está começando a estudar sobre APIs? Me de um breve resumo sobre eles.`
*   **Resposta resumida da IA:** A inteligência artificial assumiu o papel de educadora e estruturou os 8 pilares fundamentais para iniciantes:
    1.  **Conceito e Funcionamento:** A analogia do garçom como intermediário entre cliente e servidor.
    2.  **Verbos HTTP:** O uso de GET (ler), POST (criar), PUT/PATCH (atualizar) e DELETE (remover).
    3.  **Endpoints e Rotas:** As URLs que servem como pontos de acesso para as requisições.
    4.  **Formatos de Dados:** A predominância do JSON (chave-valor) sobre o antigo XML.
    5.  **Códigos de Status:** Respostas do servidor divididas em classes (2xx Sucesso, 4xx Erro do Cliente, 5xx Erro do Servidor).
    6.  **Arquiteturas:** A diferença entre o padrão tradicional REST e a flexibilidade do GraphQL.
    7.  **Segurança Inicial:** A separação entre Autenticação e Autorização.
    8.  **Documentação:** A importância do padrão OpenAPI/Swagger para guiar outros desenvolvedores.

*   **Exemplo 2: Planejamento**
*   **Pergunta:** `Como planejar detalhadamente uma API?`
*   **Resposta resumida da IA:** Estruturou um guia em 6 etapas, conectando desenvolvimento e segurança:
    1.  **Requisitos e Escopo:** Definição de casos de uso e modelagem inicial de ameaças para dados sensíveis.
    2.  **Arquitetura e Protocolos:** Escolha consciente do estilo (REST, GraphQL ou gRPC) e uso obrigatório de HTTPS/TLS para criptografia em trânsito.
    3.  **Elaboração do Contrato:** Uso do padrão OpenAPI (Swagger) em YAML/JSON para desenhar endpoints no plural, métodos HTTP e mapeamento de Status Codes.
    4.  **Segurança Nativa (Shift Left):** Planejamento de autenticação via OAuth 2.0/JWT, validação estrita de entradas e minimização de dados expostos.
    5.  **Escalabilidade:** Inclusão de paginação, controle de limite de requisições (*Rate Limiting*) e estratégias de versionamento na URL (ex: `/v1/`).
    6.  **Governança:** Centralização de tráfego por um API Gateway e geração automatizada de documentação para desenvolvedores e auditorias.
  

#### 📤 Exemplo da Segurança em APIs

*   **Exemplo 3: Introdução a Segurança**
*   **Pergunta:** `P: Quais vulnerabilidades na hora de implementar um API quem está começando a estudar deve se atentar?`
*   **Resposta resumida da IA:** 
    1.  **Autenticação Danificada:** Perigos de endpoints abertos ou envio inadequado de chaves de API na URL em vez de usar os cabeçalhos (*headers*).
    2.  **Exposição Excessiva de Dados e Atribuição em Massa:** O risco de expor o JSON do banco inteiro e a falta de controle ao mapear entradas de usuários, recomendando o uso de DTOs (*Data Transfer Objects*).
    3.  **Injeções (SQL/NoSQL/XSS):** Falhas causadas pela falta de validação e parametrização de consultas.
    4.  **Consumo Irrestrito de Recursos:** A falta de *Rate Limiting*, que expõe a API a ataques de negação de serviço (DoS).
    5.  **Configuração Incorreta:** Uso de HTTP em vez de HTTPS e exibição inadequada de erros técnicos para o usuário final.
    6.  **Gerenciamento de Inventário:** O perigo das "APIs zumbis" (versões antigas e esquecidas que ficam desprotegidas).
    7.  **Falhas de Autorização (BOLA/BFLA):** Riscos onde a API não valida a propriedade do recurso ou permite que usuários comuns acessem funções administrativas.

---

### ⚠️ 3. Cicatrizes (Troubleshooting)

#### 1: Perca do foco didático da IA e Repostas com termos complexos
* **Desafio:** Ao fazer algumas perguntas sobre os conceitos fundamentais e introdutorios, a IA trouxe respostas com uma linguagem muito tecnica, acredito pelo contexto de persona "a postura de um educador especializad", acabou usando termos complexos. Como o objetivo do notebook é servir de introdução e aprendizado para quem não sabe muito sobre APIs, a linguagem acabou ficando complexa para introdução para um iniciante.
* **Solução:** Fiz um ajuste estratégico no contexto da persona da IA. Reformulei o prompt de contexto exigindo que ela adotasse uma postura de educadora focada em ensinar sem exagerar no uso de termos técnicos, é com objetivo de ajudar a alguém que está começando a entender sobre APIs.

#### 2: Sobrecarga de Referências e Respostas repetitivas 
* **Desafio:** No início, adicionei um volume grande de fontes (diversos textos, sites, vídeos do YouTube, etc). Isso causou uma sobrecarga de contexto na IA percebi que ela não estava utilizando todo o seu potencial, ignorava os insights dos vídeos e começou a dar respostas repetitivas ou muito semelhantes apenas com trocas de palavras para perguntas que eram diferentes.
* **Solução:**  Primeiro, fiz uma limpeza das fontes, mantendo apenas o conteúdo essencial para o aprendizado e se precisar com o tempo adicionar apenas com conteúdo focado. Segundo, passei a construir prompts mais incisivos, pedindo para a IA cruzar mídias diferentes de forma explícita. Isso ajudou com as respostas mais explicativas porém para o objetivo de ser para aprendizado não ajudou muito com os prompts precisarem ser mais elaborados só para utilizar mais referências.

---

## 📖 Miniguia de Estudo 

Este guia foi preparado como material de apoio para introduzir iniciantes as APIs e sua segurança, sintetizando os aprendizados deste projeto.

### 📌 1. Resumos Estruturados: Introdução sobre APIs

#### O que é uma API e como ela funciona?
Uma API (Interface de Programação de Aplicações) funciona como uma ponte ou um contrato que permite que diferentes sistemas e aplicativos de software se comuniquem e troquem informações de maneira padronizada. Imagine a analogia de um restaurante: o cliente (usuário) escolhe um prato no cardápio, mas não fala diretamente com o chef (servidor); ele faz o pedido ao garçom (API), que leva a solicitação à cozinha e traz a resposta (o prato pronto) de volta para a mesa.
São fundamentais porque permitem que desenvolvedores utilizem funcionalidades complexas de terceiros como mapas do Google, pagamentos do PayPal ou previsões do tempo sem precisar criar tudo do zero. Além disso, elas funcionam como uma camada de segurança, ocultando os detalhes internos do sistema e expondo apenas o que é estritamente necessário para a integração.

#### Os Verbos HTTP: Como a API conversa?
Para que o "pedido" seja entendido, as APIs usam quatro comandos básicos que funcionam como ações no nosso dia a dia:
* **GET (Ler):** É quando você quer apenas visualizar uma informação. (Ex: Abrir o feed do Instagram para ver as fotos).
* **POST (Criar):** É quando você quer enviar uma informação nova. (Ex: Publicar uma foto nova ou cadastrar uma senha).
* **PUT/PATCH (Editar):** É quando você quer alterar algo que já existe. (Ex: Corrigir a legenda de uma foto que você postou).
* **DELETE (Excluir):** É quando você quer apagar uma informação do sistema. (Ex: Deletar uma postagem antiga).

#### Organização dos Dados: JSON e XML
Quando os sistemas trocam informações, eles precisam de uma linguagem comum para que ninguém se confunda. Hoje, as APIs usam principalmente duas estruturas:
* **JSON (O padrão moderno):** É extremamente leve e parece uma lista de compras organizada por categorias. Ele usa chaves `{ }` e aspas `" "` para ligar um nome ao seu valor. Por ser simples e direto, é o formato favorito dos desenvolvedores atuais.
* **XML (O padrão clássico):** É um formato mais antigo que funciona através de etiquetas, muito parecido com o HTML. Ele usa "tags" de abertura e fechamento (como `<nome>Caleb</nome>`) para envelopar a informação. É mais detalhado e formal, muito comum em sistemas de grandes empresas e bancos.

#### Como proteger a sua API?
* **Autenticação (Quem é você?):** É a chave da porta da frente. Antes de a API liberar qualquer dado, ela precisa ter certeza de quem está chamando. É aqui que entram os **Tokens (como o JWT)**, que funcionam como um crachá digital VIP: você se identifica uma vez, ganha o crachá e o apresenta toda vez que quiser entrar em uma sala.
* **Autorização:** Mesmo que você tenha a chave da porta da frente (autenticação), você não pode mexer em tudo. Se você é um cliente comum, não pode entrar na sala do administrador. Segurança básica significa garantir que o Usuário A nunca consiga ver ou alterar os dados do Usuário B só de mudar um número na barra de endereço do navegador.
* **Criptografia em Trânsito:** Quando a API envia os dados de volta para o usuário, essa informação viaja pela internet. Usar HTTPS garante que esses dados viajem criptografados e se tentarem interceptar o caminho, ele só vai ver códigos ilegíveis, protegendo senhas e dados sensíveis.

---

### 🗂️ 2. Glossário de Conceitos

* **API (Application Programming Interface):** Interface que permite a comunicação padronizada entre diferentes aplicações.
* **Endpoint:** A URL específica ou ponto de extremidade onde a API recebe as requisições.
* **JSON (JavaScript Object Notation):** Formato de dados leve, baseado em chave-valor, sendo o padrão mais utilizado em APIs modernas.
* **XML (Extensible Markup Language):** Formato baseado em tags (similar ao HTML), mais antigo e verboso, muito utilizado no protocolo SOAP.
* **Documentação / OpenAPI(Swagger):** Padrão de mercado para documentar a estrutura, parâmetros e respostas de uma API.
* **SQL Injection:** Vulnerabilidade onde comandos maliciosos são inseridos em campos de texto. Evita-se usando **consultas parametrizadas**.
* **Códigos de Status:** Respostas do servidor divididas em classes (2xx Sucesso, 4xx Erro do Cliente, 5xx Erro do Servidor).
* **Segurança Inicial:** A separação entre Autenticação e Autorização.
  
---

### 📥 3. Prompts Reutilizáveis 

Alguns prompts para usar no notebook para continuar praticando os conceitos sobre APIs:

1.  > *"Dê um resumo breve sobre os métodos de requisição de APIs,e um exemplo sobre cada um deles."*
2.  > *"Explique a diferença prática entre os formatos JSON e XML utilizando uma analogia simples do dia a dia."*
3.  > *"Crie um quiz de 5 perguntas de múltipla escolha sobre verbos HTTP e códigos de status, apresentando as respostas justificadas no final."*
4.  > *"Dê 5 dicas práticas e detalhadas de como implementar sua primeira API em Python"*
