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
| RF1 | Gestão de Conta de Usuário | O sistema deverá permitir que tanto prestadores de serviços quanto clientes se cadastrem na plataforma fornecendo informações essenciais, como nome, e-mail, telefone e tipo de usuário (prestador ou cliente) e façam gestão de suas contas. |
| RF2 |	Recuperação de Senha	|  O sistema deverá permitir que tanto prestadores de serviços quanto clientes se cadastrem na plataforma fornecendo informações essenciais, como nome, e-mail, telefone e tipo de usuário (prestador ou cliente). |
| RF3	| Gestão de serviço prestado  |	O sistema deverá permitir adicionar serviço prestado e atualizar seu progresso, tanto pelo prestador quanto pelo cliente |
| RF4 |	Avaliação de serviço prestado | Após a conclusão do serviço, tanto o cliente quanto o prestador poderão avaliar a experiênci final |
| RF5 | Pesquisa por prestador de serviço | O sistema deverá oferecer filtros para que o cliente refine sua busca, como faixa de preço, avaliação do prestador, e disponibilidade. |
| RF6 | Gestão de Indicações | O sistema deve permitir que clientes e prestadores indiquem um ao outro, editem ou removam suas indicações |

### 3.3.2 Requisitos Não Funcionais

| Código | Requisito Não Funcional (Restrição) |
|--------------------|------------------------------------|
| RNF1 | A plataforma deve ser disponibilizada para acesso web |
| RNF2 | A plataforma deve ser responsiva, mantendo-se compatível com dispositivos mobile e dektop |
| RNF3 | A plataforma deve apresentar uma interface de usuário simples e intuitiva. |
| RNF4 | A navegação deve ser simplificada para tornar a busca por serviços, agendamentos e comunicação mais intuitiva, com menus claros e bem estruturados. |
| RNF5 | A plataforma deve ser totalmente compatível com a Lei Geral de Proteção de Dados (LGPD), garantindo que todos os dados pessoais dos usuários sejam tratados de maneira transparente e segura. |
| RNF6 |O produto deve restringir o acesso por meio de senhas individuais para o usuário. |

### 3.3.3 Usuários 

| Ator | Descrição |
|--------------------|------------------------------------|
| Prestadores de serviços |	Profissionais que oferecem seus serviços sem vínculos empregatícios formais. |
| Clientes  |	Contratam os serviços dos prestadores autônomos. |

## 3.4 Modelagem do Sistema

### 3.4.1 Diagrama de Casos de Uso
Como observado no diagrama de casos de uso da Figura 1, a secretária poderá gerenciar as matrículas e professores no sistema, enquanto o coordenador, além dessas funções, poderá gerenciar os cursos de aperfeiçoamento.

#### Figura 1: Diagrama de Casos de Uso do Sistema.

![dcu](https://github.com/user-attachments/assets/41f6b731-b44e-43aa-911f-423ad6198f47)
 
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
