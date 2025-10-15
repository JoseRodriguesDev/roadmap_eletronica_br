# 📚 Roadmap Eletrônica — Brasil

## 📖 Descrição do Projeto

Este é um **sistema educacional interativo** desenvolvido para ensinar eletrônica de forma estruturada e progressiva. O projeto consiste em uma aplicação web single-page (SPA) que organiza conteúdo didático em módulos, matérias e aulas, permitindo que estudantes escolham diferentes trilhas de carreira na área de eletrônica.

## 🎯 Objetivo

Fornecer um caminho de aprendizado claro e organizado para profissionais e entusiastas de eletrônica no Brasil, desde conceitos fundamentais até especializações práticas como:
- Eletricista Residencial
- Reparo e Bancada
- Fontes Chaveadas e Inversores
- Eletrônica Automotiva

## 🏗️ Arquitetura do Projeto

### Estrutura de Arquivos

```
Roadmap eletronica/
│
├── index.html           # Aplicação principal (HTML + CSS + JavaScript)
│
└── data/
    ├── roadmap.json    # Dados dos módulos, matérias e aulas
    └── careers.json    # Definição das carreiras/trilhas de aprendizado
```

### Tecnologias Utilizadas

- **HTML5** - Estrutura da página
- **CSS3** - Estilização moderna com design responsivo
- **JavaScript (Vanilla)** - Lógica de aplicação sem frameworks
- **JSON** - Armazenamento de dados estruturados

## 🔧 Funcionalidades

### 1. **Sistema de Carreiras**
   - Múltiplas trilhas de aprendizado pré-definidas
   - Cada carreira possui módulos específicos organizados por prioridade
   - Salvamento automático da carreira selecionada (localStorage)

### 2. **Sistema de Progresso do Usuário**
   - **Marcar aulas como concluídas** com checkbox interativo
   - **Indicadores visuais** de progresso em cada módulo (%)
   - **Persistência** de progresso no localStorage (salvo localmente)
   - **Aulas completas** destacadas com ícone ✓ verde
   - **Badge de progresso** mostrando X/Y aulas concluídas

### 2.5. **Sistema de Favoritos** ⭐ NOVO v2.2
   - **Favoritar módulos** clicando na estrela (☆/⭐)
   - **Favoritar aulas específicas** individualmente
   - **Carreira "⭐ Favoritos"** dinâmica e personalizada
   - **Lógica inteligente**: Se aula favoritada → módulo aparece
   - **Interface intuitiva** com estrelas preenchidas/vazias

### 3. **Navegação Intuitiva**
   - **Sidebar** com lista de módulos filtráveis
   - **Busca em tempo real** para encontrar módulos, matérias ou aulas
   - **Painel principal** exibindo conteúdo da aula selecionada
   - **Painel lateral** com currículo completo do módulo
   - **Botões Próxima/Anterior** para navegar entre aulas ⭐ NOVO
   - **Breadcrumb** mostrando caminho completo da navegação ⭐ NOVO

### 4. **Conteúdo Rico**
   - Vídeos incorporados (YouTube)
   - Descrições detalhadas de cada aula
   - Tópicos-chave (keypoints)
   - Recursos secundários complementares com links externos

### 5. **Interface Moderna**
   - Design dark mode com paleta de cores profissional
   - Gradientes e efeitos visuais sutis
   - Layout responsivo (adaptável a diferentes tamanhos de tela)
   - Animações suaves de transição
   - **Loading spinner** durante carregamento ⭐ NOVO
   - **Tratamento de erros** amigável ⭐ NOVO

## 📚 Carreiras Disponíveis

### 0. **📚 Todos os Módulos**
Acesso completo a todo o conteúdo do roadmap
- Módulos: M01, M02, M05, M06, M07, M08, M09, M10, M11, M12
- **Ideal para**: Quem quer explorar tudo ou montar sua própria trilha

### 1. **⭐ Favoritos** ✨ NOVO
Seus módulos e aulas favoritados
- Módulos: Dinâmico (o que você favoritar)
- **Ideal para**: Revisar conteúdo específico, trilha personalizada
- **Como usar**: Clique na ⭐ em módulos ou aulas para adicionar

