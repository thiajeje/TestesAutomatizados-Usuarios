Testes de API com Postman

 
📌 Sobre o Projeto

Este projeto foi desenvolvido com o objetivo de praticar testes de API utilizando o Postman.

A API testada é responsável pelo gerenciamento de usuários, permitindo realizar operações de:
- Criar usuário (post)
- Consultar usuário (get)
- Atualizar usuário (put)
- Excluir usuário (delete)

Os testes foram feitos para validar se a API está funcionando corretamente e retornando as respostas esperadas.


🚀 Ferramentas Utilizadas
- Postman
- JavaScript básico para scripts de teste
- GitHub para versionamento e pipeline automatizado

✅ Testes Realizados

👤 Criar Usuário
- Validação do status 201 - Cadastro com sucesso
- Verificação dos dados retornados
- Teste com campos inválidos (email, nome, senha e administrador)

📖 Listar Usuário
- Busca de usuário por ID
- Listagem de usuários
- Validação do status 200 OK
- Teste com ID inexistente e maior e menor que 16 caracteres

✏️ Atualização de Usuário
- Atualização de informações do usuário (email, nome, senha e administrador)
- Verificação se os dados foram alterados corretamente
- Validação do status 400 Bad Request
- Teste com alteração de um email já cadastrado e campos vazios

🗑️ Exclusão de Usuário
- Exclusão de usuário existente
- Validação do status de sucesso
- Teste para excluir usuário inexistente


▶️ Como Executar os Testes
Pelo GitHub
1. Acesse o repositório no GitHub, pelo link:
	https://github.com/thiajeje/TestesAutomatizados-Usuarios.git
2. Clone o repositório
3. Edite o arquivo "execute_tests"
4. Faça o commit e abra um pull request


⚠️ Observações 
1. Para cada collection foi implementado o login antes para salvar o Token na variável "tokenValido".
2. Na collection "Criar Usuário" foi utilizado a variavel "emailRandom" que cria um email randomico para minimizar a possibilidade de dar erro de email já utilizado no teste de sucesso.
3. Na collection "Listar Usuários" foi testado chamar ID's com mais de 16 caracteres e com menos, visto que o ID tem que ter exatamente 16 caracteres no sistema especifico. 
4. Na collection "Atualizar Usuário" foi testado utilizado a variável "emailRandom" ao atualizar o email para testar se um novo usuário iria ser criado utilizando um email inexistente até então. 


📊 Objetivo dos Testes

Os testes foram criados para validar:
- Status das requisições
- Estrutura das respostas
- Funcionamento das operações CRUD
- Garantir 100% de cobertura para a API 


👨‍💻 Autor 
 
Projeto desenvolvido para estudos na área de QA e automação de testes de API.
