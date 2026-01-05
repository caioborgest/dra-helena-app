# 📦 Guia de Instalação - Dra. Helena App

## Pré-requisitos

✅ Navegador moderno (Chrome, Firefox, Safari ou Edge)  
✅ Conexão com internet  
✅ (Opcional) Git instalado  

## 🚀 Opção 1: GitHub Pages (RECOMENDADO)

### Passo 1: Criar Repositório no GitHub

1. Acesse https://github.com/new
2. Preencha:
   - **Repository name**: `dra-helena-app`
   - **Description**: Psicoterapia com IA - Dra. Helena Monteiro
   - **Public**: Selecionado ✅
   - **Initialize with README**: Deixe desmarcado
3. Clique **Create repository**

### Passo 2: Upload dos Arquivos

1. Vá para seu repositório criado
2. Clique **Add file** → **Upload files**
3. Selecione os arquivos:
   - index.html
   - README.md
   - INSTALACAO.md
   - LICENSE
   - GITHUB.md
4. Clique **Commit changes**

### Passo 3: Ativar GitHub Pages

1. Vá para **Settings** do seu repositório
2. No menu esquerdo, clique **Pages**
3. Em **Source**, selecione:
   - Branch: **main**
   - Folder: **/ (root)**
4. Clique **Save**
5. Aguarde 1-2 minutos

### Passo 4: Acessar Sua App

Após ativar GitHub Pages, você verá:

**https://seu-usuario.github.io/dra-helena-app**

Substitua `seu-usuario` pelo seu username do GitHub.

---

## 💻 Opção 2: Executar Localmente

### Passo 1: Baixar o Arquivo

1. Faça download do `index.html`
2. Salve em uma pasta

### Passo 2: Abra no Navegador

#### Windows
```bash
Clique duas vezes em index.html
```

#### macOS
```bash
Clique duas vezes em index.html
```

#### Linux
```bash
xdg-open index.html
```

### Passo 3: Pronto!

A app abrirá em seu navegador padrão com todas as funcionalidades ativas.

---

## 📱 Opção 3: Instalar como PWA (Progressive Web App)

### No Celular (Android)
1. Abra a URL em navegador mobile
2. Toque no menu (⋮ ou ⋮⋮)
3. Selecione **"Instalar app"** ou **"Add to Home Screen"**
4. Confirme
5. Um ícone aparecerá na tela inicial

### No Celular (iOS/Safari)
1. Abra a URL em Safari
2. Toque no ícone **Compartilhar** (canto inferior)
3. Selecione **"Adicionar à Tela de Início"**
4. Confirme
5. Um ícone aparecerá na tela inicial

### No Desktop (Chrome/Edge)
1. Abra a URL no navegador
2. Clique no ícone de instalação (canto da barra de endereço)
3. Confirme a instalação

---

## 🔧 Configuração da API Perplexity

A app vem com uma chave de demonstração. Para máxima segurança:

### Gerar sua Chave API

1. Acesse https://www.perplexity.ai/
2. Faça login ou crie conta
3. Vá para **Settings** → **API**
4. Clique **Create New Key**
5. Copie a chave gerada

### Adicionar à App

1. Abra `index.html` em editor de texto
2. Procure por: `const PERPLEXITY_API_KEY = 'pplx-...';`
3. Substitua pela sua chave:
```javascript
const PERPLEXITY_API_KEY = 'sua-chave-aqui';
```
4. Salve o arquivo

---

## ✅ Checklist de Verificação

Após instalação, teste:

- [ ] **Onboarding** - Aparece tela de apresentação
- [ ] **Chat** - Consegue enviar mensagens
- [ ] **IA Responde** - Dra. Helena responde
- [ ] **Áudio Gravação** - Botão 🎤 grava sua voz
- [ ] **Áudio Resposta** - Dra. Helena fala em áudio
- [ ] **Mood Tracker** - Registra humor diário
- [ ] **Goals** - Cria e edita metas
- [ ] **Diário** - Escreve e salva entradas
- [ ] **Progresso** - Dashboard mostra gráficos
- [ ] **PWA Install** - Opção de instalar aparece
- [ ] **Dados Salvam** - Após reload, dados persistem

---

## 🐛 Troubleshooting

### "Microfone não funciona"
**Causa**: Permissão não foi concedida

**Solução**:
1. Navegador → Settings → Privacy → Microphone
2. Adicione seu site à lista de permissões
3. Recarregue a página
4. Tente novamente

### "Áudio não sai (sem som)"
**Causa**: Síntese de voz desabilitada

**Solução**:
1. Aumente volume do dispositivo
2. Teste em outro navegador (Chrome funciona melhor)
3. Verifique se navegador suporta Speech Synthesis

### "Mensagens não salvam"
**Causa**: localStorage desabilitado

**Solução**:
1. Não use modo privado
2. Limpe cache do navegador
3. Verifique se localStorage está habilitado

### "API retorna erro"
**Causa**: Chave inválida ou limite atingido

**Solução**:
1. Verifique se chave está correta
2. Gere nova chave em perplexity.ai
3. Teste em outro navegador

### "GitHub Pages não publica"
**Causa**: Configuração incorreta

**Solução**:
1. Repositório deve ser PUBLIC
2. Vá para Settings → Pages
3. Selecione main branch
4. Aguarde 2-5 minutos
5. Recarregue com Ctrl+Shift+R

---

## 📞 Suporte & Debug

### Abrir Console do Navegador
1. Pressione **F12** ou **Ctrl+Shift+I**
2. Vá para aba **Console**
3. Procure por mensagens de erro (texto vermelho)

### Limpar Dados Completamente
1. Na aba **Info** do app
2. Clique **Limpar Tudo** (botão vermelho)
3. Página recarrega ao onboarding

---

## 🎉 Próximos Passos

1. **Passe pelo Onboarding** (4 etapas)
2. **Inicie Primeira Sessão** com Dra. Helena
3. **Explore Todos os Recursos** (mood, goals, diário)
4. **Instale como PWA** no celular
5. **Aproveite sua jornada terapêutica** 💚

---

**Bem-vindo! Qualquer dúvida, consulte este guia.**