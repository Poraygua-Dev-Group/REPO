# 🛠️ Comandos Git Essenciais

Este guia contém os comandos Git mais utilizados para contribuir com o repositório da Porãygua.

## 🚀 Configuração Inicial

### Configurar Identidade
```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu.email@exemplo.com"
```

### Verificar Configuração
```bash
git config --list
```

## 📁 Trabalhando com Repositórios

### Clonar Repositório
```bash
git clone https://github.com/usuario/repositorio.git
```

### Inicializar Repositório Local
```bash
git init
```

### Adicionar Remote
```bash
git remote add origin https://github.com/usuario/repositorio.git
git remote add upstream https://github.com/original/repositorio.git
```

### Ver Remotes
```bash
git remote -v
```

## 🔄 Fluxo de Trabalho

### Ver Status
```bash
git status
```

### Adicionar Arquivos
```bash
git add arquivo.txt              # Arquivo específico
git add .                        # Todos os arquivos
git add *.md                     # Todos os arquivos .md
```

### Fazer Commit
```bash
git commit -m "feat: adiciona nova funcionalidade"
git commit -am "fix: corrige bug"  # add + commit de arquivos modificados
```

### Ver Histórico
```bash
git log                          # Histórico completo
git log --oneline               # Histórico resumido
git log --graph                 # Histórico visual
```

## 🌿 Trabalhando com Branches

### Listar Branches
```bash
git branch                       # Branches locais
git branch -r                    # Branches remotas
git branch -a                    # Todas as branches
```

### Criar Branch
```bash
git branch nova-feature          # Criar branch
git checkout -b nova-feature     # Criar e mudar para branch
git switch -c nova-feature       # Forma moderna
```

### Mudar de Branch
```bash
git checkout main               # Forma clássica
git switch main                 # Forma moderna
```

### Deletar Branch
```bash
git branch -d feature-branch    # Deletar branch local
git push origin --delete feature-branch  # Deletar branch remota
```

## 📤 Sincronização

### Baixar Mudanças
```bash
git fetch origin               # Baixa sem mergear
git pull origin main           # Baixa e mergeia
```

### Enviar Mudanças
```bash
git push origin main           # Enviar para remote
git push -u origin feature     # Primeira vez (set upstream)
```

### Atualizar Fork
```bash
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```

## 🔀 Merge e Rebase

### Merge
```bash
git checkout main
git merge feature-branch
```

### Rebase
```bash
git checkout feature-branch
git rebase main
```

### Rebase Interativo
```bash
git rebase -i HEAD~3           # Últimos 3 commits
```

## 🆘 Comandos de Emergência

### Desfazer Último Commit (mantendo mudanças)
```bash
git reset --soft HEAD~1
```

### Desfazer Último Commit (perdendo mudanças)
```bash
git reset --hard HEAD~1
```

### Descartar Mudanças Não Commitadas
```bash
git checkout -- arquivo.txt    # Arquivo específico
git checkout .                  # Todos os arquivos
```

### Stash (salvar mudanças temporariamente)
```bash
git stash                      # Salvar mudanças
git stash pop                  # Recuperar mudanças
git stash list                 # Listar stashes
git stash drop                 # Descartar stash
```

## 🔍 Comandos de Investigação

### Ver Diferenças
```bash
git diff                       # Mudanças não staged
git diff --staged              # Mudanças staged
git diff HEAD~1               # Comparar com commit anterior
```

### Buscar em Commits
```bash
git log --grep="bug"          # Buscar por mensagem
git log --author="João"       # Buscar por autor
git log --since="2 weeks"     # Últimas 2 semanas
```

### Blame (quem mudou o quê)
```bash
git blame arquivo.txt
```

## 🏷️ Tags

### Criar Tag
```bash
git tag v1.0.0
git tag -a v1.0.0 -m "Versão 1.0.0"
```

### Listar Tags
```bash
git tag
```

### Enviar Tags
```bash
git push origin v1.0.0
git push origin --tags
```

## 🎯 Dicas Importantes

### Mensagens de Commit
- Use prefixos: `feat:`, `fix:`, `docs:`, `style:`, `refactor:`
- Seja descritivo mas conciso
- Use imperativo: "adiciona" ao invés de "adicionando"

### Boas Práticas
- Commits pequenos e frequentes
- Teste antes de fazer push
- Mantenha histórico limpo
- Use branches para features

### Atalhos Úteis
```bash
# Aliases úteis para adicionar no .gitconfig
git config --global alias.st status
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.ci commit
git config --global alias.unstage "reset HEAD --"
```

---

**Precisa de mais ajuda? Consulte a [documentação oficial do Git](https://git-scm.com/doc)! 📚**
