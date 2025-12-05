# 5. PLANO DE TESTES DE SOFTWARE
   
### 5.1 Teste de Funcionalidade

O teste de funcionalidade de software verifica se o sistema executa corretamente as funções para as quais foi projetado, de acordo com os requisitos definidos. Envolve a criação e execução de casos de teste que simulam situações reais de uso, comparando os resultados obtidos com os esperados. Falhas identificadas são registradas e corrigidas, e os testes são repetidos para garantir que o software atenda às especificações e funcione de maneira confiável para o usuário.

### 5.1.1 Teste de funcionalidade com usuário Cliente  

|  |  |  |
|--------------------|------------------------------------|----------------------------------------|
|Caso de Teste	| CT01 - Cadastrar usuário do tipo Cliente |
|Pré-Condições	| O usuário deve ter acesso à internet |
|Procedimento | 1) O ator acessa a tela de Login/Cadastro por meio dos botões iniciais “Entrar”, “Encontrar Profissionais”, “Sou Prestador” ou “Começar agora; 2) O ator informa dados válidos no campo “Nome Completo”, ”Email”, cria uma senha, seleciona o tipo Cliente de usuário e clica no botão “Criar Conta”; 3) O sistema carrega a tela inicial com as funcionalidades para Cliente;  | 
|Resultado esperado | O sistema deve retornar a tela de perfil do usuário Cliente. | 
|Dados de entrada | Facilidade na consulta de clientes indicados | 
|Prioridade | Alta |
|Técnica | Manual | 
|Interação | 1ª interação |  

<br><br>

|  |  |  |
|--------------------|------------------------------------|----------------------------------------|
|Caso de Teste	| CT02 - Buscar profissionais |
|Pré-Condições	| O usuário deve ter acesso à internet e estar cadastrado no sistema. |
|Procedimento | 1) O ator acessa a tela de Login por meio dos botões iniciais “Entrar”, “Encontrar Profissionais”, “Sou Prestador” ou “Começar agora; 2) O ator informa dados válidos no campo ”Email” e clica no botão “Entrar”;  3) O sistema carrega a tela inicial com as funcionalidades para Cliente; 4)  O ator clica no botão “Buscar Agora” na área “Buscar Profissionais”; 5) O ator pesquisa pelo prestador de serviço, escrevendo no campo de busca e esperando o sistema retornar; 6) O sistema retorna o prestador de serviços desejado;  | 
|Resultado esperado | O sistema deve retornar uma lista de prestadores de serviços. | 
|Dados de entrada | O usuário deve inserir palavras-chave na barra de pesquisa, para encontrar o prestador de serviços correto. | 
|Prioridade | Alta |
|Técnica | Manual | 
|Interação | 2ª interação |  

<br><br>

|  |  |  |
|--------------------|------------------------------------|----------------------------------------|
|Caso de Teste	| CT03 - Solicitar Serviços |
|Pré-Condições	| O usuário deve ter acesso à internet e estar cadastrado no sistema. |
|Procedimento | 1) O ator acessa a tela de Login por meio dos botões iniciais “Entrar”, “Encontrar Profissionais”, “Sou Prestador” ou “Começar agora; 2) O ator informa dados válidos no campo ”Email” e clica no botão “Entrar”;  3) O sistema carrega a tela inicial com as funcionalidades para Cliente; 4)  O ator clica no botão “Buscar Agora” na área “Buscar Profissionais”; 5) O ator pesquisa pelo prestador de serviço, escrevendo no campo de busca e esperando o sistema retornar; 6) O sistema retorna o prestador de serviços desejado; 7) O ator solicita o serviço do prestador no botão “Solicitar Serviço”; 8) O sistema carrega a tela de detalhes da solicitação de serviço; 9) O ator preenche os campos “Categoria do Serviço”, “Título do Serviço”, “Descrição Detalhada” e “Data Desejada”; 10) O ator finaliza o preenchimento e envia a solicitação através do botão “Enviar Solicitação”; 11) O sistema registra a solicitação do ator em “Minhas Solicitações”.  | 
|Resultado esperado | O sistema deve registrar a solicitação de serviços. | 
|Dados de entrada | O usuário deve preencher os campos da tela de solicitação de serviços. | 
|Prioridade | Alta |
|Técnica | Manual | 
|Interação | 3ª interação |  

