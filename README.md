# 1 INTRODUÇÃO

A ascensão das ferramentas de Inteligência Artificial generativa tem transformado radicalmente o processo de desenvolvimento de software. O fenômeno conhecido como "vibe coding" caracteriza-se pelo desenvolvimento acelerado de aplicações com auxílio massivo de assistentes de IA, priorizando a velocidade de entrega em detrimento de práticas consolidadas de engenharia de software. Embora essa abordagem permita a materialização rápida de ideias, especialmente em ambientes de startups e SaaS, ela introduz riscos significativos relacionados à qualidade, segurança e sustentabilidade do código produzido.

O conceito de dívida técnica, proposto inicialmente por Cunningham (1992), refere-se ao custo implícito de retrabalho causado pela escolha de soluções rápidas em vez de alternativas mais robustas. No contexto do vibe coding, essa dívida se manifesta de forma particularmente preocupante, pois desenvolvedores podem incorporar código gerado por IA sem compreensão profunda de suas implicações arquiteturais, de segurança ou de manutenibilidade.

Casos recentes no mercado brasileiro evidenciam as consequências dessa abordagem. Um aplicativo de relacionamento para mulheres LGBTQIA+ sofreu exposição massiva de dados sensíveis devido a falhas básicas de segurança, incluindo informações de KYC (Know Your Customer), conversas privadas e dados pessoais. O incidente não apenas violou a Lei Geral de Proteção de Dados (LGPD), mas também traiu a confiança de uma comunidade vulnerável que buscava um espaço seguro. A situação foi agravada pela resposta inadequada da equipe de desenvolvimento às notificações de pesquisadores de segurança, demonstrando lacunas não apenas técnicas, mas também de governança e cultura de segurança.

Li, Avgeriou e Liang (2015) argumentam que a dívida técnica acumula-se através de diversos mecanismos: código duplicado, falta de documentação, ausência de testes automatizados, violações de padrões arquiteturais e negligência de requisitos não funcionais. No desenvolvimento assistido por IA, esses problemas se amplificam, pois o código gerado pode parecer funcionalmente correto enquanto oculta vulnerabilidades críticas de segurança, problemas de desempenho ou dependências inadequadas.

A problemática torna-se especialmente crítica quando consideramos que, segundo projeções da indústria, a demanda por desenvolvedores aumentará significativamente nos próximos anos, enquanto a formação de profissionais qualificados não acompanha esse ritmo. Isso cria um cenário propício para a adoção acrítica de ferramentas que prometem produtividade imediata, mas que podem comprometer a qualidade estrutural do software.

## 1.1 PROBLEMA

Como o fenômeno do vibe coding, caracterizado pelo desenvolvimento acelerado com auxílio massivo de ferramentas de IA generativa, contribui para o acúmulo de dívidas técnicas em projetos de software, particularmente no que tange à segurança da informação, manutenibilidade do código e conformidade com regulamentações como a LGPD?

A hipótese deste estudo é que o uso intensivo de ferramentas de IA para geração de código, sem processos adequados de revisão, validação de segurança e compreensão profunda das soluções implementadas, resulta em acúmulo acelerado de dívida técnica, manifestando-se em vulnerabilidades de segurança, código de baixa qualidade e custos elevados de manutenção a médio e longo prazo.

## 1.2 OBJETIVOS

### 1.2.1 Objetivo Geral

Investigar a relação entre a prática de vibe coding e o acúmulo de dívidas técnicas em projetos de desenvolvimento de software, analisando seus impactos na qualidade, segurança e sustentabilidade das aplicações produzidas.

### 1.2.2 Objetivos Específicos

a) Caracterizar o fenômeno do vibe coding no contexto contemporâneo de desenvolvimento de software, identificando suas práticas, ferramentas e motivações;

b) Mapear as principais categorias de dívidas técnicas introduzidas pelo desenvolvimento acelerado com auxílio de IA, com ênfase em aspectos de segurança da informação;

c) Analisar casos reais de falhas de segurança e qualidade em aplicações desenvolvidas sob o paradigma do vibe coding, incluindo o caso do aplicativo de relacionamento brasileiro;

d) Propor diretrizes e práticas de mitigação que permitam conciliar a agilidade proporcionada por ferramentas de IA com a qualidade e segurança necessárias em sistemas de produção;

e) Avaliar a percepção de profissionais da área quanto aos riscos e benefícios do desenvolvimento assistido por IA.

## 1.3 JUSTIFICATIVA

A relevância deste estudo fundamenta-se em três pilares principais. Primeiramente, o aspecto tecnológico: a proliferação de ferramentas de IA generativa para desenvolvimento de software representa uma mudança paradigmática na forma como sistemas são construídos. Compreender os riscos e limitações dessa abordagem é fundamental para evitar a repetição sistemática de erros que comprometem a segurança e qualidade do software.

