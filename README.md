# Raio-X de Carreira do Dentista · Oral Centter

Landing page interativa para captura de leads de dentistas interessados em franquia.

## 🚀 Setup Rápido

### Pré-requisitos
- GitHub (conta free)
- Vercel (conta free, vinculada ao GitHub)
- Seu Webhook do Make (da automação)
- Seu Pixel ID do Meta

---

## 📋 Passo 1: Clonar / Criar Repositório no GitHub

### Opção A: Se você vai criar do zero

1. Acesse **github.com** e faça login
2. Clique no `+` no canto superior direito → "New repository"
3. Nome: `raiox-carreira-dentista`
4. Descrição: `LP de Raio-X de Carreira para captação de franqueados`
5. Deixe **Public** (para Vercel conseguir acessar)
6. Clique "Create repository"

### Opção B: Se você já tem um repositório

Pule para o Passo 2.

---

## 📁 Passo 2: Preparar os Arquivos Locais

Na sua máquina, crie uma pasta com essa estrutura:

```
raiox-carreira-dentista/
├── index.html          (arquivo principal)
├── README.md           (este arquivo)
└── .gitignore          (opcional)
```

### Copiar os arquivos

1. Baixe o `index.html` que forneci (arquivo standalone pronto para desktop e mobile)
2. Coloque na pasta `raiox-carreira-dentista`
3. **IMPORTANTE:** Antes de fazer upload, edite o arquivo e preencha:

```javascript
var WEBHOOK_URL = 'https://hook.us1.make.com/SEU_WEBHOOK_AQUI';
var PIXEL       = 'SEU_PIXEL_ID_AQUI';
```

---

## 🔗 Passo 3: Fazer Upload para GitHub (via Web)

Se você não tem Git instalado, usar a web é mais fácil:

1. Acesse seu repositório em github.com (ex: github.com/seu-usuario/raiox-carreira-dentista)
2. Clique em "Add file" → "Upload files"
3. Arraste o `index.html` para a caixa (ou clique para selecionar)
4. Na mensagem de commit, escreva algo como:
   - "Initial commit: Add raiox landing page"
5. Clique "Commit changes"

**Pronto!** Seu código agora está no GitHub.

---

## 🌐 Passo 4: Publicar no Vercel

Vercel é uma plataforma que lê seu GitHub e publica automaticamente.

### 4.1 Criar conta Vercel

1. Acesse **vercel.com**
2. Clique "Sign Up" → "Continue with GitHub"
3. Autorize Vercel a acessar suas contas GitHub
4. Pronto, você está logado

### 4.2 Importar repositório

1. No dashboard do Vercel, clique "Add New..." → "Project"
2. Em "Import Git Repository", encontre `raiox-carreira-dentista`
3. Clique para selecionar
4. **Configuração:**
   - Project name: deixe como está (ou customize)
   - Framework: "Other" (é HTML puro)
   - Root Directory: deixe em branco
   - Environment Variables: **deixe em branco** (vamos usar direto no HTML)
5. Clique "Deploy"

**Vercel vai:**
- Clonar seu repositório
- Fazer build (no caso, só copia os arquivos)
- Publicar em um URL tipo: `https://raiox-carreira-dentista.vercel.app`

### 4.3 Aguardar deployment

Você vai ver uma barra de progresso. Quando virar verde com um ✓, pronto!

---

## 🔄 Atualizar o site (após mudanças)

Workflow simples:

1. **Edite localmente** o `index.html` na sua máquina
2. **Faça upload para GitHub:**
   - Via web: clique no arquivo no repositório → edit (ícone de lápis) → cole o conteúdo atualizado → "Commit changes"
   - Ou via Git (se souber usar terminal)
3. **Vercel vai detectar a mudança automaticamente** e fará redeploy em segundos
4. Seu site no Vercel atualiza sozinho

---

## ⚙️ Configurar o Webhook e Pixel

Se precisar mudar o Webhook ou Pixel depois:

1. Abra o `index.html` no repositório (clique nele no GitHub)
2. Clique no ícone de edição (lápis)
3. Procure por:
   ```javascript
   var WEBHOOK_URL = '...';
   var PIXEL = '...';
   ```
4. Altere os valores
5. Clique "Commit changes"
6. Vercel refaz o deploy em ~30 segundos

---

## ✅ Testar

1. Acesse a URL do Vercel (ex: `https://raiox-carreira-dentista.vercel.app`)
2. Teste em desktop e mobile
3. Preencha o formulário até o final
4. Verifique se o lead chegou no seu Webhook/Kommo

---

## 🆘 Troubleshooting

### Site não aparece
- Espere 2-3 minutos após o deploy ficar verde
- Recarregue (Ctrl+Shift+R no Chrome/Firefox)
- Verifique a URL (sem typos)

### Webhook ou Pixel não funcionando
- Verifique se as variáveis estão corretas (sem espaços extras)
- Teste o Webhook isoladamente (pode usar Postman)
- Meta Pixel: verifique se o pixel está ativo no Meta Ads Manager

### Mudanças não aparecem no site
- Verifique se fez Commit no GitHub (marque a caixa "Commit directly...")
- Aguarde 30-60 segundos (tempo de redeploy do Vercel)
- Limpe cache do navegador (Ctrl+Shift+Del)

---

## 📊 Monitorar Deployment

No dashboard do Vercel, você vê:
- Histórico de deployments
- Logs de erro (se houver)
- Estatísticas de performance
- Domínio customizado (opcional, pago)

---

## 🎯 Próximos Passos

- Customizar domínio (exemplo: `carreira.oralcentter.com`) — pago, mas fácil
- Adicionar Analytics (Google Analytics, Hotjar)
- A/B testing com Vercel Analytics

---

**Dúvidas?** Mensagem direta ou repositório Issues no GitHub.
