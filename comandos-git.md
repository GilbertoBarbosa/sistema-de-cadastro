# Comandos GIT mais comuns

Configurações Iniciais
```
# Cadastrando nome
git config --local/global user.name = "Nome do usuário Git" 

# Cadastrando email
git config --local/global user.email = "E-mail do usuário Git"

```

Inicia um novo repositório
```
git init
git init --bare #indica que o repositório é puro
```

Adiciona alterações nos arquivos
```
git add .
```

Faz um commit - Para todos arquivos digite . após o commit
```
git commit -m  <arquivo> "Mensagem commit"
```

Copia um repositório da nuvem (github) para a máquina local (git)
Grava por cima de um repositório já existente.
É realizado só no início do projeto
```
git clone <repositorio>
```

Merge e Rebase
```
# Junta os trabalhos e gera um merge commit
git merge <branch>

# Aplica os commits de outra branch na branch atual
git rebase <branch>
```

Atualiza um repositório local com base no repositório da nuvem.
```
git pull <repositório>

# Integra as mudanças de um branch para outro
git pull --rebase
```

Sobe as alterações (comitadas) do repositório local para a nuvem (GitHub)
origin main (divisão principal)
```
git push origin main
```

Git log
```
# Mostra o histórico de commits
git log

# Mostra o histórico de commits de forma resumida (uma linha)
git log --oneline

# Mostra o histórico de commits de forma detalhada
git log -p

# Mostra o histórico de commits de forma gráfica
git log -graph
```

Visualiza o que está diferente no projeto
```
git status
```

Desfazendo alterações
```
# Desfaz alterações não commitadas em um arquivo
git restore <arquivo>

# Desfaz alterações não commitadas em todos os arquivos
git restore .

# Desmarca arquivos marcadados para commitar
git restore --staged <arquivo>

# Reverter um commit ja realizado
git revert <rash do commit a ser revertido>
```

Voltando um arquivo a um estado anterior:
```
# Para verificar o código do commit
git log --oneline

# Para reverter alteração localmente
git restore --source <codigo> <arquivo ou .>

# Para comitar as alterações localmente
git commit <arquivo> -m "Mensagem do commit"

# Para subir a reversão para o GitHub
git push
```

Guardando alterações para depois
```
# Salva alterações para depois
git stash

# Lista alterações salvas
git stash list

# Inclui alteração guardada no arquivo
git stash apply <código da alteração>

# Exclui alteração guardada
git stash drop

# Inclui a alteração e exclui da stash
git stash pop
```

Git diff
```
# Mostrando a diferença do código entre commits
git diff <hash cod1>...<hash cod2>

# Mostrando o que não foi commitado
git diff
```

Versões no Git
```
# Inserir uma nova Tag
git tag -a v1.0.0

# Listar as Tags
git tag

# Enviar a versão para o servidor
git push <servidor> <tag>
```

Git Remote
```
# Lista os repositórios remotos disponíveis
git remote

# Adicionar novo repositório
git remote add <nome> <endereço>
```

Incluir arquivo(s) no último commit
```
git add .
git commit --amend


Branches
```
# Criando uma nova branche
git checkout -b <nome>

# Mudando de breach
git switch main

# Enviando alterações para o GitHub
git push origin <nome da branche>

```