Em segundo lugar, a dimensão econômica: segundo Kruchten, Nord e Ozkaya (2012), o custo de correção de dívidas técnicas cresce exponencialmente com o tempo. Organizações que adotam o vibe coding sem estratégias adequadas de gestão de qualidade podem enfrentar custos proibitivos de retrabalho, perda de clientes e danos reputacionais. O mercado brasileiro, especialmente o ecossistema de startups, tem adotado essas práticas de forma acelerada, tornando urgente a discussão sobre seus impactos.

O terceiro pilar é o aspecto social e legal: aplicações que lidam com dados sensíveis, como informações pessoais, dados de saúde, localização e comunicações privadas, têm responsabilidades amplificadas sob a LGPD. Falhas de segurança não são apenas problemas técnicos, mas violações de direitos fundamentais que podem expor indivíduos a riscos significativos, especialmente membros de comunidades vulneráveis. O caso do aplicativo LGBTQIA+ ilustra como a negligência técnica pode ter consequências graves para a segurança física e psicológica de usuários.

Além disso, este estudo contribui para a formação de profissionais de engenharia de software, oferecendo subsídios teóricos e empíricos para uma postura crítica e responsável frente às novas tecnologias. Como observado por Sommerville (2016), a engenharia de software não se resume à escrita de código, mas engloba práticas de qualidade, segurança, ética e responsabilidade profissional.

## 1.4 CARACTERIZAÇÃO DA METODOLOGIA

Esta pesquisa caracteriza-se como exploratória e qualitativa, com triangulação de dados provenientes de múltiplas fontes. A natureza exploratória justifica-se pelo caráter recente do fenômeno estudado, enquanto a abordagem qualitativa permite compreensão aprofundada das práticas, percepções e contextos envolvidos no vibe coding.

### 1.4.1 Universo e Amostra

O universo da pesquisa compreende profissionais de desenvolvimento de software atuantes no mercado brasileiro, com foco em startups, empresas de SaaS e projetos que utilizam ferramentas de IA generativa. A amostra será composta por:

a) 15 a 20 desenvolvedores que utilizam ferramentas de IA regularmente em seu trabalho;

b) 5 a 8 líderes técnicos (CTOs, arquitetos de software, tech leads) com experiência em gestão de dívida técnica;

c) 3 a 5 especialistas em segurança da informação e proteção de dados.

A seleção dos participantes seguirá critério de amostragem não probabilística por conveniência e bola de neve, priorizando diversidade de experiência, tipo de organização e tecnologias utilizadas.

### 1.4.2 Instrumentos

Serão utilizados três instrumentos principais de coleta de dados:

a) Entrevistas semiestruturadas: roteiro com questões abertas sobre práticas de desenvolvimento, uso de ferramentas de IA, percepções sobre qualidade e segurança, e experiências com dívida técnica. As entrevistas terão duração estimada de 45 a 60 minutos e serão realizadas remotamente via videoconferência.

b) Análise documental: exame de relatórios de vulnerabilidades, postagens em redes sociais sobre incidentes de segurança, documentações técnicas de ferramentas de IA, e guidelines de organizações sobre uso de código gerado por IA.

c) Estudo de caso: análise aprofundada do incidente de vazamento de dados do aplicativo brasileiro, incluindo análise técnica das vulnerabilidades, timeline de eventos, resposta da organização e impactos observados.

### 1.4.3 Procedimentos

A pesquisa será conduzida em quatro etapas:

Etapa 1 - Revisão sistemática de literatura: levantamento e análise de estudos sobre dívida técnica, desenvolvimento assistido por IA, qualidade de software e segurança da informação. Bases consultadas incluirão IEEE Xplore, ACM Digital Library, ScienceDirect e Google Scholar.

Etapa 2 - Coleta de dados primários: realização de entrevistas com participantes selecionados, mediante consentimento informado e garantia de confidencialidade. As entrevistas serão gravadas (com autorização), transcritas e codificadas tematicamente.

Etapa 3 - Análise de dados: aplicação de análise de conteúdo temática sobre transcrições de entrevistas, identificando padrões, categorias emergentes e relações entre os fenômenos estudados. Os dados documentais serão analisados através de análise crítica e triangulação com dados primários.

Etapa 4 - Síntese e proposição: consolidação dos achados em framework conceitual que relaciona práticas de vibe coding, tipos de dívida técnica e estratégias de mitigação, culminando em conjunto de diretrizes práticas para profissionais e organizações.

## 1.5 EMBASAMENTO TEÓRICO

O referencial teórico deste trabalho estrutura-se em torno de três pilares conceituais fundamentais:

