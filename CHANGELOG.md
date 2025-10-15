# Changelog

Todas as mudanças notáveis neste projeto serão documentadas neste arquivo.

## [2.0.0] - 2025-10-14

### ✨ Novas Funcionalidades

#### 📊 Sistema de Progresso do Usuário
- ✅ **Marcar aulas como concluídas**: Checkbox interativo abaixo de cada vídeo
- ✅ **Persistência de dados**: Progresso salvo automaticamente no localStorage
- ✅ **Indicadores visuais**: 
  - Porcentagem de conclusão em cada módulo na sidebar (ex: "67%")
  - Aulas completas destacadas com ícone ✓ verde
  - Borda verde nas aulas concluídas
  - Badge de progresso mostrando "X/Y aulas (Z%)"
- ✅ **Cálculo automático**: Sistema recalcula progresso ao marcar/desmarcar aulas

#### 🧭 Navegação Aprimorada
- ✅ **Breadcrumb**: Navegação hierárquica mostrando caminho completo
  - Formato: `Carreira › Módulo › Matéria › Aula`
  - Atualiza automaticamente ao trocar de aula
  - Aula atual destacada em cyan
- ✅ **Botões de navegação**: 
  - Botão "Aula Anterior" (com ícone de seta esquerda)
  - Botão "Próxima Aula" (com ícone de seta direita)
  - Desabilitados automaticamente na primeira/última aula
  - Navegação sequencial através de todas as aulas da carreira

#### ⚡ Melhorias Técnicas
- ✅ **Loading spinner**: Animação durante carregamento inicial dos dados
- ✅ **Validação de dados**: Verifica integridade dos arquivos JSON
- ✅ **Tratamento de erros robusto**: 
  - Mensagens de erro amigáveis e informativas
  - Instruções sobre como resolver problemas comuns
  - Detalhes técnicos no console para debug

### 🎨 Melhorias Visuais

- Novo estilo para botões de aula (layout flex com ícone de check)
- Badge de sucesso verde quando módulo 100% completo
- Indicador de progresso em tempo real nos cards de módulo
- Botões de navegação com hover effects e estados disabled
- Loading overlay com spinner animado
- Melhor responsividade em telas menores

### 🔧 Mudanças Técnicas

- Adicionado objeto `currentLesson` para rastrear contexto atual
- Novas funções de gerenciamento de progresso:
  - `getProgressKey()` - Gera chave única para localStorage
  - `isLessonComplete()` - Verifica se aula está concluída
  - `setLessonComplete()` - Marca/desmarca aula
  - `getModuleProgress()` - Calcula estatísticas de progresso
  - `updateModuleProgress()` - Atualiza badge de progresso
  - `toggleLessonComplete()` - Handler do checkbox
- Novas funções de navegação:
  - `getAllLessonsFlat()` - Lista plana de todas as aulas
  - `getCurrentLessonIndex()` - Índice da aula atual
  - `navigateLesson()` - Navega para próxima/anterior
  - `updateNavigationButtons()` - Atualiza estado dos botões
- Nova função de breadcrumb:
  - `updateBreadcrumb()` - Renderiza caminho de navegação
- Novas funções de loading:
  - `showLoading()` - Exibe overlay de loading
  - `hideLoading()` - Esconde overlay de loading

### 📦 Armazenamento Local

O sistema agora utiliza localStorage para:
- `careerId` - Última carreira selecionada
- `lesson_complete_{aulaId}` - Estado de cada aula (true/false)

### 🎯 CSS Adicionado

```css
.loading-overlay - Overlay fullscreen com spinner
.spinner - Animação de loading
.breadcrumb - Navegação hierárquica
.lesson-nav - Container dos botões de navegação
.nav-btn - Estilo dos botões de navegação
.lesson-complete-wrapper - Container do checkbox
.btn.completed - Estado de aula concluída
.check-icon - Ícone de check verde
.progress-indicator - Indicador de % nos módulos
.badge.success - Badge verde de 100%
```

---

## [1.0.0] - Data Inicial

### Funcionalidades Iniciais

- Sistema de carreiras múltiplas
- Estrutura de módulos, matérias e aulas
- Player de vídeo integrado
- Busca em tempo real
- Design dark mode responsivo
- Sidebar com lista de módulos
- Painel de currículo lateral
- Salvamento de carreira selecionada
- Recursos complementares por aula
- Links externos para material de apoio

