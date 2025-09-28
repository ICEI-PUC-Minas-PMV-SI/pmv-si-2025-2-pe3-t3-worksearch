# 3. DOCUMENTO DE ESPECIFICAÇÃO DE REQUISITOS DE SOFTWARE

## 3.1 Objetivos deste documento

Descrever e especificar as necessidades dos Prestadores de Serviço e Clientes que devem ser atendidas pelo sistema UaiWork.

## 3.2 Escopo do produto

### 3.2.1 Nome do produto e seus componentes principais

O produto será nomeado "UaiWork", nome escolhido como trocadilho entre o termo "Uai" em português e "Why" em inglês, voltado para conectar prestadores de serviço e clientes.

Ele terá:

(1) Módulo de usuários, com elementos necessários para gestão de cadastrados de ambos os tipos (prestador de serviço e cliente)
(2) Módulo de serviços prestados, com elementos necessários para gestão de progresso dos serviços, comentários e avaliações dos serviços por todos os usuários envolvidos
(3) Módulo de indicação de usuários, com elementos necessários para que prestadores e clientes indiquem um ao outro

### 3.2.2 Missão do produto

Fornecer uma conexão justa e funcional entre clientes e prestadores de serviço, focando no serviço prestado como ele é na realidade. Proporcionar um ambiente colaborativo entre prestadores e clientes.

### 3.2.3 Limites do produto

O UaiWork não realiza gestão de pagamentos ou integração com gateways de terceiros. O UaiWork não realiza suporte ao cliente sobre o serviço do prestador.

### 3.2.4 Benefícios do produto

| # | Benefício | Valor para o Cliente |
|--------------------|------------------------------------|----------------------------------------|
|1	| Facilidade no cadastro de serviço prestado |	Essencial |
|2	| Facilidade no cadastro de progresso do serviço prestado |	Essencial |
|3 | Facilidade na consulta de prestadores disponíveis | Essencial | 
|4 | Facilidade na consulta de prestadores indicados | Essencial | 
|5 | Facilidade na consulta de clientes indicados | Essencial | 
|6 | Segurança das informações sobre o serviço prestado tanto do cliente quanto do prestador | Essencial | 
|7 | Comunicação direta entre prestadores e cliente | Recomendável | 

## 3.3 Descrição geral do produto

### 3.3.1 Requisitos Funcionais

| Código | Requisito Funcional (Funcionalidade) | Descrição |
|--------------------|------------------------------------|----------------------------------------|
| RF1 | Cadastro de usuário |  O sistema deverá permitir que tanto prestadores de serviços quanto clientes se cadastrem na plataforma fornecendo informações essenciais, como nome, e-mail, telefone e tipo de usuário (prestador ou cliente). |
| RF2 | Autenticação de usuário  | O sistema deverá permitir que usuários previamente cadastrados realizem login utilizando suas credenciais (usuário/e-mail e senha) e gerenciem os dados da sua conta. Isso inclui a inclusão de novas contas, remoção de contas existentes, alteração de dados cadastrais e consulta de informações do usuário. |
| RF3 |	Recuperação de senha	|  O sistema deverá permitir que os usuários recuperem suas senhas em caso de esquecimento.  |
| RF4 | Sistema de verificação | O sistema poderá permitir a verificação de identidade (via documentos ou biometria) para aumentar a confiança na plataforma. |
| RF5  |  Pesquisa de prestadores de serviço | O cliente poderá buscar prestadores de serviço baseados em palavras-chave, categorias de serviços, localização e avaliações de outros clientes.
| RF6 | Solicitação de serviço | O cliente poderá enviar uma solicitação de serviço para um prestador específico. |
| RF7 | Aceitação ou recusa da solicitação | O prestador poderá aceitar ou recusar a solicitação de serviço enviada pelo cliente. |
| RF8 | Comunicação Direta |  O sistema deverá permitir que cliente e prestador de serviço se comuniquem por meio de chat ou mensagens dentro da plataforma antes de formalizar o acordo.
| RF9 | Sistema de avaliação de serviço | Após a conclusão do serviço, tanto o cliente quanto o prestador poderão avaliar a experiência por meio de uma nota (1 a 5 estrelas) e um comentário. |
| RF10 | Exibição de avaliações | As avaliações do cliente serão visíveis para futuros clientes, e as avaliações dos prestadores de serviço serão visíveis para outros prestadores ou usuários. |
| RF11 | Sistema de feedback construtivo |  O sistema permitirá que o cliente forneça feedback construtivo diretamente ao prestador, sem prejudicar a imagem pública do prestador de serviço. |
| RF12 | Notificações | O sistema deverá notificar os usuários sempre que uma nova solicitação for feita, ou quando um prestador aceitar ou recusar uma solicitação. |
| RF13	| Gestão de serviço prestado  |	O sistema deverá permitir adicionar serviço prestado e atualizar seu progresso, tanto pelo prestador quanto pelo cliente |
| RF14 | Gestão de Indicações | O sistema deve permitir que clientes e prestadores indiquem um ao outro, editem ou removam suas indicações |