### 5.1.2 Teste de funcionalidade com usuário Prestador de Serviços  

|  |  |  |
|--------------------|------------------------------------|----------------------------------------|
|Caso de Teste	| CT04 - Cadastrar usuário do tipo Prestador |
|Pré-Condições	| O usuário deve ter acesso à internet |
|Procedimento | 1) O ator acessa a tela de Login por meio dos botões iniciais “Entrar”, “Encontrar Profissionais”, “Sou Prestador” ou “Começar agora; 2) O ator informa dados válidos no campo “Nome Completo”, ”Email”, cria uma senha, seleciona o tipo Cliente de usuário e clica no botão “Criar Conta”; 3) O sistema carrega a tela inicial com as funcionalidades para Prestador; | 
|Resultado esperado | O sistema deve retornar a tela de perfil do usuário Prestador de Serviços. | 
|Dados de entrada | O usuário deve inserir seu nome completo, email e criar uma senha. | 
|Prioridade | Alta |
|Técnica | Manual | 
|Interação | 1ª interação |  

<br><br>

|  |  |  |
|--------------------|------------------------------------|----------------------------------------|
|Caso de Teste	| CT05 - Preencher perfil de Prestador de Serviços |
|Pré-Condições	| O usuário deve ter acesso à internet e estar cadastrado no sistema. |
|Procedimento | 1) O ator acessa a tela de Login por meio dos botões iniciais “Entrar”, “Encontrar Profissionais”, “Sou Prestador” ou “Começar agora; 2) O ator informa dados válidos no campo ”Email” e clica no botão “Entrar”;  3) O sistema carrega a tela inicial com as funcionalidades para Prestador; 4) O ator clica no botão “Editar Perfil” na área “Meu Perfil”; 5) O sistema retorna a tela de informações pessoais; 6) O ator preenche a tela Informações Pessoais nos campos “Nome Completo”, “Email”, “Telefone” “Localização” e “Sobre Você” com dados válidos e seus serviços prestados; 7) O ator salva as informações clicando em “Salvar Alterações”. | 
|Resultado esperado | O sistema deve retornar a tela de perfil do usuário Prestador de Serviços. | 
|Dados de entrada | O usuário deve preencher seus dados de perfil e seus serviços prestados. | 
|Prioridade | Alta |
|Técnica | Manual | 
|Interação | 2ª interação |  

<br><br>

|  |  |  |
|--------------------|------------------------------------|----------------------------------------|
|Caso de Teste	| CT06 - Visualizar solicitações de clientes |
|Pré-Condições	| O usuário deve ter acesso à internet e estar cadastrado no sistema. |
|Procedimento | 1) O ator acessa a tela de Login por meio dos botões iniciais “Entrar”, “Encontrar Profissionais”, “Sou Prestador” ou “Começar agora; 2) O ator informa dados válidos no campo ”Email” e clica no botão “Entrar”; 3) O sistema carrega a tela inicial com as funcionalidades para Prestador; 4) O ator clica no botão “Ver pedidos” na área “Solicitações Recebidas”; 5) O sistema retorna a tela de Pedidos Recebidos, listando os pedidos dos clientes. | 
|Resultado esperado | O sistema deve retornar a tela pedidos recebidos. | 
|Dados de entrada | Não é necessário dados de entrada. | 
|Prioridade | Alta |
|Técnica | Manual | 
|Interação | 3ª interação |  

### 5.2 Teste de usabilidade  

O teste de usabilidade avalia a facilidade com que os usuários conseguem interagir com um software ou sistema, verificando se ele é intuitivo, eficiente e satisfatório de usar. Durante o teste, usuários reais realizam tarefas específicas enquanto observadores registram dificuldades, erros e percepções sobre a interface. O objetivo é identificar problemas de navegação, compreensão ou ergonomia, permitindo ajustes que tornem o sistema mais acessível, agradável e eficiente para o público-alvo.  

### 5.2.1 Teste de usabilidade com usuário Cliente  

