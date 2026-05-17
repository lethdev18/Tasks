# 🚀 O que temos para hoje? — Dashboard de Produtividade

Dashboard pessoal de produtividade com integração ao **Google Gmail**, **Google Calendar** e **Google Tasks**.

Cada usuário faz login com a **própria conta Google** e vê apenas os seus dados.

## 🌐 Acesso

👉 **[Abrir o Dashboard](https://lethdev18.github.io/Tasks/)**

---

## ⚙️ Configuração (para o desenvolvedor)

### 1. Habilitar o GitHub Pages

1. Vá em **Settings → Pages** no repositório
2. Em **Source**, selecione `Deploy from a branch`
3. Branch: `main` | Pasta: `/ (root)`
4. Clique em **Save**

### 2. Autorizar o domínio no Google Cloud Console

Para que o login Google funcione no GitHub Pages, adicione a URL do site nas origens autorizadas:

1. Acesse [console.cloud.google.com](https://console.cloud.google.com)
2. Vá em **APIs e Serviços → Credenciais**
3. Clique no seu **OAuth 2.0 Client ID**
4. Em **Origens JavaScript autorizadas**, adicione:
   ```
   https://SEU-USUARIO.github.io
   ```
5. Em **URIs de redirecionamento autorizados**, adicione:
   ```
   https://SEU-USUARIO.github.io/SEU-REPOSITORIO/
   ```
6. Clique em **Salvar**

### 3. Publicar o app OAuth (para outros usuários)

Se quiser que **outras pessoas** também possam fazer login:

1. Vá em **APIs e Serviços → Tela de permissão OAuth**
2. Clique em **Publicar app**
3. Confirme a publicação

> ⚠️ Se o app estiver em modo "Teste", apenas os e-mails cadastrados como testadores conseguem fazer login.

---

## 🔑 Permissões solicitadas

O dashboard solicita acesso **somente leitura** às seguintes APIs:

| Permissão | Uso |
|---|---|
| `gmail.readonly` | Conta e-mails não lidos |
| `calendar` | Exibe eventos de hoje e amanhã |
| `tasks` | Sincroniza lista de tarefas |
| `userinfo.profile` | Exibe nome e foto do usuário |
| `userinfo.email` | Identifica a conta logada |

---

## 📁 Arquivos do projeto

```
📂 raiz/
 ├── index.html       ← Dashboard completo (HTML + CSS + JS)
 ├── floyd-bg2.jpg    ← Wallpaper de fundo
 └── README.md        ← Este arquivo
```

---

© 2026 Dashboard de Produtividade