### 3.3.2 Requisitos Não Funcionais

| Código | Requisito Não Funcional |
|--------------------|------------------------------------|
| RNF1 | A plataforma deverá ser acessível em diferentes dispositivos, como desktops, smartphones e tablets, garantindo uma boa experiência de uso em qualquer tipo de tela.  |
| RNF2 | A plataforma deve ser capaz de processar requisições (como busca de prestadores de serviço ou envio de solicitações) em até 3 segundos, em média.
| RNF3 | O sistema deverá ser escalável para suportar picos de acesso de usuários simultâneos sem degradação significativa de desempenho. 
| RNF4 | A plataforma deve ser totalmente compatível com a Lei Geral de Proteção de Dados (LGPD), garantindo que todos os dados pessoais dos usuários sejam tratados de maneira transparente e segura. |


### 3.3.3 Usuários 

| Ator | Descrição |
|--------------------|------------------------------------|
| Prestadores de serviços |	Profissionais que oferecem seus serviços sem vínculos empregatícios formais. |
| Clientes  |	Contratam os serviços dos prestadores autônomos. |

## 3.4 Modelagem do Sistema

### 3.4.1 Diagrama de Casos de Uso

#### Figura 2: Diagrama de Casos de Uso do Sistema CSU01.

<img width="1818" height="742" alt="01" src="https://github.com/user-attachments/assets/7202863c-c09f-4212-823e-0bd53b35bfc4" />


#### Figura 3: Diagrama de Casos de Uso do Sistema CSU02 e CSU03.

<img width="1417" height="491" alt="02-03" src="https://github.com/user-attachments/assets/49fc2b96-3352-436f-b2d8-64e91a78aa56" />


#### Figura 4: Diagrama de Casos de Uso do Sistema CSU04.

<img width="2273" height="424" alt="04" src="https://github.com/user-attachments/assets/7020c61a-5c3d-4495-9cbb-e1c61d8757ab" />

#### Figura 5: Diagrama de Casos de Uso do Sistema CSU05.

<img width="2902" height="424" alt="05" src="https://github.com/user-attachments/assets/a0b5cc4b-0fbd-4b9c-a919-c816b63cbcef" />

#### Figura 6: Diagrama de Casos de Uso do Sistema CSU06.

<img width="1753" height="424" alt="06" src="https://github.com/user-attachments/assets/20f90a26-1d16-4be9-ab6f-baab6f81d0cc" />

#### Figura 7: Diagrama de Casos de Uso do Sistema CSU07.

<img width="1918" height="424" alt="07" src="https://github.com/user-attachments/assets/9c129d6d-7a1a-4515-80cb-e862e636e83b" />

#### Figura 8: Diagrama de Casos de Uso do Sistema CSU08.

<img width="1918" height="424" alt="08" src="https://github.com/user-attachments/assets/c6dea607-930a-4271-89e5-2ed878057c6a" />

#### Figura 9: Diagrama de Casos de Uso do Sistema CSU09.

<img width="1218" height="424" alt="09" src="https://github.com/user-attachments/assets/9b8b61f9-499e-4a6f-820c-7835a8e7ea5c" />

#### Figura 10: Diagrama de Casos de Uso do Sistema CSU010.

<img width="1717" height="512" alt="10" src="https://github.com/user-attachments/assets/be3dcbc0-8ac3-4341-a828-1fd5b534979a" />

#### Figura 11: Diagrama de Casos de Uso do Sistema CSU013.

