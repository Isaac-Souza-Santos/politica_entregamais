# 🚀 Deploy da Política de Privacidade no Heroku

## 📋 Pré-requisitos

1. **Conta no Heroku** - [Criar conta](https://heroku.com)
2. **Heroku CLI** - [Instalar](https://devcenter.heroku.com/articles/heroku-cli)
3. **Git** - [Instalar](https://git-scm.com)

## 🔧 Deploy Rápido

### 1. Login no Heroku

```bash
heroku login
```

### 2. Criar App

```bash
heroku create entrega-plus-privacy
```

### 3. Deploy

```bash
git init
git add .
git commit -m "Deploy política de privacidade"
git push heroku main
```

### 4. Abrir Site

```bash
heroku open
```

## 🌐 URLs

- **Site:** https://entrega-plus-privacy.herokuapp.com
- **Dashboard:** https://dashboard.heroku.com/apps/entrega-plus-privacy

## 📱 Integração com o App

No arquivo `entrega_plus/lib/shared/services/route_optimization_service.dart`, adicione:

```dart
class RouteOptimizationService {
  static const String _baseUrl = 'https://entregamaisapi-183964d61a02.herokuapp.com';
  static const String _privacyPolicyUrl = 'https://entrega-plus-privacy.herokuapp.com';
  // ... resto do código
}
```

## 🔄 Atualizações

Para atualizar a política:

1. **Editar o arquivo:**

```bash
# Editar index.html com as mudanças necessárias
```

2. **Fazer commit:**

```bash
git add index.html
git commit -m "Atualizar política de privacidade"
```

3. **Deploy:**

```bash
git push heroku main
```

## 🎨 Personalização

### Cores

Para alterar as cores, edite o CSS no `index.html`:

```css
/* Cores principais */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
color: #667eea;
```

### Logo

Para adicionar um logo, substitua o emoji no header:

```html
<h1>🚚 Entrega Plus</h1>
<!-- Por -->
<h1>
  <img src="logo.png" alt="Entrega Plus" style="height: 50px;" /> Entrega Plus
</h1>
```

## 📊 Monitoramento

### Logs

```bash
heroku logs --tail
```

### Status

```bash
heroku ps
```

### Configurações

```bash
heroku config
```

## 🔒 Segurança

- ✅ HTTPS automático
- ✅ Sem dados sensíveis
- ✅ Site estático
- ✅ Sem banco de dados

## 💰 Custos

- **Hobby Plan**: Gratuito (com limitações)
- **Basic Plan**: $7/mês (recomendado para produção)

## 🆘 Troubleshooting

### Erro de Deploy

```bash
heroku logs --tail
```

### Site não carrega

```bash
heroku restart
```

### Problemas de Git

```bash
git remote -v
heroku git:remote -a entrega-plus-privacy
```

## 📞 Suporte

- [Documentação Heroku](https://devcenter.heroku.com/)
- [Heroku Support](https://help.heroku.com/)
