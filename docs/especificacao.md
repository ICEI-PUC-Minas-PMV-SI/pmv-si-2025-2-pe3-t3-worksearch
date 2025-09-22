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
| RF2 | Autenticação de usuário | O sistema deverá permitir que os usuários façam login na plataforma através de e-mail e senha ou via autenticação por redes sociais. |
| RF3 |	Recuperação de senha	|  O sistema deverá permitir que os usuários recuperem suas senhas em caso de esquecimento.  |
| RF4 | Sistema de verificação | O sistema poderá permitir a verificação de identidade (via documentos ou biometria) para aumentar a confiança na plataforma. |
| RF5  |  Pesquisa de prestadores de serviço | O cliente poderá buscar prestadores de serviço baseados em palavras-chave, categorias de serviços, localização e avaliações de outros clientes.
| RF6 | Solicitação de serviço | O cliente poderá enviar uma solicitação de serviço para um prestador específico. |
| RF7 | Aceitação ou recusa da solicitação | O prestador poderá aceitar ou recusar a solicitação de serviço enviada pelo cliente. |
| RF8 | Comunicação Direta |  O sistema deverá permitir que cliente e prestador de serviço se comuniquem por meio de chat ou mensagens dentro da plataforma antes de formalizar o acordo.
| RF9 | Métodos de pagamento | --------|
| RF10 | Sistema de avaliação de serviço | Após a conclusão do serviço, tanto o cliente quanto o prestador poderão avaliar a experiência por meio de uma nota (1 a 5 estrelas) e um comentário. |
| RF11 | Exibição de avaliações | As avaliações do cliente serão visíveis para futuros clientes, e as avaliações dos prestadores de serviço serão visíveis para outros prestadores ou usuários. |
| RF12 | Sistema de feedback construtivo |  O sistema permitirá que o cliente forneça feedback construtivo diretamente ao prestador, sem prejudicar a imagem pública do prestador de serviço. |
| RF13 | Notificações | O sistema deverá notificar os usuários sempre que uma nova solicitação for feita, ou quando um prestador aceitar ou recusar uma solicitação. |
| RF14	| Gestão de serviço prestado  |	O sistema deverá permitir adicionar serviço prestado e atualizar seu progresso, tanto pelo prestador quanto pelo cliente |
| RF15 |	Avaliação de serviço prestado | Após a conclusão do serviço, tanto o cliente quanto o prestador poderão avaliar a experiênci final |
| RF16 | Pesquisa por prestador de serviço | O sistema deverá oferecer filtros para que o cliente refine sua busca, como faixa de preço, avaliação do prestador, e disponibilidade. |
| RF17 | Gestão de Indicações | O sistema deve permitir que clientes e prestadores indiquem um ao outro, editem ou removam suas indicações |

### 3.3.2 Requisitos Não Funcionais

| Código | Requisito Não Funcional (Restrição) |
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
Como observado no diagrama de casos de uso da Figura 1, a secretária poderá gerenciar as matrículas e professores no sistema, enquanto o coordenador, além dessas funções, poderá gerenciar os cursos de aperfeiçoamento.

#### Figura 1: Diagrama de Casos de Uso do Sistema.

<img width="1360" height="1760" alt="Image" src="https://github.com/user-attachments/assets/e9d047a3-a2ab-43eb-bdae-4d78250007b1" />

#### Figura 2: Diagrama de Casos de Uso do Sistema.

<img width="1220" height="1020" alt="Image" src="https://github.com/user-attachments/assets/1283db65-22f0-4240-be49-2a306bc58d41" />

#### Figura 3: Diagrama de Casos de Uso do Sistema.

<img width="1299" height="1160" alt="Image" src="https://github.com/user-attachments/assets/de9fc00f-d82c-4dcc-a740-20cb415561b4" />

### 3.4.2 Descrições de Casos de Uso

Cada caso de uso deve ter a sua descrição representada nesta seção. Exemplo:

#### Gerenciar Professor (CSU01)

Sumário: A Secretária realiza a gestão (inclusão, remoção, alteração e consulta) dos dados sobre professores.

