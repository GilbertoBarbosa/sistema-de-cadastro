# Comandos GIT mais comuns

Inicia um novo repositório
```
git ini
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
```

Sobe as alterações (comitadas) do repositório local para a nuvem (GitHub)
origin main (divisão principal)
```
git push origin main
```

Mostra o histórico de commits
```
git log
```

Mostra o histórico de commits de forma resumida
```
git log --oneline
```

Visualiza o que está diferente no projeto
```
git status
```