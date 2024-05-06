## Comandos Básicos de Configuração do Git

- `git`: Exibe a lista de comandos e opções disponíveis no Git.
- `git config --list`: Mostra todas as configurações do Git, incluindo variáveis de usuário e repositório.
- `git config --local`: Configurações específicas para o repositório atual.
- `git config --global`: Configurações aplicadas a todos os repositórios do usuário no sistema.
- `git config --global user.name "Nome Sobrenome"`: Define o nome do usuário para todos os commits no sistema.
- `git config --global user.email seuemail@email.com`: Define o e-mail do usuário para todos os commits no sistema.
- `git config --global init.defaultBranch main`: Define o nome do branch inicial para novos repositórios como 'main'.
- `git config --global credential.helper cache`: Armazena credenciais na memória por um tempo limitado.
- `git config --global credential.helper store`: Salva as credenciais no disco.

## Comandos de Operação do Repositório

- `git status`: Mostra o estado atual do repositório, arquivos modificados, adicionados, etc.
- `git log`: Exibe o histórico de commits.
- `git reflog`: Exibe um log de suas operações no repositório, como commits e resets.

- `git init`: Inicializa um novo repositório Git.
- `git remote`: Lista os repositórios remotos configurados.
- `git remote add origin [URL]`: Adiciona um novo repositório remoto chamado 'origin'.

- `git clone [URL]`: Clona um repositório remoto para o local.
- `git clone --branch [branch] --single-branch [URL]`: Clona um único branch específico de um repositório.

## Comandos de Gerenciamento de Mudanças

- `git add [arquivos]`: Adiciona arquivos ao próximo commit.
- `git commit`: Confirma as mudanças no repositório.
- `git commit -m"[mensagem]"`: Faz um commit com uma mensagem.
- `git commit --amend -m"[nova mensagem]"`: Altera o último commit.

- `git reset`: Redefine o HEAD para um estado específico.
- `git reset --soft [commit]`: Mantém o estado atual dos arquivos.
- `git reset --mixed [commit]`: Redefine o índice, mas mantém o conteúdo dos arquivos.
- `git reset --hard [commit]`: Redefine tudo para o estado de um commit específico.

## Comandos de Sincronização e Atualização

- `git push`: Envia commits para o repositório remoto.
- `git push -u origin [branch]`: Envia commits para uma branch específica e rastreia a branch.
- `git pull`: Atualiza o repositório local com o repositório remoto.

## Comandos de Restauração

- `git restore [arquivo]`: Desfaz alterações em arquivos não commitados.
- `git reset`: Usado para desfazer mudanças.

## Gerenciamento de Branches e Mesclagem

- `git branch`: Lista todos os branches locais.
- `git checkout -b nova-branch`: Cria e muda para uma nova branch.
- `git branch -d nome-da-branch`: Deleta uma branch.
- `git branch -v`: Lista branches com informações adicionais.
- `git merge [branch]`: Mescla mudanças de uma branch para outra.

## Comandos Avançados

- `git fetch`: Atualiza referências locais com mudanças de um repositório remoto.
- `git diff`: Mostra as diferenças entre commits, branches, etc.

- `git stash`: Guarda mudanças locais temporariamente.
- `git stash list`: Lista as mudanças guardadas.
- `git stash pop`: Aplica a última mudança guardada e remove do stash.
- `git stash apply`: Aplica a última mudança guardada mas mantém no stash.

## Convenções

- **Convenções para nomear branch**: Geralmente utiliza-se nomes como `feature/nome-da-funcionalidade`, `bugfix/descrição-do-bug`, etc.
- **Convenções para nomear commit**: Mensagens de commit devem ser claras e explicativas, como "Adiciona validação de formulário" ou "Corrige erro de cálculo em relatório".