### 2. **Fundamentos / Núcleo Comum**
Conceitos básicos essenciais para todas as áreas
- Módulos: M01, M02

### 3. **Manutenção de Smartphones (início rápido)** 📱
Hardware, diagnóstico e reparo de smartphones
- Módulos: M01, M02, M11, M12

### 4. **Reparo & Bancada (início rápido)**
Instrumentação e técnicas de diagnóstico
- Módulos: M01, M02, M05, M06

### 5. **Fontes Chaveadas & Inversores (início rápido)**
Eletrônica de potência e conversores DC-DC/DC-AC
- Módulos: M01, M02, M07, M08

### 6. **Eletrônica Automotiva (diagnóstico & módulos)**
Sistemas elétricos veiculares e diagnóstico automotivo
- Módulos: M01, M02, M09, M10

## 📋 Conteúdo dos Módulos

### 🚧 Em Construção

O conteúdo completo dos módulos está sendo desenvolvido. Atualmente temos:

- ✅ **10 módulos** estruturados
- ✅ **60+ aulas** planejadas
- 🎥 **Vídeos educacionais** sendo adicionados progressivamente
- 📚 **Recursos complementares** em cada aula

**Status atual:**
- **Módulo 01** (Fundamentos de Eletricidade): 10 aulas com vídeos
- Demais módulos: Estrutura pronta, vídeos em processo de adição

Para ver o conteúdo completo e atualizado, acesse a plataforma e explore as carreiras disponíveis!

## 💻 Como Usar

### Requisitos
- Navegador web moderno (Chrome, Firefox, Edge, Safari)
- Servidor HTTP local (devido a requisições AJAX dos arquivos JSON)

### Execução Local

#### Opção 1: Python
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```

#### Opção 2: Node.js (http-server)
```bash
npx http-server -p 8000
```

#### Opção 3: PHP
```bash
php -S localhost:8000
```

Depois, acesse: `http://localhost:8000`

### Uso da Interface

1. **Selecione uma carreira** no menu superior
2. **Navegue pelos módulos** na barra lateral
   - Veja o **% de progresso** no canto superior direito de cada módulo
3. **Clique em um módulo** para ver suas matérias e aulas
4. **Selecione uma aula** no painel lateral direito
   - Aulas concluídas aparecem com **✓ verde**
5. **Assista a aula** e use os recursos:
   - **Breadcrumb** no topo mostra onde você está
   - **Checkbox** abaixo do vídeo para marcar como concluída
   - **Botões de navegação** para ir para próxima/anterior aula
6. **Use a busca** para filtrar conteúdo rapidamente

### Recursos da Interface v2.0

#### 📊 Sistema de Progresso
- Marque aulas como concluídas usando o checkbox
- Veja o progresso de cada módulo (ex: "3/9 aulas - 33%")
- Progresso é salvo automaticamente no navegador
- Aulas completas ficam destacadas com borda verde

#### 🧭 Navegação Aprimorada
- **Breadcrumb**: Carreira › Módulo › Matéria › Aula
- **Botões de navegação**: Avance/volte entre aulas sem precisar clicar na lista
- Botões desabilitados automaticamente na primeira/última aula

#### ⚡ Loading & Erros
- Spinner animado durante carregamento inicial
- Mensagens de erro detalhadas se algo falhar
- Validação de dados JSON

## 🎨 Paleta de Cores

```css
--bg: #0f172a        /* Fundo principal */
--card: #0c122d      /* Cards e painéis */
--muted: #9ca3af     /* Texto secundário */
--accent: #22d3ee    /* Destaque (cyan) */
--good: #10b981      /* Verde (sucesso) */
--warn: #f59e0b      /* Amarelo (aviso) */
--text: #e5e7eb      /* Texto principal */
--line: #1f2937      /* Bordas e divisores */
```

## 🔍 Funcionalidades Técnicas

### Armazenamento Local
O sistema utiliza `localStorage` para salvar:
- Última carreira selecionada pelo usuário

