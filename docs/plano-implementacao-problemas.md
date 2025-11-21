# Plano de Implementação - Seção "Problemas Identificados"

## 🎯 Objetivo
Expandir e melhorar a seção "Problemas Identificados" na homepage do projeto (`index.html`) para demonstrar claramente as diferenças entre o site original ufsc.br e a versão corrigida, fundamentadas nas 10 Heurísticas de Usabilidade de Jakob Nielsen.

---

## 📋 Estrutura Proposta

### Seção Expandida com 7 Problemas Principais

Cada problema será apresentado em um card expandido contendo:

1. **Número e Título do Problema**
2. **Heurísticas Violadas** (com ícones/cores)
3. **Descrição do Problema no Site Original**
4. **Comparação Visual** (Antes vs Depois)
5. **Correções Implementadas** (lista detalhada)
6. **Fundamentação Teórica Resumida**
7. **Link para Ver Correção** (quando aplicável)
8. **Impacto na Experiência do Usuário**

---

## 🔧 Implementação Detalhada

### 1. Problema: Navegação Complexa e Sobrecarga Cognitiva

**Heurísticas Violadas:** #6 (Reconhecimento), #8 (Design Minimalista), #3 (Controle)

**Card Expandido:**
- **Antes:** Menu com 50+ links, múltiplos níveis hierárquicos, estrutura confusa
- **Depois:** Menu simplificado (6 itens principais), seção "Acesso Rápido" com cards visuais
- **Correções:**
  - Menu principal reduzido de 50+ para 6 itens principais
  - Criação de seção "Acesso Rápido" com 8 serviços mais utilizados
  - Cards visuais com ícones para identificação rápida
  - Busca destacada e acessível
- **Fundamentação:** Nielsen (1994) - Interfaces devem minimizar carga cognitiva
- **Link:** `pages/homepage/` (demonstração na homepage corrigida)

---

### 2. Problema: Falta de Feedback Visual em Interações

**Heurísticas Violadas:** #1 (Visibilidade do Status), #4 (Consistência), #7 (Eficiência)

**Card Expandido:**
- **Antes:** Links sem hover states, botões sem feedback, elementos não indicam interatividade
- **Depois:** Todos os elementos têm estados hover/focus/active claros, transições suaves
- **Correções:**
  - Estados hover implementados em todos os links e botões
  - Transições CSS suaves para feedback visual
  - Indicadores de foco visíveis para navegação por teclado
  - Carrossel com indicadores ativos e controles visíveis
- **Fundamentação:** Nielsen (1994) - Sistema deve sempre informar ao usuário o que está acontecendo
- **Link:** `pages/homepage/` (ver interações na homepage)

---

### 3. Problema: Hierarquia Visual Inconsistente

**Heurísticas Violadas:** #8 (Design Minimalista), #6 (Reconhecimento), #4 (Consistência)

**Card Expandido:**
- **Antes:** Múltiplos elementos competindo pela atenção, sem hierarquia clara
- **Depois:** Banner dominante, seções bem definidas, tipografia hierárquica
- **Correções:**
  - Carrossel hero com título grande e destaque visual
  - Sistema de tipografia claro (H1-H6 com tamanhos distintos)
  - Grid system consistente para organização
  - Contraste e espaçamento adequados entre seções
- **Fundamentação:** Preece et al. (2015) - Hierarquia visual guia atenção e facilita compreensão
- **Link:** `pages/homepage/` (ver hierarquia aplicada)

---

### 4. Problema: Problemas de Acessibilidade

**Heurísticas Violadas:** #1 (Visibilidade), #7 (Flexibilidade), WCAG 2.1

