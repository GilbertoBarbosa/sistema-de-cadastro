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

Criando uma Tag no Git
```
git tag -a v1.0.0
```

Git Remote
```
# Lista os repositórios remotos disponíveis
git remote

# Adicionar novo repositório
git remote add <nome> <endereço>
```

Branches
```
# Criando uma nova branche
git checkout -b <nome>

# Mudando de breach
git switch main

# Enviando alterações para o GitHub
git push origin <nome da branche>

```