<img width="1127" height="424" alt="13" src="https://github.com/user-attachments/assets/2c2e4704-5c57-4196-bb2f-f1625a1b2687" />

#### Figura 12: Diagrama de Casos de Uso do Sistema CSU014.

<img width="1184" height="424" alt="14" src="https://github.com/user-attachments/assets/e1b9ee72-5dca-4d91-b900-d7e5a56a5026" />

#### Figura 13: Diagrama de Casos de Uso do Sistema CSU015.

<img width="1218" height="424" alt="15" src="https://github.com/user-attachments/assets/98a14851-a40b-4c3a-8188-c103c66144b6" />


### 3.4.2 Descrições de Casos de Uso

| **Cadastrar Usuário (CSU01)** |
|-------------------------------|
| **Sumário:** O usuário se cadastra na plataforma para poder acessar as funcionalidades de busca, contratação e prestação de serviços. |
| **Atores:** Usuário (cliente ou prestador). |
| **Pré-condições:** O sistema deve estar disponível e acessível ao usuário que deseja se cadastrar. |
| **Fluxo Principal:** |
| 1. O usuário acessa a página inicial da plataforma. |
| 2. O usuário escolhe entre se cadastrar como prestador de serviço ou cliente. |
| 3. O Sistema apresenta uma janela com formulário de cadastro. |
| 4. O usuário preenche o formulário de cadastro com informações básicas, como nome, e-mail, telefone e senha. |
| 5. O sistema envia um link de confirmação para o e-mail informado. |
| **Fluxos Alternativos:** |
| 1. Se o usuário tentar se cadastrar com um e-mail já registrado, o sistema informa que o e-mail já está em uso e solicita uma nova tentativa. |
| **Pós-condições:** O usuário terá um perfil criado, podendo acessar a plataforma com o login. |

| **Login de Usuário (CSU02)** |
|-------------------------------|
| **Sumário:** O usuário realiza o login e gestão (inclusão, remoção, alteração e consulta) dos dados sobre usuário. |
| **Ator Primário:** Usuário (cliente ou prestador). |
| **Ator Secundário:** Sistema. |
| **Pré-condições:** O usuário já deve ser cadastrado e validado pelo Sistema. |
| **Fluxo Principal:** |
| 1. O usuário requisita o login de usuário. |
| 2. O Sistema apresenta campos de usuário/e-mail e senha para o usuário preencher. |
| 3. O usuário preenche os campos de usuário/e-mail e senha com os respectivos dados. |
| 4. O Sistema verifica a validade dos dados. Se os dados forem válidos, o usuário é autenticado e acessa a conta referente; caso contrário, o Sistema reporta o fato, solicita novos dados e repete a verificação. |
| **Fluxo Alternativo (1) – Inclusão:** |
| 1. O usuário requisita a inclusão de uma nova conta de usuário. |
| 2. O Sistema apresenta uma janela solicitando o e-mail do usuário a ser cadastrado. |
| 3. O usuário fornece o dado solicitado. |
| 4. O Sistema verifica se o usuário já está cadastrado. Se sim, o Sistema reporta o fato e volta ao início; caso contrário, apresenta um formulário em branco para que os detalhes do usuário (Código, Tipo de Usuário, Nome, Endereço, CEP, Estado, Cidade, Bairro, Telefone, Identidade, Sexo, CPF, Data do Cadastro e Descrição) sejam incluídos. |
| 5. O usuário fornece os detalhes da nova conta de usuário. |
| 6. O Sistema verifica a validade dos dados. Se os dados forem válidos, inclui o novo usuário e a tabela do banco de dados de usuários é atualizada; caso contrário, o Sistema reporta o fato, solicita novos dados e repete a verificação. |
| **Fluxo Alternativo (2) – Remoção:** |
| 1. O usuário seleciona a opção “Excluir conta” e requisita ao Sistema que o remova. |
| 2. O Sistema mostra uma tela de confirmação de remoção. |
| 3. O usuário confirma a remoção da conta. |
| 4. O Sistema realiza a remoção da conta. |
| **Fluxo Alternativo (3) – Alteração:** |
| 1. O usuário altera um ou mais dos detalhes na conta de usuário e requisita ao sistema a sua atualização. |
| 2. O Sistema verifica a validade dos dados e, se eles forem válidos, altera os dados na tabela de usuários no banco de dados; caso contrário, o erro é reportado. |
| **Fluxo Alternativo (4) – Consulta:** |
| 1. O usuário solicita a consulta sobre a conta de usuário. |
| 2. O Sistema apresenta uma tela contendo informações detalhadas sobre a conta de usuário. |
| **Pós-condições:** Um usuário foi inserido ou removido, seus dados foram alterados ou apresentados na tela. |

