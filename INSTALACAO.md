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
   - **Initialize with README**: Deixe desmarcado (vamos adicionar)
3. Clique **Create repository**

### Passo 2: Upload dos Arquivos

#### Opção A: Via GitHub Web
1. Vá para seu repositório criado
2. Clique **Add file** → **Create new file**
3. Adicione cada arquivo:
   - Copie o conteúdo de `index.html`
   - Cole no editor
   - Commit

#### Opção B: Via Git (Linha de Comando)
```bash
# Clone seu repositório
git clone https://github.com/seu-usuario/dra-helena-app.git
cd dra-helena-app

# Copie os arquivos para a pasta

# Adicione todos os arquivos
git add .

# Commit
git commit -m "Adicionar Dra. Helena App"

# Push para GitHub
git push origin main
```

### Passo 3: Ativar GitHub Pages

1. Vá para **Settings** do seu repositório
2. No menu esquerdo, clique **Pages**
3. Em **Source**, selecione:
   - Branch: **main**
   - Folder: **/ (root)**
4. Clique **Save**
5. Aguarde 1-2 minutos

### Passo 4: Acessar Sua App

Após ativar GitHub Pages, você verá uma mensagem de sucesso com o link:

**https://seu-usuario.github.io/dra-helena-app**

Substitua `seu-usuario` pelo seu username do GitHub.

---

## 💻 Opção 2: Executar Localmente

### Passo 1: Clone o Repositório

```bash
git clone https://github.com/caioborgest/dra-helena-app.git
cd dra-helena-app
```

### Passo 2: Abra no Navegador

#### Windows
```bash
start index.html
```

#### macOS
```bash
open index.html
```

#### Linux
```bash
xdg-open index.html
```

Ou simplesmente clique duas vezes em `index.html`

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
4. Um atalho será criado na sua área de trabalho

---

## 🔧 Configuração da API Perplexity

A app vem com uma chave de demonstração incluída. Para máxima segurança e limite de requisições, configure sua própria chave:

### Gerar sua Chave API

1. Acesse https://www.perplexity.ai/
2. Faça login ou crie conta
3. Vá para **Settings** → **API**
4. Clique **Create New Key**
5. Copie a chave gerada

### Adicionar à Sua App

#### Se usar GitHub Pages
1. Abra seu repositório no GitHub
2. Clique em `index.html`
3. Clique no lápis (✏️) para editar
4. Procure pela linha:
```javascript
const PERPLEXITY_API_KEY = 'pplx-...';
```
5. Substitua pela sua chave:
```javascript
const PERPLEXITY_API_KEY = 'sua-chave-aqui';
```
6. Desça, clique **Commit changes**

#### Se usar Localmente
1. Abra `index.html` em editor de texto
2. Procure por `const PERPLEXITY_API_KEY`
3. Substitua a chave
4. Salve (Ctrl+S)
5. Recarregue o navegador

---

## ✅ Checklist de Verificação

Após instalação, teste cada funcionalidade:

- [ ] **Onboarding** - Aparece tela de apresentação na primeira vez
- [ ] **Chat** - Consigo enviar mensagens de texto
- [ ] **IA Responde** - Dra. Helena responde com confiança
- [ ] **Áudio Gravação** - Botão 🎤 funciona e grava
- [ ] **Áudio Resposta** - Dra. Helena fala sua resposta
- [ ] **Mood Tracker** - Posso registrar humor
- [ ] **Goals** - Posso criar e editar metas
- [ ] **Diário** - Posso escrever e salvar entradas
- [ ] **Progresso** - Dashboard mostra estatísticas
- [ ] **PWA Install** - Opção de instalar aparece
- [ ] **Offline** - Dados persistem após reload

---

## 🐛 Troubleshooting

### "Microfone não funciona"
**Causa**: Permissão não foi concedida

**Solução**:
1. Verifique permissão do navegador
2. Chrome/Edge: **Settings** → **Privacy** → **Microphone**
3. Adicione seu site à lista de permissões
4. Recarregue a página
5. Tente novamente

### "Áudio não sai (sem som)"
**Causa**: Síntese de voz desabilitada

**Solução**:
1. Aumente volume do dispositivo
2. Teste em outra aba/navegador
3. Verifique se navegador suporta Speech Synthesis
4. Chrome/Firefox/Safari funcionam bem

### "Mensagens não salvam"
**Causa**: localStorage está desabilitado ou cheio

**Solução**:
1. Verifique se está em modo privado (desabilita localStorage)
2. Limpe cache do navegador
3. Tente em modo normal
4. Na aba Info, clique **Limpar Tudo**

### "API retorna erro 401"
**Causa**: Chave da API inválida ou expirada

**Solução**:
1. Gere nova chave em perplexity.ai
2. Substitua no código
3. Confirme que copiou corretamente (sem espaços)
4. Teste em outro navegador

### "GitHub Pages não publica"
**Causa**: Configuração incorreta

**Solução**:
1. Verifique se repositório é PUBLIC
2. Vá para **Settings** → **Pages**
3. Selecione **main branch**
4. Espere 2-5 minutos
5. Verifique URL: `seu-usuario.github.io/dra-helena-app`

---

## 📞 Suporte & Debug

### Abrir Console do Navegador
1. Pressione **F12** ou **Ctrl+Shift+I**
2. Vá para aba **Console**
3. Procure por mensagens de erro (texto vermelho)
4. Copie e guarde para referência

### Limpar Dados Completamente
1. Abra a aba **Info** no app
2. Clique em **Limpar Tudo** (botão vermelho)
3. Confirme
4. Página recarrega e volta ao onboarding

### Factory Reset (Console)
Se precisar resetar completamente:
```javascript
// Abra console (F12) e cole:
localStorage.removeItem('caioTherapyState');
location.reload();
```

---

## 🎉 Próximos Passos

Após instalação bem-sucedida:

1. **Passe pelo Onboarding** 
   - Conheça Dra. Helena
   - Explore funcionalidades
   - Entenda as áreas de trabalho

2. **Inicie Primeira Sessão**
   - Conte sobre seu estado emocional
   - Escolha foco principal
   - Comece conversa com IA

3. **Explore Todos os Recursos**
   - Registre humor diário
   - Crie metas terapêuticas
   - Escreva no diário
   - Acompanhe progresso

4. **Customize (Opcional)**
   - Adicione sua foto de perfil
   - Personalize temas
   - Ajuste preferências de áudio

---

## 🔐 Notas de Segurança

✅ **O que é privado:**
- Todas as mensagens
- Humor registrado
- Metas e diário
- Dados pessoais

❌ **O que não é privado:**
- Requisições à API Perplexity (padrão da API)
- Texto enviado para IA (você controla)

**Recomendação**: Use sua própria chave de API e não compartilhe links com dados sensíveis.

---

## 📚 Documentação Adicional

- **README.md** - Visão geral do projeto
- **LICENSE** - MIT License (use livremente)
- Este arquivo - Guia de instalação completo

---

**Bem-vindo à sua jornada terapêutica! 💚**

Qualquer dúvida, consulte o README ou abra uma issue no GitHub.