Dívida Técnica: baseado nos trabalhos seminais de Cunningham (1992) e nas taxonomias desenvolvidas por Alves et al. (2016) e Li, Avgeriou e Liang (2015), que categorizam a dívida técnica em dimensões arquitetural, de código, de documentação, de testes e de defeitos. O conceito de juros da dívida técnica, proposto por Kruchten, Nord e Ozkaya (2012), será utilizado para analisar os custos de longo prazo das decisões técnicas tomadas sob pressão de velocidade.

Qualidade de Software e Segurança: fundamentado nos princípios da norma ISO/IEC 25010, que define características de qualidade de produto de software, e nos frameworks de segurança como OWASP Top 10 e princípios de Security by Design. Trabalhos de McGraw (2006) sobre segurança em software e de Viega e McGraw (2001) sobre defeitos de segurança fornecerão base para análise das vulnerabilidades decorrentes do vibe coding.

Desenvolvimento Assistido por IA: literatura emergente sobre ferramentas de geração de código por IA, incluindo estudos sobre GitHub Copilot, ChatGPT e similares. Pesquisas de Dakhel et al. (2023) sobre segurança de código gerado por IA e de Nguyen e Nadi (2022) sobre qualidade e compreensibilidade do código assistido por IA serão fundamentais para contextualizar os riscos específicos dessa abordagem.

## 1.6 ESTRUTURA DO TRABALHO

Este trabalho está organizado em quatro capítulos principais além desta introdução:

O Capítulo 2 apresenta uma revisão abrangente da literatura sobre dívida técnica, suas causas, manifestações e consequências, seguida de discussão sobre ferramentas de IA generativa no desenvolvimento de software e suas implicações. São também abordados aspectos de segurança da informação e conformidade regulatória, com ênfase na LGPD.

O Capítulo 3 descreve os resultados da pesquisa empírica, apresentando dados das entrevistas realizadas, análise do estudo de caso do aplicativo brasileiro, e categorização das dívidas técnicas identificadas em projetos que adotam vibe coding.

O Capítulo 4 oferece análise crítica dos dados coletados, discutindo as relações entre práticas de desenvolvimento, acúmulo de dívida técnica e manifestação de problemas de qualidade e segurança. São também propostas diretrizes práticas para mitigação dos riscos identificados.

Finalmente, a Conclusão sintetiza os principais achados da pesquisa, suas contribuições teóricas e práticas, limitações do estudo e sugestões para pesquisas futuras.

---

# 2 DESENVOLVIMENTO

## 2.1 DÍVIDA TÉCNICA: CONCEITOS E TAXONOMIA

O conceito de dívida técnica foi introduzido por Ward Cunningham em 1992, estabelecendo uma metáfora financeira para descrever o custo futuro de decisões de desenvolvimento tomadas no presente. Assim como uma dívida financeira acumula juros ao longo do tempo, decisões técnicas subótimas geram custos crescentes de manutenção, evolução e correção (CUNNINGHAM, 1992).

McConnell (2007) propõe uma distinção fundamental entre dívida técnica intencional e não intencional. A dívida intencional resulta de decisões conscientes de fazer concessões técnicas em favor de objetivos de negócio, como time-to-market. Já a dívida não intencional surge de falta de conhecimento, habilidades inadequadas ou negligência. No contexto do vibe coding, observa-se predominância de dívida não intencional, pois desenvolvedores frequentemente desconhecem as implicações do código gerado por IA.

Alves et al. (2016) desenvolveram uma taxonomia abrangente de dívida técnica, categorizando-a em treze tipos distintos. Para este estudo, destacam-se:

Dívida de Código: código mal estruturado, duplicado ou que viola princípios de design. Manifesta-se através de alta complexidade ciclomática, baixa coesão e alto acoplamento. Ferramentas de IA frequentemente geram código que, embora funcional, apresenta esses problemas estruturais.

Dívida de Arquitetura: decisões arquiteturais inadequadas que dificultam evolução e manutenção do sistema. Incluem violações de padrões arquiteturais, dependências inadequadas e falta de modularização apropriada.

Dívida de Documentação: ausência ou inadequação de documentação técnica, incluindo comentários de código, documentação de APIs e diagramas arquiteturais. O código gerado por IA raramente vem acompanhado de documentação contextual adequada.

Dívida de Testes: cobertura insuficiente de testes automatizados, qualidade inadequada dos testes existentes ou ausência de estratégia de testes. Este tipo de dívida é particularmente crítico em código gerado por IA, que pode conter comportamentos não óbvios.

Dívida de Defeitos: bugs conhecidos não corrigidos que se acumulam no sistema. No vibe coding, defeitos podem permanecer ocultos devido à falta de revisão adequada do código gerado.