Ator Primário: Secretária.

Ator Secundário: Coordenador.

Pré-condições: A Secretária deve ser validada pelo Sistema.

Fluxo Principal:

1) 	A Secretária requisita manutenção de professores.
2) 	O Sistema apresenta as operações que podem ser realizadas: inclusão de um novo professor, alteração de um professor, a exclusão de um professor e a consulta de dados de um professor.
3) 	A Secretária seleciona a operação desejada: Inclusão, Exclusão, Alteração ou Consulta, ou opta por finalizar o caso de uso.
4) 	Se a Secretária desejar continuar com a gestão de professores, o caso de uso retorna ao passo 2; caso contrário o caso de uso termina.

Fluxo Alternativo (3): Inclusão

a)	A Secretária requisita a inclusão de um professor. <br>
b)	O Sistema apresenta uma janela solicitando o CPF do professor a ser cadastrado. <br>
c)	A Secretária fornece o dado solicitado. <br>
d)	O Sistema verifica se o professor já está cadastrado. Se sim, o Sistema reporta o fato e volta ao início; caso contrário, apresenta um formulário em branco para que os detalhes do professor (Código, Nome, Endereço, CEP, Estado, Cidade, Bairro, Telefone, Identidade, Sexo, Fax, CPF, Data do Cadastro e Observação) sejam incluídos. <br>
e)	A Secretária fornece os detalhes do novo professor. <br>
f)	O Sistema verifica a validade dos dados. Se os dados forem válidos, inclui o novo professor e a grade listando os professores cadastrados é atualizada; caso contrário, o Sistema reporta o fato, solicita novos dados e repete a verificação. <br>

Fluxo Alternativo (3): Remoção

a)	A Secretária seleciona um professor e requisita ao Sistema que o remova. <br>
b)	Se o professor pode ser removido, o Sistema realiza a remoção; caso contrário, o Sistema reporta o fato. <br>

Fluxo Alternativo (3): Alteração

a)	A Secretária altera um ou mais dos detalhes do professor e requisita sua atualização. <br>
b)	O Sistema verifica a validade dos dados e, se eles forem válidos, altera os dados na lista de professores, caso contrário, o erro é reportado. <br>
 
Fluxo Alternativo (3): Consulta

a)	A Secretária opta por pesquisar pelo nome ou código e solicita a consulta sobre a lista de professores. <br>
b)	O Sistema apresenta uma lista professores. <br>
c)	A Secretária seleciona o professor. <br>
d)	O Sistema apresenta os detalhes do professor no formulário de professores. <br>

Pós-condições: Um professor foi inserido ou removido, seus dados foram alterados ou apresentados na tela.

#### Cadastrar usuário

O usuário se cadastra na plataforma para poder acessar as funcionalidades de busca, contratação e prestação de serviços. 

Atores: Cliente, prestador de serviço 

Pré-condições: O usuário não deve estar logado no sistema. 

Fluxo Principal:

1) 	O usuário acessa a página inicial da plataforma.
2) 	O usuário escolhe entre se cadastrar como prestador de serviço ou cliente. 
3) 	O usuário preenche o formulário de cadastro com informações básicas, como nome, e-mail, telefone e senha. 
4) 	O sistema envia um link de confirmação para o e-mail informado.

Fluxos Alternativos:

1) Se o usuário tentar se cadastrar com um e-mail já registrado, o sistema informa que o e-mail já está em uso e solicita uma nova tentativa. 
2) Se o usuário esquecer a senha, o sistema oferece a opção de recuperação de senha. 


Pós-condições: O usuário terá um perfil criado, podendo acessar a plataforma com o login. 

#### Recuperar senha
O usuário pode recuperar sua senha caso tenha esquecido. 

Atores: Cliente, prestador de serviço 

Pré-condições: O usuário deve ter um cadastro na plataforma. 

