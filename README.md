# 🎓 credly-badges-widget

**Widget de badges Credly com fundo transparente para GitHub Pages**

Um widget elegante que exibe todos os seus badges da Credly com design responsivo e fundo transparente. Perfeito para incorporar em seus repositórios GitHub via iframe.

## ✨ Características

- 🔄 **Integração automática com GitHub Actions** - Usa a action [pemtajo/badge-readme](https://github.com/marketplace/actions/badges-readme) para buscar TODOS os badges da Credly
- 🎨 **Design responsivo** - Se adapta a qualquer tamanho de tela
- ✨ **Badges circulares com fundo transparente** - Design limpo e moderno
- 📱 **Embed em iframe** - Incorpore facilmente em qualquer repositório GitHub
- 🚀 **Hosted no GitHub Pages** - Deploy automático e gratuito
- 🔄 **Atualizações automáticas** - Sincroniza com seus badges da Credly diariamente

## 🚀 Como Usar

### Opção 1: Ver o Widget em Tempo Real

Acesse diretamente em:
```
https://aiexxplorer.github.io/credly-badges-widget/
```

### Opção 2: Incorporar em seu README

Adicione o código HTML abaixo em seu arquivo `README.md` onde deseja que os badges apareçam:

```html
<iframe 
  src="https://aiexxplorer.github.io/credly-badges-widget/" 
  style="width: 100%; height: 500px; border: none; border-radius: 8px;" 
  title="Credly Badges Widget"
></iframe>
```

Ou com CSS customizado:

```html
<div align="center">
  <iframe 
    src="https://aiexxplorer.github.io/credly-badges-widget/" 
    width="100%" 
    height="600" 
    style="border: none; border-radius: 8px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);" 
    title="Credly Badges"
  ></iframe>
</div>
```

## 🔧 Tecnologia

- **Frontend**: HTML5, CSS3, JavaScript vanilla
- **CI/CD**: GitHub Actions
- **Hosting**: GitHub Pages
- **Badge Source**: [Credly](https://www.credly.com/)

## 📋 Estrutura

```
.
├── .github/workflows/
│   └── credly-badges.yml       # Workflow que executa a action
├── public/
│   └── badges-data.html        # HTML gerado com os badges
├── index.html                  # Página principal (GitHub Pages)
└── README.md                   # Esta documentação
```

## 🔄 Como Funciona

1. **GitHub Action Diária**: O workflow `credly-badges.yml` executa diariamente às 00:00 UTC
2. **Badge Readme Action**: A action [pemtajo/badge-readme](https://github.com/marketplace/actions/badges-readme) busca TODOS os badges do seu perfil Credly
3. **Geração de HTML**: Um arquivo HTML é gerado com os badges em design responsivo
4. **GitHub Pages**: O arquivo é servido via GitHub Pages
5. **Embed via iframe**: Você pode incorporar em qualquer lugar usando um iframe

## 🛠️ Customização

Para usar em seu próprio perfil Credly:

1. **Fork este repositório**
2. **Edite o arquivo `.github/workflows/credly-badges.yml`** e altere:
   ```yaml
   CREDLY_USER: seu-usuario-credly
   ```
3. **Customize o HTML** em `public/badges-data.html` conforme necessário
4. **Ative GitHub Pages** nas configurações do repositório
5. **Use a URL do seu repositório** no iframe

## 📊 Workflow Automático

O arquivo `.github/workflows/credly-badges.yml` inclui:

- ✅ Execução diária automática (00:00 UTC)
- ✅ Trigger manual via `workflow_dispatch`
- ✅ Integração com pemtajo/badge-readme action
- ✅ Geração dinâmica de HTML com CSS
- ✅ Commit automático de mudanças
- ✅ Permissões de escrita necessárias

## 🎯 Exemplo de Integração

Em seu README.md principal, adicione:

```markdown
## 🏆 Certificações e Badges

<div align="center">
  <iframe 
    src="https://aiexxplorer.github.io/credly-badges-widget/" 
    width="100%" 
    height="600" 
    style="border: none;" 
  ></iframe>
</div>
```

## 📝 Notas Importantes

- Os badges são atualizados automaticamente diariamente
- O design utiliza fundo **transparente** - funciona com qualquer cor de fundo
- Os badges são **clicáveis** e levam ao seu perfil Credly
- A altura do iframe pode ser ajustada conforme necessário (recomendado mínimo 500px)

## 🔗 Links Úteis

- [Meu Perfil Credly](https://www.credly.com/users/aiexxplorer/badges)
- [Badge Readme Action](https://github.com/marketplace/actions/badges-readme)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)

## 📄 Licença

Este projeto está disponível sob a licença MIT.

---

**Desenvolvido com ❤️ para a comunidade de desenvolvimento**
