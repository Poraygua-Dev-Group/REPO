# 🤝 Guia de Contribuição - Porãygua

Este guia vai te ajudar a contribuir para o repositório de treinamento da comunidade Porãygua.

## 📋 Pré-requisitos

* Conta no GitHub
* Git instalado no seu computador
* Editor de texto (VS Code, Vim, Nano, etc.)

## 🔄 Fluxo de Contribuição

### 1\. Fork do Repositório

1. Acesse o repositório original: `YhannMatheus/Rank.gg`
2. Clique no botão **Fork** no canto superior direito
3. Selecione sua conta para criar o fork

### 2\. Clone do Fork

``` bash
git clone https://github.com/Poraygua-Dev-Group/REPO.git
cd REPO
```

### 3\. Configurar Remote Upstream

``` bash
git remote add upstream https://github.com/Poraygua-Dev-Group/REPO.git
git remote -v
```

### 4\. Criar uma Branch

``` bash
git checkout -b apresentacao/seu-nome
# Exemplo: git checkout -b apresentacao/joao-silva
```

### 5\. Fazer suas Mudanças

* Copie o arquivo `exemplo-apresentacao.md`
* Renomeie para `seu-nome.md`
* Coloque na pasta `apresentacoes/`
* Preencha com suas informações

### 6\. Commit das Mudanças

``` bash
git add .
git commit -m "feat: adiciona apresentação de [Seu Nome]"
```

### 7\. Push para seu Fork

``` bash
git push origin apresentacao/seu-nome
```

### 8\. Criar Pull Request

1. Acesse seu fork no GitHub
2. Clique em **Compare & pull request**
3. Preencha o título e descrição
4. Clique em **Create pull request**

## 📝 Padrões de Commit

Use os seguintes prefixos nos seus commits:

* `feat:` \- Nova funcionalidade ou apresentação
* `fix:` \- Correção de bugs
* `docs:` \- Mudanças na documentação
* `style:` \- Formatação\, sem mudança de código
* `refactor:` \- Refatoração de código
* `test:` \- Adição ou correção de testes

**Exemplos:**

* `feat: adiciona apresentação sobre Docker`
* `fix: corrige link quebrado no README`
* `docs: atualiza instruções de contribuição`

## 📁 Estrutura de Apresentação

Sua apresentação deve seguir o template em `exemplo-apresentacao.md` e incluir:

* **Nome e GitHub**: Identificação
* **Título**: Tema da apresentação
* **Resumo**: Breve descrição
* **Tópicos**: Lista dos pontos abordados
* **Recursos**: Links e materiais de apoio
* **Contato**: Como te encontrar

## 🎯 Dicas de Git

### Manter Fork Atualizado

``` bash
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```

### Resolver Conflitos

1. Identifique os arquivos com conflito
2. Edite os arquivos removendo as marcações
3. Adicione e commite as mudanças
4. Continue o merge/rebase

### Comandos Úteis

``` bash
# Ver status
git status

# Ver histórico
git log --oneline

# Ver diferenças
git diff

# Desfazer último commit (mantendo mudanças)
git reset --soft HEAD~1

# Desfazer mudanças não commitadas
git checkout -- arquivo.md
```

## ❓ Precisa de Ajuda?

* Abra uma **Issue** descrevendo sua dúvida
* Pergunte no canal da comunidade Porãygua
* Consulte a [documentação oficial do Git](https://git-scm.com/doc)

## 🌊 Código de Conduta

* Seja respeitoso com todos os membros
* Mantenha discussões construtivas
* Ajude outros membros quando possível
* Divirta-se aprendendo!

- - -

**Obrigado por contribuir com a comunidade Porãygua! 🎉**