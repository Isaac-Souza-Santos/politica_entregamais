# 📄 Política de Privacidade - Entrega+

Site estático com a política de privacidade do app Entrega+, hospedado no Heroku.

## 🚀 Deploy no Heroku

### Deploy Automático

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/seu-usuario/entrega-plus-privacy)

### Deploy Manual

1. **Criar app no Heroku:**

```bash
heroku create entrega-plus-privacy
```

2. **Fazer deploy:**

```bash
git init
git add .
git commit -m "Deploy política de privacidade"
git push heroku main
```

3. **Abrir site:**

```bash
heroku open
```

## 📁 Estrutura

- `index.html` - Política de privacidade em HTML
- `Procfile` - Configuração do Heroku
- `runtime.txt` - Versão do Python
- `requirements.txt` - Dependências (nenhuma)
- `app.json` - Configuração do app

## 🌐 URL

Após o deploy, a política estará disponível em:
`https://entrega-plus-privacy.herokuapp.com`

## 📱 Integração com o App

No app Flutter, use esta URL para a política de privacidade:

```dart
static const String privacyPolicyUrl = 'https://entrega-plus-privacy.herokuapp.com';
```

## 🔧 Personalização

Para editar a política:

1. Modifique o arquivo `index.html`
2. Faça commit das alterações
3. Faça push para o Heroku

```bash
git add index.html
git commit -m "Atualizar política de privacidade"
git push heroku main
```

## 📋 Conteúdo

A política de privacidade inclui:

- ✅ Informações coletadas
- ✅ Como os dados são usados
- ✅ Compartilhamento de informações
- ✅ Segurança e armazenamento
- ✅ Direitos do usuário
- ✅ Retenção de dados
- ✅ Menores de idade
- ✅ Alterações na política
- ✅ Base legal (LGPD)
- ✅ Informações de contato

## 🎨 Design

- Design responsivo
- Cores do app Entrega Plus
- Fácil leitura
- Navegação clara
- Compatível com mobile
