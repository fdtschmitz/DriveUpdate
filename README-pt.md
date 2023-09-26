# DriveUpdate
Implementação simples para a biblioteca PyDrive2. Itere através de uma pasta raiz do Google Drive e retorne uma lista de pastas e arquivos.

# Contexto
A ideia de implementação surgiu da necessidade de criar um índice e atualizado para um repositório publico de livros.

# Antes de Começar
Para que o código funcione é necessário gerar chaves de autenticação no painel do Google Cloud em https://console.cloud.google.com/

Crie um novo projeto, e busque por APIs e Serviços. Antes de gerar a chave você vai precisar configurar a tela de permissão OAuth; Selecione o tipo de usuário. Como estamos utilizando a versão gratuíta só temos acesso a opção Externo. Clique em criar.

Na tela seguinte informe o nome do seu App, o seu email para suporte e o contato do desenvolvedor. Clique em Salvar e continuar. Em Escopo você pode deixar vazio por enquanto.

Na tela de Test users você precisa adicionar os usuários que irão utilizar esse código. Mesmo que seja somente você, é necessário colocar o seu email. Clique em Adicionar Usuário para informar o email. Salve e finalize a configuração.

De volta ao dashboard, vá em Credenciais e clique em Criar Credenciais. Selecione ID do client OAuth. Para este exemplo, selecione Desktop app. Dê um nome para a chave e clique em Criar. Na tela que aparece você vai poder baixar o JSON que iremos utilizar no código. Ele precisa estar na mesma pasta do projeto.

# Pré-requisitos
Este código utiliza a biblioteca PyDrive2. Visite a página do projeto para ver como instalar: https://github.com/iterative/PyDrive2/

Utilizaremos também a biblioteca openpyxl. Documentação em: https://openpyxl.readthedocs.io/
