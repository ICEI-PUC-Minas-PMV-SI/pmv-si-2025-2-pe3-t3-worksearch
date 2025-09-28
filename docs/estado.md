# 2. ESTADO DA ARTE

A transformação do modelo de trabalho desde a Revolução Industrial é marcada pela progressiva diminuição da formalidade nas relações trabalhistas, fenômeno amplamente discutido na literatura (Carneiro et al., 2023). Nos últimos anos, o papel das plataformas digitais como intermediárias entre clientes e prestadores autônomos tornou-se central, com impactos econômicos e sociais significativos (Carneiro et al., 2023; Fonseca, 2021; Abílio, 2019). Esse processo tem sido denominado gig economy podendo ser traduzido como "economia dos bicos", em que a digitalização possibilita tanto o acesso de trabalhadores autônomos a novas oportunidades quanto o alcance dos clientes a esses profissionais (Fonseca, 2021; Carneiro et al., 2023).

Segundo Dedema (2023), a Uber, lançada em 2010, é considerada pioneira na digitalização massiva do trabalho autônomo. Em revisão sistemática de 515 artigos publicados ao longo de 12 anos, o autor destaca três eixos principais da pesquisa internacional: (1) o ambiente digital de trabalho, incluindo a infraestrutura informacional e a natureza dos serviços prestados; (2) a gestão algorítmica, abrangendo governança da informação, desempenho, assimetria de poder e manipulação de sistemas de big data; e (3) o design ético, relacionado aos valores que os trabalhadores esperam das plataformas sendo eles: (3.1) confiança, (3.2) justiça, (3.3) igualdade, (3.4) privacidade e (3.5) transparência. A literatura, contudo, indica que essas expectativas não se confirmam na prática, revelando uma lacuna entre valores desejados e práticas existentes.

No Brasil, a plataforma GetNinjas tem sido objeto de diversos estudos, servindo como caso representativo da lógica de marketplaces digitais. Grohman (2020), em pesquisa com 24 trabalhadores brasileiros, identificou que a maioria dos usuários da plataforma já possuía histórico de emprego formal, mas migrava para o aplicativo como meio de prospecção de clientes. Entre os problemas relatados, destacam-se: (1) concorrência intensa entre prestadores; (2) avaliação unilateral dos serviços; e (3) cobrança de taxas de acesso às oportunidades. Esses pontos reforçam as críticas recorrentes a modelos baseados em leilão reverso e monetização por leads (Lopes, 2021), em que profissionais pagam para concorrer sem garantias de retorno.

Amaral (2025) amplia a discussão trazendo a pauta da arquitetura da informação e seu diálogo com o crescimento das plataformas de intermediação, fenômeno denominado "uberização". O autor ressalta a dificuldade de localizar pequenos prestadores em nível local, mesmo quando disponíveis, devido à falta de transparência nos critérios de ranqueamento. Como resposta, propõe um framework de modelagem baseado em engenharia de requisitos e ontologias, com destaque para o uso de BPMN e taxonomias reutilizáveis em sistemas de matching e reputação. Tal proposta aponta a necessidade de superar a simplicidade das regras atuais (localização, categoria e avaliações), frequentemente limitadas por algoritmos opacos.

Outro ponto relevante é a lógica de monetização. Lopes (2021) demonstra que o modelo de "moedas virtuais" adotado por plataformas como GetNinjas cria uma barreira de entrada para trabalhadores, priorizando a sustentabilidade financeira da empresa em detrimento da garantia de retorno ao prestador. Esse mecanismo, classificado como pay-per-lead, tem sido criticado por reproduzir assimetrias de poder e gerar frustração entre trabalhadores (Dedema, 2023; Grohman, 2020).

Além disso, estudos recentes destacam que a lógica de reputação algorítmica permanece enviesada: clientes avaliam prestadores, mas o inverso raramente ocorre, o que gera um desequilíbrio na relação de poder (Pereira, 2023; Martins, 2021; Silva, 2023; Barreto, 2021). Isso contrasta com a expectativa de transparência e justiça documentada por Dedema (2023).

Do ponto de vista técnico, Amaral (2025) descreve os elementos básicos para o funcionamento dessas plataformas: (1) frontend adaptável em formato de Progressive Web App ou aplicativos nativos; (2) backend modularizado com APIs que abrangem pagamento, ranqueamento, avaliações, leads, notificações e suporte; e (3) integração com serviços externos, como gateways de pagamento e geolocalização. Ainda que funcional, esse modelo reforça a crítica de que a conectividade entre prestador e cliente é condicionada ao pagamento, restringindo o acesso e a transparência.

A literatura converge em torno de cinco principais lacunas:

1. **Ausência de documentação clara** sobre os critérios de ranqueamento e matching, que permanecem incompreensíveis para trabalhadores e clientes.

2. **Modelagem de reputação superficial e enviesada**, limitada ao prestador e sem valorização do papel do cliente.

3. **Escassez de soluções de usabilidade** voltadas para o prestador de serviço, dificultando que o trabalhador atinja seus objetivos.

4. **Predomínio de modelos de monetização** que transferem risco ao trabalhador (pay-per-lead), sem garantias de retorno.

5. **Interoperabilidade reduzida**: plataformas operam em sistemas fechados, limitando integrações com ERPs, CRMs ou ecossistemas abertos.

Essas lacunas reforçam a necessidade de novas propostas de design e operação de plataformas digitais de trabalho autônomo.