| **Autenticação de Usuário (CSU03)** |
|-------------------------------------|
| **Sumário:** Permite que o usuário acesse a plataforma por meio de uma autenticação de e-mail e senha. |
| **Ator Primário:** Usuário (cliente ou prestador). |
| **Ator Secundário:** Sistema. |
| **Pré-condições:** O usuário já deve ser cadastrado e validado pelo Sistema. |
| **Fluxo Principal:** |
| 1. O usuário acessa a tela de login. |
| 2. Informa e-mail e senha de usuário válidos. |
| 3. O sistema valida as credenciais; se forem válidas, o usuário é autenticado e redirecionado para o painel principal; caso contrário, o sistema reporta o fato, solicita novos dados e repete a verificação. |
| **Pós-condições:** O usuário é autenticado na plataforma. |

| **Recuperação de Senha (CSU04)** |
|----------------------------------|
| **Sumário:** Permite que os usuários recuperem o acesso em caso de esquecimento de senha. |
| **Ator Primário:** Usuário. |
| **Ator Secundário:** Sistema. |
| **Pré-condições:** O usuário já deve ser cadastrado e validado pelo Sistema. |
| **Fluxo Principal:** |
| 1. O usuário seleciona “Esqueci minha senha”, requisitando uma redefinição de senha para o sistema. |
| 2. O usuário informa o e-mail da conta para o sistema. |
| 3. Caso o e-mail seja cadastrado no sistema, o sistema envia um link para redefinição de senha, o usuário acessa o link e cria uma nova senha; caso contrário, o sistema exibe uma mensagem de erro. |
| **Pós-condições:** O usuário possui uma nova senha ativa para login. |

| **Sistema de Verificação (CSU05)** |
|------------------------------------|
| **Sumário:** Permite aumentar a confiança da plataforma por meio da verificação de identidade. |
| **Ator Primário:** Usuário (cliente ou prestador). |
| **Ator Secundário:** Serviço externo de validação de documento/biometria. |
| **Pré-condições:** O usuário já deve ser cadastrado e validado pelo Sistema. |
| **Fluxo Principal:** |
| 1. O usuário solicita a verificação de identidade. |
| 2. O usuário envia os documentos ou realiza a biometria. |
| 3. O sistema encaminha os dados para a validação. |
| 4. A validação é concluída e o status “Verificado” é atualizado no perfil do usuário; caso os dados não sejam validados, o sistema informa a rejeição e solicita nova tentativa. |
| **Pós-condições:** O usuário passa a ter o perfil marcado como “Verificado”. |

| **Pesquisar por Prestadores de Serviço (CSU06)** |
|--------------------------------------------------|
| **Sumário:** O cliente pesquisa por prestadores de serviço dentro de uma categoria específica, usando filtros como localização, avaliação e preço. |
| **Atores:** Cliente |
| **Pré-condições:** O cliente já deve ser cadastrado e validado pelo Sistema. |
| **Fluxo Principal:** |
| 1. O cliente acessa a página de pesquisa de serviços. |
| 2. O cliente insere palavras-chave ou seleciona filtros (categoria, localização, preço, disponibilidade etc.). |
| 3. O sistema exibe a lista de prestadores de serviço que atendem aos critérios definidos pelo cliente. |
| 4. O cliente visualiza os perfis dos prestadores de serviço e escolhe um para entrar em contato. |
| **Fluxo Alternativo:** |
| 1. Se não houver prestadores que atendem aos filtros, o sistema exibirá uma mensagem informando que não há resultados para os critérios selecionados. |
| **Pós-condições:** O resultado da pesquisa de prestadores é exibido para o cliente. |

