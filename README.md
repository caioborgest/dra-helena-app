# 🧠 Dra. Helena - Psicoterapia com IA

**Sua psicóloga particular assistida por IA**

Aplicação web de psicoterapia personalizada para Caio Diniz Borges com integração de inteligência artificial, chat em tempo real, rastreamento de humor, metas terapêuticas e diário pessoal.

## ✨ Funcionalidades

### 💬 Chat Terapêutico
- Conversa em tempo real com Dra. Helena
- Respostas baseadas em TCC, Teoria do Apego e Terapia do Esquema
- Contexto personalizado para sua situação profissional
- Histórico completo de sessões

### 🎤 Áudio Bidirecional
- **Grave sua voz** enquanto fala com a Dra. Helena
- **Ouça respostas** em áudio com síntese de voz natural em português
- Reproduza/pause qualquer mensagem de áudio
- Funciona com permissão de microfone

### 😊 Rastreador de Humor
- Registre seu bem-estar diário com emojis
- Acompanhe padrões emocionais
- Histórico semanal visualizado

### 🎯 Metas Terapêuticas
- Crie e acompanhe objetivos terapêuticos
- Progresso visual com barras
- Marque como concluídas

### 📔 Diário Pessoal
- Registre pensamentos e reflexões
- Organize por temas
- Histórico persistente

### 📈 Dashboard de Progresso
- Métricas gerais de evolução
- Gráficos por área de trabalho
- Timeline de sessões

## 🎯 Áreas de Trabalho

Especializada em desafios profissionais:
- ⚡ **Ansiedade Profissional** - Estratégias para pressão e deadlines
- 🎭 **Síndrome do Impostor** - Reconhecer seu valor real
- 🔥 **Burnout** - Recuperar energia e equilíbrio
- ✨ **Perfeccionismo** - Desenvolver realismo

## 🚀 Como Usar

### Online
1. Acesse: https://caioborgest.github.io/dra-helena-app
2. Passe pelo onboarding (4 etapas)
3. Comece sua primeira sessão

### Local
1. Faça download do arquivo `index.html`
2. Abra no navegador (funciona offline)
3. Instale como PWA no seu celular

### Como PWA
1. Abra em navegador mobile
2. Menu → "Instalar app"
3. Ícone na tela inicial

## 🔐 Privacidade

✅ **Dados 100% Privados**
- Armazenados localmente em localStorage
- Nenhuma informação enviada para servidores externos
- Exceção: API Perplexity para IA (sem logs pessoais)
- Você controla tudo

## ⚙️ Requisitos

- Navegador moderno (Chrome, Firefox, Safari, Edge)
- Conexão de internet para:
  - IA (Perplexity API)
  - Síntese de voz
  - Primeira inicialização
- Microfone (opcional, para áudio)

## 🛠️ Tecnologia

- **Frontend**: HTML5, CSS3, JavaScript vanilla
- **Armazenamento**: localStorage
- **IA**: Perplexity API (Llama 3.1 Sonar)
- **Áudio**: Web Audio API + Speech Synthesis API
- **PWA**: Service Worker

## 📋 Estrutura de Arquivos

```
dra-helena-app/
├── index.html              # Aplicação completa
├── README.md               # Este arquivo
├── LICENSE                 # MIT License
├── INSTALACAO.md           # Guia de instalação
└── .gitignore              # Configuração Git
```

## 🔑 Configuração

### API Key Perplexity
O app vem com uma chave de API de demonstração. Para máxima segurança, adicione sua própria chave:

1. Crie conta em https://perplexity.ai
2. Gere uma chave API
3. Substitua em `index.html`:
```javascript
const PERPLEXITY_API_KEY = 'sua-chave-aqui';
```

## 📱 Mobile

Otimizado para todos os tamanhos:
- ✅ Smartphone (375px+)
- ✅ Tablet (768px+)
- ✅ Desktop (1200px+)

## 🎓 Onboarding

4 etapas interativas:
1. **Apresentação** - Conheça a Dra. Helena
2. **Como Funciona** - Explore os recursos
3. **Áreas de Trabalho** - Temas personalizados
4. **Primeira Sessão** - Comece agora

## ⚠️ Disclaimer Importante

**Este app é um complemento ao acompanhamento psicológico profissional, não uma substituição.**

- Não é uma sessão terapêutica real
- Não substitui profissional de saúde mental
- Em crise: procure atendimento urgente

## 📄 Licença

MIT License - Veja arquivo LICENSE

## 👨‍💼 Desenvolvido Para

**Caio Diniz Borges**  
Growth & Marketing Professional  
Pernambuco, Brasil

---

**Desenvolvido com ❤️ usando Perplexity AI**