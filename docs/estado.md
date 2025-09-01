# 2. ESTADO DA ARTE
<!--O estado da arte é um mapeamento de toda a produção acadêmica sobre um assunto específico, aqui especificamente sobre o tema escolhido para o seu trabalho. A ideia consiste em reunir as conclusões que outras pesquisas científicas chegaram sobre um determinado assunto. Neste momento você deverá buscar respostas para as seguintes perguntas:

1.	Quais pesquisas estão sendo desenvolvidas sobre esse tema?
2.	Quem está pesquisando e onde?
3.	O que as atuais pesquisas científicas concluíram sobre o tema? 
4.	Quais as divergências dos pesquisadores sobre o assunto? 
5.	Quais aspectos carecem de maior abordagem?

É importante referenciar estas pesquisas, fazendo as devidas citações de acordo com as normas da ABNT e colocando as referências completas ao final do trabalho.-->

As plataformas digitais de prestação de serviços têm transformado significativamente as dinâmicas de intermediação entre clientes e profissionais autônomos. Modelos como o da plataforma GetNinjas exemplificam a adoção de sistemas técnicos baseados em algoritmos, fluxos de informação otimizados e mecanismos digitais de monetização, como leads pagos e moedas virtuais. Essas plataformas funcionam como marketplaces, oferecendo uma arquitetura híbrida que integra aplicações web e mobile, sistemas de ranqueamento, geolocalização e controle de reputação.
Nos últimos anos, o crescimento desse tipo de serviço motivou uma série de pesquisas acadêmicas com diferentes enfoques — desde aspectos sociais e jurídicos até abordagens técnicas voltadas à engenharia de sistemas, usabilidade e lógica algorítmica. Este trabalho tem como objetivo apresentar o estado da arte dessas pesquisas sob uma perspectiva técnica, analisando as soluções desenvolvidas, os modelos de negócio adotados, as divergências teóricas e as lacunas ainda existentes no campo.

### 1. Pesquisas Técnicas Desenvolvidas sobre Plataformas de Serviços Digitais
As pesquisas técnicas abordam principalmente:
#### a) Arquitetura da informação em plataformas de intermediação digital
A tese de Eduardo Diniz Amaral (UFSC) investiga os fluxos de informação entre usuários (clientes e prestadores), propondo um framework para modelagem de plataformas de serviço, baseado em engenharia de requisitos e modelagem ontológica.
Ele explora métodos como BPMN e modelos taxonômicos reutilizáveis aplicados a sistemas de matching e gerenciamento de reputação.
#### b) Modelos de funcionamento e monetização técnica (moedas e leads)
A pesquisa da UFBA analisa o sistema técnico de cobrança por leads, no qual profissionais precisam adquirir “moedas virtuais” para destravar contatos — um modelo técnico de pay-per-lead embutido no backend da plataforma.
O sistema opera por lógica de leilão reverso algorítmico: o cliente publica uma demanda e os profissionais disputam para oferecer propostas, sem garantia de retorno.
#### c) Controle algorítmico e mediação via IA simples
Diversos artigos descrevem a lógica de matching baseada em:
Localização (geolocalização/GPS);
Avaliações anteriores;
Categorias de serviço.
A lógica é implementada via regras de negócio simples, mas cada vez mais influenciada por mecanismos de ranqueamento e reputação algorítmica.
#### d) Modelos de negócios freemium com backend modularizado
Estudos sobre o modelo de negócios do GetNinjas apontam o uso de sistemas modulares, em que:
O front-end funciona como uma vitrine adaptada (Progressive Web App ou aplicativo nativo);
O back-end opera com microserviços para:
- pagamento;
- ranqueamento;
- avaliação;
- leads;
- notificações;
- suporte.

As plataformas utilizam APIs para integração com serviços de terceiros (gateways de pagamento, mapas, notificações, etc.).

### 2. Principais Pesquisadores e Instituições Envolvidas

|Pesquisador    | Instituição  | Enfoque técnico|
|------|-----------------------------------------|----|
| Eduardo Diniz Amaral | UFSC (PPGCI) | Modelagem de sistemas de informação, arquitetura da informação, ontologias. |
| Randerson Lopes | UFBA | Análise crítica de sistemas de cobrança por moeda virtual e leilão reverso. |
| Helena Martins & Jonas Valente | UFC / University of Oxford | Controle algorítmico, vigilância digital do trabalho, subsunção tecnológica. |
| Autores diversos (ResearchGate) | Diversas Universidades | Modelos de reputação, engenharia de plataforma, monetização escalável. |

### 3. Conclusões Técnicas das Pesquisas Científicas sobre o Tema
- As plataformas operam como sistemas híbridos e escaláveis, com:
  - Front-end (web/mobile) para geração de demanda;
  - Back-end com microserviços, para processamento de transações, leads, reputação e notificações.
    
- O sistema de monetização por moedas/leads é sistematicamente desenhado para gerar receita constante, mesmo sem garantia de retorno ao prestador. Isso levanta críticas técnicas e éticas.
  
- O sistema de matching funciona com base em critérios técnicos fixos:
  - Geolocalização (via API de mapa);
  - Categoria do serviço;
  - Reputação (nota e volume de atendimentos);
  - Moedas disponíveis.
  
  Resultado: o acesso às oportunidades é condicionado por barreiras técnicas (paywall digital).

- A arquitetura dos fluxos de dados é centralizada e opaca:
  - O prestador só visualiza o cliente após o pagamento;
  - O cliente vê apenas candidatos selecionados pelo algoritmo;
  - O algoritmo não é transparente.



### 4. Divergências Técnicas entre Pesquisadores

|Tema | Visão (A) | Visão (B) |
|------|-----------------------------------------|----|
| Sistema de moedas | Estratégia legítima e escalável de monetização | Modelo tecnicamente injusto, que transfere risco ao prestador |
| Matching algorítmico | Automatiza o processo com critérios objetivos | Gera desigualdade e bolhas de reputação, sem transparência algorítmica |
| Leilão reverso digital | Reduz custos para o cliente e aumenta a concorrência | Gera “corrida para o fundo” e afeta a sustentabilidade técnica do profissional |
| Arquitetura de sistema | Modular e replicável para múltiplos nichos | Centralizada e opaca, favorecendo apenas a plataforma |





### 5. Lacunas Técnicas e Demandas por Novas Abordagens
   
#### a) Transparência algorítmica
- Falta documentação técnica clara sobre:
  - Ranqueamento;
  - Critérios de matching;
  - Distribuição de leads.
- Recomendação: auditorias algorítmicas e logs de decisão.
  
#### b) Modelagem de reputação e viés técnico
- Há escassez de análises sobre:
  - Impacto técnico das avaliações;
  - Efeitos de viés sobre novos profissionais;
  - Exclusão digital algorítmica.
    
#### c) Desenho centrado no usuário (UX técnico)
- Escassez de estudos sobre:
  - Usabilidade de apps para profissionais;
  - Acessibilidade;
  - Jornada de navegação.
    
#### d) Segurança e integridade de dados
- Faltam estudos técnicos sobre:
  - Proteção de dados pessoais;
  - Histórico de pagamentos e avaliações;
  - Geolocalização e privacidade.
    
#### e) Interoperabilidade e APIs públicas
- A maioria das plataformas opera em sistemas fechados;
- Pouca discussão sobre:
  - Integração com ERPs e CRMs;
  - Disponibilidade de APIs públicas/documentadas para terceiros.