### Busca e Filtro
- Busca em tempo real através do texto digitado
- Filtro case-insensitive aplicado aos módulos visíveis

### Renderização Dinâmica
- Conteúdo carregado de arquivos JSON
- DOM atualizado dinamicamente sem recarregar página
- Scroll suave ao selecionar aulas

### Responsividade
```css
@media (max-width: 1100px) {
  /* Layout em coluna única */
  /* Sidebar não-fixo */
  /* Grid 2-colunas vira 1-coluna */
}
```

## 🎥 Sistema de Vídeos

Atualmente, todos os vídeos apontam para um player temporário (placeholder). A estrutura está preparada para incorporar:
- Vídeos do YouTube (`recursosPrincipais`)
- Links para conteúdo complementar (`recursosSecundarios`)

## 📊 Estrutura de Dados

### careers.json
```json
{
  "carreiras": [
    {
      "id": "string",
      "nome": "string",
      "trilha": [
        {
          "moduloId": "string",
          "materias": "*",
          "prioridade": number
        }
      ]
    }
  ]
}
```

### roadmap.json
```json
{
  "modulos": [
    {
      "idModulo": "string",
      "numeroModulo": number,
      "tituloModulo": "string",
      "descricaoModulo": "string",
      "materias": [
        {
          "idMateria": "string",
          "numeroMateria": number,
          "tituloMateria": "string",
          "aulas": [...]
        }
      ]
    }
  ]
}
```

## ✅ Melhorias Implementadas (v2.0)

- [x] **Sistema de progresso do usuário** - Concluído!
- [x] **Marcação de aulas concluídas** - Concluído!
- [x] **Navegação com botões Próxima/Anterior** - Concluído!
- [x] **Breadcrumb de navegação** - Concluído!
- [x] **Loading spinner** - Concluído!
- [x] **Validação e tratamento de erros** - Concluído!

## 🚀 Possíveis Melhorias Futuras

- [ ] Quiz/exercícios práticos ao final de cada aula
- [ ] Certificados de conclusão por módulo/carreira
- [ ] Modo offline (PWA - Progressive Web App)
- [ ] Comentários e discussões por aula
- [ ] Integração com plataforma de vídeo própria
- [ ] Sistema de busca mais avançado (tags, categorias)
- [ ] Notas e anotações do usuário por aula
- [ ] Exportação/importação de progresso (backup)
- [ ] Atalhos de teclado (← → para navegar)
- [ ] Estatísticas de aprendizado (tempo total, streak)
- [ ] Modo Light/Dark theme toggle
- [ ] Gamificação (badges, conquistas)

## 📝 Licença

**Copyright (c) 2025 Jose Vitor**

Este projeto é licenciado sob a **GNU Affero General Public License v3.0 (AGPL-3.0)** com condições adicionais:

### ⚠️ Uso Comercial Não Autorizado

Este código **NÃO PODE** ser utilizado (total ou parcialmente) em:
- ❌ Projetos comerciais
- ❌ Produtos pagos
- ❌ Serviços que gerem receita

**Sem permissão expressa por escrito do autor.**

### ✅ Uso Permitido

- ✅ Uso educacional
- ✅ Uso pessoal
- ✅ Estudo e aprendizado
- ✅ Modificações para uso próprio
- ✅ Compartilhamento (com mesma licença)

### 📄 Licença Completa

Consulte o arquivo `LICENSE` na raiz do projeto ou visite: https://www.gnu.org/licenses/agpl-3.0.html

### 👤 Autor

**Jose Vitor**  
GitHub: [github.com/JoseRodriguesDev](https://github.com/JoseRodriguesDev)

## 👥 Contribuindo

Para adicionar novos módulos ou carreiras:

1. Edite `data/roadmap.json` para adicionar módulos/matérias/aulas
2. Edite `data/careers.json` para criar ou modificar trilhas
3. Siga a estrutura de dados existente

## 🔗 Links Úteis

Todos os recursos secundários incluem links para vídeos educacionais do YouTube relacionados aos tópicos de cada aula.

---

**Desenvolvido com ❤️ para estudantes de eletrônica no Brasil**