| **Solicitar Serviço (CSU07)** |
|-------------------------------|
| **Sumário:** O cliente solicita um serviço de um prestador de serviço, podendo especificar detalhes sobre o trabalho. |
| **Atores:** Cliente, prestador de serviço |
| **Pré-condições:** O cliente deve estar logado. |
| **Fluxo Principal:** |
| 1. O cliente visualiza o perfil do prestador de serviço escolhido. |
| 2. O cliente clica no botão "Solicitar serviço". |
| 3. O cliente preenche os detalhes do serviço (descrição, data, localização, dentre outros). |
| 4. O prestador recebe a notificação da solicitação e tem a opção de aceitar ou recusar. |
| 5. Se o prestador aceitar, o cliente é notificado, e ambos podem comunicar-se. |
| **Fluxo Alternativo:** |
| 1. Se o prestador recusar, o cliente será notificado e poderá procurar outro prestador de serviço. |
| **Pós-condições:** A solicitação de serviço foi enviada ao prestador de serviço, e ambos podem começar a se comunicar. |

| **Aceitação ou Recusa da Solicitação (CSU08)** |
|------------------------------------------------|
| **Sumário:** Permite que o prestador aceite ou recuse uma solicitação recebida. |
| **Ator Primário:** Prestador de serviço. |
| **Ator Secundário:** Cliente. |
| **Pré-condições:** O prestador deve estar autenticado e ter recebido a solicitação. |
| **Fluxo Principal:** |
| 1. O prestador acessa a lista de solicitações. |
| 2. O prestador visualiza os detalhes da solicitação. |
| 3. O prestador aceita ou recusa a solicitação; caso contrário, se o prazo definido de resposta for ultrapassado, a mensagem é marcada como expirada. |
| **Pós-condições:** A solicitação é atualizada com status de aceita ou recusada. |

| **Comunicação Direta (CSU09)** |
|--------------------------------|
| **Sumário:** Permite interação entre cliente e prestador via chat interno. |
| **Ator Primário:** Cliente. |
| **Ator Secundário:** Prestador de serviço. |
| **Pré-condições:** Ambos (prestador e cliente) devem estar autenticados. |
| **Fluxo Principal:** |
| 1. Cliente ou prestador acessa o chat da solicitação. |
| 2. Cliente ou prestador envia mensagens. |
| 3. O sistema registra e exibe as mensagens em tempo real caso a conexão esteja estável; caso contrário, o sistema exibe erro de envio da mensagem. |
| **Pós-condições:** Histórico de mensagens armazenado na solicitação. |

| **Avaliar Serviço (CSU10)** |
|-----------------------------|
| **Sumário:** Após a conclusão do serviço, o cliente avalia o prestador de serviço com uma nota. |
| **Atores:** Cliente |
| **Pré-condições:** O serviço deve ter sido concluído. |
| **Fluxo Principal:** |
| 1. O cliente acessa o serviço concluído no seu histórico de serviços. |
| 2. O cliente seleciona a opção para avaliar o prestador. |
| 3. O cliente atribui uma nota de 1 a 5 estrelas. |
| 4. O sistema registra a avaliação e a exibe no perfil do prestador de serviço. |
| **Fluxo Alternativo:** |
| 1. Se o cliente não quiser deixar uma avaliação, ele pode optar por não avaliar o serviço. |
| **Pós-condições:** A avaliação do cliente é registrada no sistema e fica disponível para futuros clientes. |

| **Exibição de Avaliações (CSU11)** |
|-----------------------------------|
| **Sumário:** Permite exibição pública de avaliações entre clientes e prestadores. |
| **Ator Primário:** Cliente e Prestador. |
| **Ator Secundário:** Sistema. |
| **Pré-condições:** O serviço deve estar concluído. |
| **Fluxo Principal:** |
| 1. O usuário acessa o perfil de cliente ou prestador. |
| 2. O sistema exibe as avaliações públicas (comentários e notas). |
| 3. O usuário seleciona uma nota para o cliente ou prestador. |
| 4. O usuário insere um comentário público e envia. |
| **Pós-condições:** Avaliações ficam disponíveis para a consulta de todos os usuários. |

