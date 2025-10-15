# 🚀 Início Rápido - Roadmap Eletrônica

## Executar o Projeto

### Opção 1: Python (Recomendado)
```bash
# Navegue até a pasta do projeto
cd "Roadmap eletronica"

# Execute o servidor
python -m http.server 8000
```

### Opção 2: Node.js
```bash
npx http-server -p 8000
```

### Opção 3: PHP
```bash
php -S localhost:8000
```

Depois acesse: **http://localhost:8000**

---

## 📖 Como Usar

### 1️⃣ Escolha sua Carreira
No menu superior direito, selecione a trilha que deseja seguir:
- 🔧 Fundamentos / Núcleo Comum
- 🏠 Eletricista Residencial
- 🔨 Reparo & Bancada
- ⚡ Fontes Chaveadas & Inversores
- 🚗 Eletrônica Automotiva

### 2️⃣ Navegue pelos Módulos
Na **barra lateral esquerda**, você verá:
- Lista de módulos da carreira escolhida
- **% de progresso** em cada módulo (canto superior direito)
- Campo de busca para filtrar rapidamente

### 3️⃣ Estude as Aulas
Ao clicar em um módulo:
- **Painel central**: Vídeo da aula + conteúdo detalhado
- **Painel direito**: Lista de todas as matérias e aulas
- **Breadcrumb** no topo mostra onde você está

### 4️⃣ Acompanhe seu Progresso
Durante o estudo:
- ✅ **Marque aulas como concluídas** usando o checkbox
- 📊 Veja seu progresso em tempo real
- ➡️ Use os botões **"Próxima Aula"** / **"Aula Anterior"**
- 🎯 Aulas completas ficam com **borda verde** e **ícone ✓**

---

## 🎯 Recursos Principais

### 📊 Sistema de Progresso
```
✓ Marcar aulas como concluídas
✓ Progresso salvo automaticamente
✓ Indicadores visuais (%, ícones)
✓ Persistência no navegador
```

### 🧭 Navegação Inteligente
```
✓ Breadcrumb: Carreira › Módulo › Matéria › Aula
✓ Botões Próxima/Anterior aula
✓ Busca em tempo real
✓ Scroll automático ao trocar aula
```

### 💾 Dados Salvos Localmente
Seu progresso é salvo no **localStorage** do navegador:
- Última carreira selecionada
- Aulas marcadas como concluídas
- Não precisa de conta ou login!

> ⚠️ **Importante**: Se limpar os dados do navegador, seu progresso será perdido.

---

## ❓ Problemas Comuns

### Erro ao Carregar JSON
**Sintoma**: Mensagem de erro ao abrir o site

**Solução**: 
1. Certifique-se de estar usando **HTTP**, não abrindo o arquivo direto (file://)
2. Verifique se os arquivos `roadmap.json` e `careers.json` estão na pasta `/data/`
3. Confira se os arquivos JSON são válidos (sem erros de sintaxe)

### Progresso não Salva
**Sintoma**: Aulas marcadas voltam desmarcadas

**Solução**: 
1. Verifique se o localStorage está habilitado no navegador
2. Não use modo anônimo/privado
3. Verifique se há espaço disponível no localStorage

### Botões de Navegação Desabilitados
**Sintoma**: Não consigo clicar em "Próxima Aula"

**Isso é normal!** Os botões são desabilitados quando:
- Você está na **primeira aula** (Anterior desabilitado)
- Você está na **última aula** (Próxima desabilitado)

---

## 📱 Acesso Mobile

O site é **totalmente responsivo**! Funciona perfeitamente em:
- 📱 Smartphones
- 📱 Tablets
- 💻 Notebooks
- 🖥️ Desktops

Em telas menores:
- Menu lateral fica na vertical
- Grid vira 1 coluna
- Botões de navegação ficam empilhados

---

## 🆘 Suporte

Problemas? Verifique:
1. Console do navegador (F12) para erros
2. Arquivo CHANGELOG.md para mudanças recentes
3. README.md para documentação completa

---

**Desenvolvido com ❤️ para estudantes de eletrônica no Brasil**

Versão: 2.0.0