**Card Expandido:**
- **Antes:** Contraste insuficiente, navegação por teclado limitada, falta de estrutura semântica
- **Depois:** Contraste WCAG AA, navegação por teclado completa, HTML semântico
- **Correções:**
  - Contraste de cores aumentado (azul #003366 sobre branco)
  - Navegação por teclado com indicadores de foco visíveis
  - Estrutura HTML semântica (header, nav, section, footer)
  - Labels descritivos em elementos interativos
  - Suporte a leitores de tela melhorado
- **Fundamentação:** WCAG 2.1 - Critérios objetivos de contraste e navegação
- **Link:** `pages/homepage/` (testar acessibilidade)

---

### 5. Problema: Linguagem Técnica Não Adequada

**Heurísticas Violadas:** #2 (Compatibilidade), #6 (Reconhecimento), #10 (Ajuda)

**Card Expandido:**
- **Antes:** Siglas sem contexto (PROGRAD, PROEX, CAGR), jargão acadêmico
- **Depois:** Linguagem orientada a tarefas, termos claros, contexto fornecido
- **Correções:**
  - Menu principal usa linguagem do usuário ("Ensino", "Pesquisa", "Extensão")
  - Seção "Acesso Rápido" com nomes descritivos completos
  - Textos introdutórios em linguagem clara e acessível
  - Eliminação de siglas desnecessárias no menu principal
- **Fundamentação:** Norman (2013) - Sistemas devem usar linguagem do mundo real
- **Link:** `pages/homepage/` (ver linguagem aplicada)

---

### 6. Problema: Falta de Prevenção de Erros em Formulários

**Heurísticas Violadas:** #5 (Prevenção), #9 (Recuperação), #1 (Visibilidade)

**Card Expandido:**
- **Antes:** Validação apenas no submit, mensagens de erro pouco claras
- **Depois:** Validação em tempo real, máscaras de entrada, feedback imediato
- **Correções:**
  - Validação em tempo real implementada (`assets/js/main.js`)
  - Máscaras de entrada para CPF e telefone
  - Mensagens de erro descritivas e acionáveis
  - Feedback visual durante preenchimento
- **Fundamentação:** Nielsen (1994) - Melhor prevenir erros do que depender de mensagens
- **Link:** `pages/formularios/` (quando disponível) ou `assets/js/main.js` (código)

---

### 7. Problema: Inconsistência Visual e de Padrões

**Heurísticas Violadas:** #4 (Consistência), #6 (Reconhecimento), #3 (Controle)

**Card Expandido:**
- **Antes:** Estilos diferentes entre páginas, espaçamentos variáveis, cores inconsistentes
- **Depois:** Design system unificado, componentes padronizados, consistência visual
- **Correções:**
  - Design system centralizado (`assets/css/style.css`)
  - Paleta de cores consistente (azul UFSC #003366)
  - Componentes reutilizáveis (botões, cards, formulários)
  - Espaçamentos padronizados (variáveis CSS)
  - Tipografia consistente em toda a interface
- **Fundamentação:** Nielsen (1994) - Usuários não devem se perguntar se ações diferentes significam a mesma coisa
- **Link:** `pages/homepage/` (ver consistência aplicada)

---

## 🎨 Componentes Visuais a Criar

### Cards de Problema Expandidos
- Layout em grid responsivo (1 coluna mobile, 2 colunas tablet, 3 colunas desktop)
- Cards com sombra e hover effect
- Seção "Antes vs Depois" com comparação visual
- Badges coloridos para heurísticas violadas
- Ícones para cada tipo de problema

### Comparação Visual
- Screenshots ou mockups lado a lado (quando possível)
- Código de exemplo mostrando correção técnica
- Lista de melhorias implementadas

### Badges de Heurísticas
- Cores diferentes para cada heurística
- Tooltip explicativo ao passar o mouse
- Link para fundamentação teórica completa

---

## 📝 Estrutura HTML Proposta

```html
<section id="problemas" class="section section-alt">
    <div class="container">
        <h2>Problemas Identificados e Correções</h2>
        <p class="text-secondary mb-lg">
            Análise comparativa entre o site original ufsc.br e a versão corrigida, 
            fundamentada nas 10 Heurísticas de Usabilidade de Jakob Nielsen.
        </p>
        
        <div class="problems-grid-expanded">
            <!-- Card 1: Navegação -->
            <div class="problem-card-expanded">
                <div class="problem-header">
                    <span class="problem-number">1</span>
                    <h3>Navegação Complexa</h3>
                    <div class="heuristics-badges">
                        <span class="badge badge-heuristic" data-heuristic="6">#6</span>
                        <span class="badge badge-heuristic" data-heuristic="8">#8</span>
                        <span class="badge badge-heuristic" data-heuristic="3">#3</span>
                    </div>
                </div>
                
                <div class="problem-comparison">
                    <div class="comparison-before">
                        <h4>❌ Site Original</h4>
                        <ul>
                            <li>Menu com 50+ links simultâneos</li>
                            <li>Múltiplos níveis hierárquicos</li>
                            <li>Sobrecarga cognitiva</li>
                        </ul>
                    </div>
                    <div class="comparison-after">
                        <h4>✅ Versão Corrigida</h4>
                        <ul>
                            <li>Menu simplificado (6 itens principais)</li>
                            <li>Seção "Acesso Rápido" com cards visuais</li>
                            <li>Busca destacada e acessível</li>
                        </ul>
                    </div>
                </div>
                
                <div class="problem-corrections">
                    <h4>Correções Implementadas:</h4>
                    <ul class="corrections-list">
                        <li>✓ Redução do menu principal de 50+ para 6 itens</li>
                        <li>✓ Criação de seção "Acesso Rápido" com 8 serviços</li>
                        <li>✓ Cards visuais com ícones para identificação rápida</li>
                        <li>✓ Busca destacada na navegação principal</li>
                    </ul>
                </div>
                
                <div class="problem-theory">
                    <p><strong>Fundamentação:</strong> Nielsen (1994) - Interfaces devem minimizar carga cognitiva, 
                    apresentando informações de forma clara e hierárquica.</p>
                </div>
                
                <div class="problem-actions">
                    <a href="pages/homepage/" target="_blank" class="btn btn-primary">
                        Ver Correção na Homepage
                    </a>
                </div>
            </div>
            
            <!-- Repetir para outros 6 problemas -->
        </div>
    </div>
</section>
```

---

## 🎨 Estilos CSS Necessários

### Classes Principais:
- `.problems-grid-expanded` - Grid responsivo para cards
- `.problem-card-expanded` - Card individual expandido
- `.problem-header` - Cabeçalho com número e badges
- `.problem-comparison` - Seção antes/depois
- `.comparison-before` / `.comparison-after` - Colunas de comparação
- `.problem-corrections` - Lista de correções
- `.corrections-list` - Lista estilizada com checkmarks
- `.problem-theory` - Fundamentação teórica
- `.heuristics-badges` - Badges das heurísticas
- `.badge-heuristic` - Badge individual com cor por heurística

### Cores por Heurística:
- #1 (Visibilidade): Azul claro
- #2 (Compatibilidade): Verde claro
- #3 (Controle): Laranja claro
- #4 (Consistência): Roxo claro
- #5 (Prevenção): Vermelho claro
- #6 (Reconhecimento): Amarelo claro
- #7 (Eficiência): Ciano claro
- #8 (Minimalismo): Cinza claro
- #9 (Recuperação): Rosa claro
- #10 (Ajuda): Marrom claro

---

## 📊 Ordem de Implementação

### Fase 1: Estrutura Base
1. Expandir HTML da seção de problemas
2. Criar estrutura de cards expandidos
3. Adicionar todos os 7 problemas identificados

### Fase 2: Conteúdo Detalhado
4. Preencher descrições "Antes" e "Depois" para cada problema
5. Listar todas as correções implementadas
6. Adicionar fundamentação teórica resumida

### Fase 3: Estilização
7. Criar CSS para cards expandidos
8. Implementar badges de heurísticas com cores
9. Estilizar comparação antes/depois
10. Adicionar hover effects e transições

### Fase 4: Interatividade
11. Adicionar tooltips nos badges de heurísticas
12. Implementar links funcionais para páginas de correção
13. Adicionar animações suaves de expansão (opcional)

### Fase 5: Refinamento
14. Revisar textos e garantir clareza
15. Testar responsividade em diferentes dispositivos
16. Validar acessibilidade (contraste, navegação por teclado)

---

## 🔗 Links e Referências

### Links Internos:
- `pages/homepage/` - Homepage corrigida (demonstra todos os problemas corrigidos)
- `pages/navegacao/` - Página específica de navegação melhorada
- `pages/feedback-visual/` - Página específica de feedback visual
- `docs/analise-problemas.md` - Documentação completa dos problemas
- `docs/fundamentacao-teorica.md` - Fundamentação teórica completa

### Seções da Página:
- `#problemas` - Seção de problemas identificados
- `#prototipo` - Seção do protótipo
- `#comparacao` - Seção de comparação vídeo

---

## ✅ Critérios de Sucesso

A implementação será considerada bem-sucedida quando:

1. ✅ Todos os 7 problemas principais estão documentados
2. ✅ Cada problema mostra claramente "Antes vs Depois"
3. ✅ Correções implementadas estão listadas detalhadamente
4. ✅ Heurísticas violadas estão identificadas com badges visuais
5. ✅ Fundamentação teórica está presente em cada card
6. ✅ Links para ver correções estão funcionais
7. ✅ Design é responsivo e acessível
8. ✅ Comparação visual é clara e compreensível

---

## 📝 Notas de Implementação

- Manter consistência visual com o resto do site
- Usar design system existente (`assets/css/style.css`)
- Garantir que textos sejam claros e acessíveis
- Adicionar screenshots quando possível (futuro)
- Considerar adicionar animações sutis para melhorar UX
- Manter foco na clareza e objetividade acadêmica

---

## 🚀 Próximos Passos

1. Implementar estrutura HTML base
2. Adicionar conteúdo detalhado de cada problema
3. Criar estilos CSS para cards expandidos
4. Testar e refinar
5. Adicionar screenshots comparativos (opcional, futuro)