Fluxo Principal: 
1) O usuário clica na opção "Esqueci minha senha" na tela de login.
2) O sistema solicita o e-mail do usuário.
3) O usuário insere o e-mail e o sistema envia um link de recuperação para o endereço informado.
4) O usuário acessa o link e cria uma nova senha.
5) O sistema confirma a alteração e direciona o usuário para a tela de login.

Fluxo Alternativo:
1) Se o e-mail fornecido não estiver registrado, o sistema informa que não há conta associada a esse e-mail.

Pós-condições: O usuário recupera o acesso à plataforma com uma nova senha. 

#### Pesquisar por prestadores de serviço

O cliente pesquisa por prestadores de serviço dentro de uma categoria específica, usando filtros como localização, avaliação e preço.

Atores: Cliente 

Pré-condição: O cliente pode estar logado ou não na plataforma.

Fluxo principal:
1) O cliente acessa a página de pesquisa de serviços.
2) O cliente escolhe uma categoria de serviço.
3) O cliente define filtros de pesquisa, como preço, localização, avaliação dos prestadores e disponibilidade.
4) O sistema exibe a lista de prestadores de serviço que atendem aos critérios definidos pelo cliente.
5) O cliente visualiza os perfis dos prestadores de serviço e escolhe um para entrar em contato.

Fluxo alternativo:
1) Se não houver prestadores que atendem aos filtros, o sistema exibirá uma mensagem informando que não há resultados para os critérios selecionados.

Pós-condições: O cliente pode visualizar os perfis dos prestadores.

#### Solicitar serviço 

O cliente solicita um serviço de um prestador de serviço, podendo especificar detalhes sobre o trabalho.

Atores: Cliente, prestador de serviço 

Pré-condições: O cliente deve estar logado.

Fluxo principal:
1) O cliente visualiza o perfil do prestador de serviço escolhido.
2) O cliente clica no botão "Solicitar serviço".
3) O cliente preenche os detalhes do serviço (descrição, data, localização, dentre outros.)
4) O prestador recebe a notificação da solicitação e tem a opção de aceitar ou recusar.
5) Se o prestador aceitar, o cliente é notificado, e ambos podem comunicar-se.

Fluxo alternativo:
1) Se o prestador recusar, o cliente será notificado e poderá procurar outro prestador de serviço.

Pós-condições: A solicitação de serviço foi enviada ao prestador de serviço, e ambos podem começar a se comunicar.

#### Avaliar serviço

Após a conclusão do serviço, o cliente avalia o prestador de serviço com uma nota.

Atores: Cliente

Pré-condições: O serviço deve ter sido concluído.

Fluxo principal:
1) O cliente acessa o serviço concluído no seu histórico de serviços.
2) O cliente seleciona a opção para avaliar o prestador.
3) O cliente atribui uma nota de 1 a 5 estrelas.
4) O sistema registra a avaliação e a exibe no perfil do prestador de serviço.

Fluxo alternativo:
1) Se o cliente não quiser deixar uma avaliação, ele pode optar por não avaliar o serviço.

Pós-condições: A avaliação do cliente é registrada no sistema e fica disponível para futuros clientes.

### 3.4.3 Diagrama de Classes 

A Figura 2 mostra o diagrama de classes do sistema. A Matrícula deve conter a identificação do funcionário responsável pelo registro, bem com os dados do aluno e turmas. Para uma disciplina podemos ter diversas turmas, mas apenas um professor responsável por ela.

#### Figura 2: Diagrama de Classes do Sistema.
 
![image](https://github.com/user-attachments/assets/abc7591a-b46f-4ea2-b8f0-c116b60eb24e)


### 3.4.4 Descrições das Classes 

| # | Nome | Descrição |
|--------------------|------------------------------------|----------------------------------------|
| 1	|	Aluno |	Cadastro de informações relativas aos alunos. |
| 2	| Curso |	Cadastro geral de cursos de aperfeiçoamento. |
| 3 |	Matrícula |	Cadastro de Matrículas de alunos nos cursos. |
| 4 |	Turma |	Cadastro de turmas.
| 5	|	Professor |	Cadastro geral de professores que ministram as disciplinas. |
| ... |	... |	... |