Li, Avgeriou e Liang (2015) observam que a dívida técnica não é intrinsecamente negativa quando gerenciada adequadamente. Organizações podem fazer trade-offs conscientes entre velocidade e qualidade, desde que compreendam os custos futuros e estabeleçam estratégias de pagamento dessa dívida. O problema surge quando a dívida se acumula sem controle ou monitoramento.

Kruchten, Nord e Ozkaya (2012) introduzem o conceito de juros da dívida técnica, representando o esforço adicional contínuo necessário devido à presença de dívida. Juros se manifestam como:

a) Tempo extra para implementar novas funcionalidades devido à complexidade ou fragilidade do código existente;

b) Esforço adicional de teste e depuração causado por instabilidade ou falta de cobertura de testes;

c) Dificuldade de compreensão do código por novos membros da equipe ou pelo próprio autor após algum tempo;

d) Riscos aumentados de introdução de novos defeitos ao modificar código problemático.

Guo, Seaman e Zazworka (2011) realizaram estudo empírico demonstrando que aproximadamente 25% do esforço de desenvolvimento em projetos maduros é consumido pagando juros de dívida técnica. Em projetos com alta dívida, esse percentual pode ultrapassar 50%, tornando o desenvolvimento progressivamente mais lento e custoso.

## 2.2 VIBE CODING E FERRAMENTAS DE IA GENERATIVA

O termo "vibe coding" emergiu recentemente na comunidade de desenvolvimento para descrever uma abordagem de programação caracterizada pelo uso intensivo de ferramentas de IA generativa, priorização de velocidade sobre qualidade, e desenvolvimento baseado mais em intuição e experimentação rápida do que em planejamento arquitetural rigoroso (CHEN et al., 2023).

Barke et al. (2023) conduziram estudo etnográfico com desenvolvedores usuários do GitHub Copilot, identificando padrões de uso que incluem: geração de código boilerplate, implementação de funcionalidades conhecidas mas não memorizadas, exploração de APIs desconhecidas, e até mesmo geração de lógica de negócio complexa. Os autores observam que desenvolvedores frequentemente aceitam sugestões da IA com revisão mínima, especialmente sob pressão de tempo.

Dakhel et al. (2023) investigaram especificamente a segurança de código gerado por ferramentas de IA, revelando descobertas preocupantes. Em amostra de 1.897 programas gerados pelo GitHub Copilot para tarefas de segurança crítica, 40% continham vulnerabilidades de segurança, incluindo:

a) Injeção de SQL devido a falta de sanitização de inputs;

b) Cross-Site Scripting (XSS) em código de aplicações web;

c) Uso de funções criptográficas obsoletas ou implementadas incorretamente;

d) Exposição de informações sensíveis através de logs inadequados;

e) Validação insuficiente de dados de entrada.

Crucialmente, os autores demonstraram que desenvolvedores com menos experiência em segurança eram significativamente mais propensos a aceitar código vulnerável gerado por IA sem identificar os problemas. Isso cria um ciclo vicioso onde a ferramenta que promete democratizar o desenvolvimento pode, na verdade, amplificar riscos de segurança.

Nguyen e Nadi (2022) analisaram a qualidade e compreensibilidade de código gerado por modelos de linguagem, encontrando que, embora o código seja frequentemente correto funcionalmente, ele apresenta problemas significativos de manutenibilidade. Os autores identificaram padrões como:

a) Nomes de variáveis e funções genéricos ou não descritivos;

b) Ausência de tratamento adequado de erros e casos extremos;

c) Lógica desnecessariamente complexa onde soluções mais simples seriam apropriadas;

d) Falta de modularização e reutilização de código;

e) Inconsistência estilística mesmo dentro de um único arquivo.

Vaithilingam et al. (2022) conduziram estudos de usabilidade com programadores utilizando ferramentas de IA, revelando que a experiência do usuário é significativamente afetada por sugestões incorretas ou inadequadas. Desenvolvedores relataram frustração quando a IA gera código que parece correto mas contém erros sutis, pois o tempo gasto identificando e corrigindo esses erros frequentemente excede o tempo que seria necessário para escrever o código manualmente.

## 2.3 SEGURANÇA DA INFORMAÇÃO E LGPD

A Lei Geral de Proteção de Dados (Lei nº 13.709/2018) estabelece princípios e diretrizes para tratamento de dados pessoais no Brasil. O artigo 6º estabelece princípios fundamentais, destacando-se o princípio da segurança, que determina a utilização de medidas técnicas e administrativas aptas a proteger os dados pessoais de acessos não autorizados e de situações acidentais ou ilícitas de destruição, perda, alteração, comunicação ou difusão (BRASIL, 2018).

Bioni (2019) argumenta que a LGPD não prescrev