| **Sistema de Feedback Construtivo (CSU12)** |
|---------------------------------------------|
| **Sumário:** Permite feedback construtivo privado entre clientes e prestadores. |
| **Ator Primário:** Cliente e Prestador. |
| **Ator Secundário:** Sistema. |
| **Pré-condições:** O serviço deve estar concluído. |
| **Fluxo Principal:** |
| 1. O usuário acessa o perfil de cliente ou prestador. |
| 2. O sistema exibe as avaliações públicas (comentários e notas). |
| 3. O usuário seleciona a opção de enviar um feedback. |
| 4. O usuário insere um comentário e envia. |
| **Pós-condições:** A avaliação de feedback privado aparece para o usuário designado. |

| **Notificações (CSU13)** |
|---------------------------|
| **Sumário:** Garante que usuários sejam notificados sobre solicitações e respostas. |
| **Ator Primário:** Sistema. |
| **Ator Secundário:** Cliente ou Prestador. |
| **Pré-condições:** O serviço deve estar concluído. |
| **Fluxo Principal:** |
| 1. O sistema detecta um evento (nova solicitação, aceitação ou recusa). |
| 2. O sistema envia uma notificação ao usuário correspondente. |
| **Pós-condições:** Usuário informado sobre mudanças relevantes. |

| **Gestão de Serviço Prestado (CSU14)** |
|----------------------------------------|
| **Sumário:** Permite acompanhar e atualizar o andamento do serviço. |
| **Ator Primário:** Prestador de serviço. |
| **Ator Secundário:** Cliente. |
| **Pré-condições:** Serviço deve ter sido aceito pelo prestador ou cliente. |
| **Fluxo Principal:** |
| 1. O prestador acessa o painel de serviços. |
| 2. O prestador atualiza status (ex.: iniciado, em andamento, concluído). |
| 3. O cliente acompanha o progresso. |
| **Pós-condições:** Status atualizado refletido no sistema. |

| **Gestão de Indicações (CSU15)** |
|----------------------------------|
| **Sumário:** Permite que clientes e prestadores indiquem, editem ou removam recomendações. |
| **Ator Primário:** Cliente e Prestador. |
| **Ator Secundário:** Cliente ou Prestador. |
| **Pré-condições:** O serviço deve estar concluído. |
| **Fluxo Principal:** |
| 1. O usuário acessa a área de indicações. |
| 2. O usuário registra, edita ou remove uma indicação. |
| 3. O sistema salva a alteração. |
| **Pós-condições:** Indicação é registrada, atualizada ou removida com sucesso. |

### 3.4.3 Diagrama de Classes 

#### Figura 2: Diagrama de Classes do Sistema.

 ![WhatsApp Image 2025-09-28 at 16 41 13 (1)](https://github.com/user-attachments/assets/4e82527f-1a05-461b-aeec-11d30517b26d)


### 3.4.4 Descrições das Classes 

| # | Nome          | Descrição                                                                 |
|---|---------------|---------------------------------------------------------------------------|
| 1 | Usuário       | Representa a entidade principal do sistema, podendo ser cliente ou prestador. Possui informações de cadastro, autenticação e interação na plataforma. |
| 2 | Cliente       | Usuário que solicita serviços na plataforma, podendo avaliar, recomendar e interagir com prestadores. |
| 3 | Prestador     | Usuário que oferece serviços na plataforma, podendo aceitar solicitações, ser avaliado e recomendado. |
| 4 | Serviço       | Entidade que representa o trabalho solicitado e oferecido, gerando avaliações, solicitações e recomendações. |
| 5 | Avaliação     | Registro de feedback público do serviço prestado, contendo nota e comentário visível para outros usuários. |
| 6 | Solicitação   | Pedido de um cliente a um prestador para execução de um serviço específico. Pode ser aceita ou recusada. |
| 7 | Recomendação  | Indicação de confiança entre usuários (clientes ou prestadores), fortalecendo a reputação na plataforma. |
| 8 | Notificação   | Mensagem automática enviada pelo sistema para informar usuários sobre eventos (ex.: nova solicitação, aceitação, recusa). |
| 9 | Chat          | Canal de comunicação direta entre cliente e prestador dentro da plataforma. |
|10 | Mensagem      | Conteúdo de texto enviado dentro do chat, permitindo interação entre cliente e prestador. |
|11 | Indicação     | Registro formal de indicação criada por um usuário sobre outro, reforçando relações de confiança na plataforma. |