|  |  |  |
|--------------------|------------------------------------|----------------------------------------|
|Caso de Teste	| CT07 - Navegar na tela principal do perfil Cliente. Acessar a tela de busca por profissionais, buscar um perfil de prestador e realizar uma solicitação. |
|Pré-Condições	| O usuário deve ter acesso à internet e estar cadastrado no sistema. |
|Procedimento | 1) O ator acessa a tela de Login por meio dos botões iniciais “Entrar”, “Encontrar Profissionais”, “Sou Prestador” ou “Começar agora; 2) O ator informa dados válidos no campo ”Email” e clica no botão “Entrar”; 3) O sistema carrega a tela inicial com as funcionalidades para Cliente; 4)  O ator clica no botão “Buscar Agora” na área “Buscar Profissionais”; 5) O ator pesquisa pelo prestador de serviço, escrevendo no campo de busca e esperando o sistema retornar; 6) O sistema retorna o prestador de serviços desejado; 7) O ator solicita o serviço do prestador no botão “Solicitar Serviço”; 8) O sistema carrega a tela de detalhes da solicitação de serviço; 9) O ator preenche os campos “Categoria do Serviço”, “Título do Serviço”, “Descrição Detalhada” e “Data Desejada”; 10) O ator finaliza o preenchimento e envia a solicitação através do botão “Enviar Solicitação”; 11) O sistema registra a solicitação do ator em “Minhas Solicitações”; 12) O ator retorna para a tela inicial do perfil; 13) O ator clica no botão “Ver Solicitações” na área “Minhas Solicitações”; 14) O sistema retorna todas as solicitações feitas pelo usuário Cliente. | 
|Resultado esperado | O sistema deve retornar a tela pedidos recebidos. | 
|Dados de entrada | Não é necessário dados de entrada. | 
|Prioridade | Alta |
|Técnica | Manual | 
|Interação | 1ª interação |  

### 5.2.1 Teste de usabilidade com usuário Prestador de Serviços  

|  |  |  |
|--------------------|------------------------------------|----------------------------------------|
|Caso de Teste	| CT08 - Navegar na tela principal do perfil Prestador. Acessar a tela de Solicitações Recebidas, acessar e alterar a tela de Meu Perfil. |
|Pré-Condições	| O usuário deve ter acesso à internet e estar cadastrado no sistema. |
|Procedimento | 1) O ator acessa a tela de Login por meio dos botões iniciais “Entrar”, “Encontrar Profissionais”, “Sou Prestador” ou “Começar agora; 2) O ator informa dados válidos no campo ”Email” e clica no botão “Entrar”; 3) O sistema carrega a tela inicial com as funcionalidades para Prestador; 4) O ator clica no botão “Editar Perfil” na área “Meu Perfil”; 5) O sistema retorna a tela de informações pessoais; 6) O ator preenche a tela Informações Pessoais nos campos “Nome Completo”, “Email”, “Telefone” “Localização” e “Sobre Você” com dados válidos e seus serviços prestados; 7) O ator salva as informações clicando em “Salvar Alterações”; 8) O ator retorna para a página de principal do perfil; 9) O ator clica no botão “Ver pedidos” na área “Solicitações Recebidas”; 10) O sistema retorna a tela de Pedidos Recebidos, listando os pedidos dos clientes. | 
|Resultado esperado | O sistema deve retornar a tela pedidos recebidos. | 
|Dados de entrada | Não é necessário dados de entrada. | 
|Prioridade | Alta |
|Técnica | Manual | 
|Interação | 1ª interação |

<br><br>

[Avaliacao_Heuristica.xlsx](https://github.com/user-attachments/files/23963607/Avaliacao_Heuristica.1.xlsx)

[Teste_Carlos_Cliente.docx](https://github.com/user-attachments/files/23963622/Teste_Carlos_Cliente.docx)

[Teste_Carlos_Prestador.docx](https://github.com/user-attachments/files/23963625/Teste_Carlos_Prestador.docx)

[Relatório de Teste com Usuário - Leandro.docx](https://github.com/user-attachments/files/23963630/Relatorio.de.Teste.com.Usuario.-.Leandro.docx)
