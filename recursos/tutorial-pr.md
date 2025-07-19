# 🔄 Como Fazer um Pull Request (PR)

Este tutorial ensina como criar um Pull Request no GitHub para contribuir com o repositório da Porãygua.

## 🎯 O que é um Pull Request?

Um Pull Request (PR) é uma solicitação para que suas mudanças sejam incorporadas ao repositório principal. É uma forma de:

- Propor mudanças
- Revisar código
- Discutir implementações
- Colaborar com a comunidade

## 📋 Pré-requisitos

- Fork do repositório feito ✅
- Clone local do seu fork ✅
- Mudanças commitadas na sua branch ✅
- Push das mudanças para seu fork ✅

## 🚀 Passo a Passo

### 1. Acesse seu Fork no GitHub

1. Vá para `https://github.com/SEU_USUARIO/Rank.gg`
2. Certifique-se de que suas mudanças foram enviadas

### 2. Inicie o Pull Request

Você verá uma das opções:

**Opção A: Banner Automático**
- GitHub mostra um banner: "Compare & pull request"
- Clique neste botão

**Opção B: Manual**
1. Clique na aba **Pull requests**
2. Clique em **New pull request**
3. Selecione as branches:
   - **base:** `YhannMatheus/Rank.gg` → `main`
   - **compare:** `SEU_USUARIO/Rank.gg` → `sua-branch`

### 3. Preencha as Informações

#### Título
Use um título claro e descritivo:
```
feat: adiciona apresentação sobre Docker por João Silva
fix: corrige links quebrados no README
docs: atualiza instruções de contribuição
```

#### Descrição
Preencha com detalhes sobre sua contribuição:

```markdown
## 📝 Descrição

Adiciona minha apresentação sobre Docker para a pasta de apresentações.

## 🎯 Tipo de Mudança

- [x] Nova apresentação
- [ ] Correção de bug
- [ ] Atualização de documentação
- [ ] Outro: ___________

## 📋 Checklist

- [x] Segui o template de apresentação
- [x] Adicionei minha apresentação na pasta correta
- [x] Testei todos os links
- [x] Revisei o conteúdo

## 📚 Sobre a Apresentação

- **Tema:** Docker para Iniciantes
- **Duração:** ~30 minutos
- **Nível:** Iniciante
- **Data planejada:** 15/08/2024

## 💬 Observações

Primeira contribuição para a comunidade Porãygua! 🌊
```

### 4. Configurar o Pull Request

#### Reviewers (Opcional)
- Adicione `@YhannMatheus` como reviewer
- Outros membros experientes da comunidade

#### Assignees
- Atribua a você mesmo se for trabalhar no PR

#### Labels (Se disponíveis)
- `apresentação` - Para novas apresentações
- `documentação` - Para updates de docs
- `iniciante` - Para primeiras contribuições

#### Projects (Se aplicável)
- Adicione ao projeto da comunidade

### 5. Criar o Pull Request

1. Revise todas as informações
2. Clique em **Create pull request**
3. Aguarde a revisão da comunidade

## 📝 Template de Descrição

Copie e cole este template para padronizar seus PRs:

```markdown
## 📝 Descrição

[Descreva brevemente o que foi feito]

## 🎯 Tipo de Mudança

- [ ] Nova apresentação
- [ ] Correção de bug
- [ ] Atualização de documentação
- [ ] Melhoria de código
- [ ] Outro: ___________

## 📋 Checklist

- [ ] Segui as diretrizes de contribuição
- [ ] Testei as mudanças localmente
- [ ] Atualizei documentação se necessário
- [ ] Adicionei/atualizei testes se aplicável

## 📚 Detalhes Adicionais

[Informações extras sobre a mudança]

## 💬 Observações

[Comentários, agradecimentos, dúvidas]
```

## ✅ Após Criar o PR

### O que Esperar

1. **Revisão Automática**
   - GitHub pode executar checks automáticos
   - Aguarde os resultados

2. **Revisão da Comunidade**
   - Membros irão revisar seu código
   - Podem solicitar mudanças
   - Façam perguntas ou sugestões

3. **Discussão**
   - Participem da discussão
   - Respondam comentários
   - Façam mudanças se necessário

### Como Atualizar o PR

Se precisar fazer mudanças:

1. **Faça as mudanças localmente**
   ```bash
   # Na mesma branch do PR
   git add .
   git commit -m "fix: corrige comentários da revisão"
   git push origin sua-branch
   ```

2. **O PR será atualizado automaticamente**

### Respondendo a Comentários

- **Seja respeitoso** e profissional
- **Agradeça** o feedback
- **Esclareça dúvidas** quando necessário
- **Faça as mudanças** solicitadas

## 🎉 Merge do Pull Request

Quando seu PR for aprovado:

1. **Maintainer fará o merge**
2. **Sua branch pode ser deletada**
3. **Atualize seu fork local**
   ```bash
   git checkout main
   git pull upstream main
   git push origin main
   ```

## 🚨 Problemas Comuns

### PR com Conflitos

```bash
# Atualizar sua branch com a main
git checkout main
git pull upstream main
git checkout sua-branch
git rebase main

# Resolver conflitos manualmente
# Depois continuar o rebase
git rebase --continue
git push --force-with-lease origin sua-branch
```

### Commits Muito Grandes

- Use `git rebase -i` para squash commits
- Mantenha histórico limpo

### Mudanças Solicitadas

- Não leve para o pessoal
- Veja como oportunidade de aprender
- Faça as mudanças e continue

## 💡 Dicas de Ouro

### Para um Bom PR

- **Título claro** e objetivo
- **Descrição completa** mas concisa
- **Uma mudança por PR** quando possível
- **Testes** suas mudanças antes

### Para Boa Colaboração

- **Seja paciente** com reviews
- **Seja respeitoso** com feedback
- **Aprenda** com os comentários
- **Ajude outros** quando possível

### Para a Comunidade

- **Revisar PRs** de outros membros
- **Dar feedback construtivo**
- **Compartilhar conhecimento**
- **Celebrar contribuições**

## 📞 Precisa de Ajuda?

- **Comente no PR** explicando sua dúvida
- **Abra uma Issue** para problemas técnicos
- **Pergunte na comunidade** Porãygua
- **Consulte a documentação** do GitHub

---

**Sua primeira contribuição é especial! Seja bem-vindo à colaboração open source! 🌊**
