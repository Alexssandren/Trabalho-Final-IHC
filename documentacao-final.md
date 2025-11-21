# Análise Crítica e Redesign de Interface - Site UFSC.br

## 📄 Documento Técnico para Atividade Final 1 - IHC

**Disciplina:** Interface Humano-Computador (IHC)  
**Instituição:** Universidade Federal de Santa Catarina (UFSC)  
**Curso:** Tecnologia da Informação e Comunicação (TIC)  
**Período:** 5ª Fase  
**Data:** Dezembro de 2025  

**Autores:**  
Felipe F. e Letícia  

---

## 📋 SUMÁRIO

1. [INTRODUÇÃO](#1-introdução)
2. [CONTEXTUALIZAÇÃO DO SISTEMA ANALISADO](#2-contextualização-do-sistema-analisado)
3. [METODOLOGIA DE ANÁLISE](#3-metodologia-de-análise)
4. [PROBLEMAS IDENTIFICADOS](#4-problemas-identificados)
   4.1. [Problema 1: Navegação Complexa e Sobrecarga Cognitiva](#problema-1-navegação-complexa-e-sobrecarga-cognitiva)
   4.2. [Problema 2: Falta de Feedback Visual em Interações](#problema-2-falta-de-feedback-visual-em-interações)
   4.3. [Problema 3: Hierarquia Visual Inconsistente](#problema-3-hierarquia-visual-inconsistente)
   4.4. [Problema 4: Problemas de Acessibilidade](#problema-4-problemas-de-acessibilidade)
   4.5. [Problema 5: Linguagem Técnica Não Adequada](#problema-5-linguagem-técnica-não-adequada)
   4.6. [Problema 6: Falta de Prevenção de Erros em Formulários](#problema-6-falta-de-prevenção-de-erros-em-formulários)
   4.7. [Problema 7: Inconsistência Visual e de Padrões](#problema-7-inconsistência-visual-e-de-padrões)
5. [CONCLUSÃO](#5-conclusão)
6. [REFERÊNCIAS](#6-referências)

---

# 1. INTRODUÇÃO

## 1.1 Justificativa da Escolha do Sistema

A escolha do site institucional da Universidade Federal de Santa Catarina (UFSC) como objeto de análise crítica justifica-se por diversos fatores estratégicos para o aprendizado em Interface Humano-Computador (IHC):

Primeiramente, trata-se de um sistema de **domínio público e cotidiano**, utilizado por milhares de usuários diariamente - estudantes, servidores, comunidade externa e pesquisadores. Esta característica garante que os problemas identificados tenham impacto real na experiência de usuários diversos.

Segundo, o site ufsc.br representa um **caso típico de sistemas governamentais/institucionais**, que frequentemente sofrem dos mesmos problemas de IHC identificados em diversas organizações públicas. A análise deste sistema permite extrair lições aplicáveis a outros contextos similares.

Terceiro, a escolha fundamenta-se na **proximidade acadêmica**: como estudantes da UFSC, temos acesso direto aos usuários finais (colegas, professores, funcionários) e podemos validar as observações com experiências reais de uso.

## 1.2 Objetivos da Análise

Esta análise crítica tem como objetivos:

- **Identificar problemas reais de IHC** no site ufsc.br, fundamentados nas 10 Heurísticas de Usabilidade de Jakob Nielsen
- **Demonstrar aplicação prática** dos conceitos teóricos estudados em sala de aula
- **Propor correções fundamentadas** através de protótipos funcionais
- **Consolidar o aprendizado** sobre princípios de IHC aplicados a sistemas reais

## 1.3 Estrutura do Documento

Este documento apresenta, inicialmente, a contextualização do sistema analisado e a metodologia empregada. Em seguida, detalha cada problema identificado com evidências visuais, fundamentação teórica e propostas de correção. Finaliza com conclusões sobre a importância da análise de IHC no desenvolvimento de sistemas.

---

# 2. CONTEXTUALIZAÇÃO DO SISTEMA ANALISADO

## 2.1 Descrição do Sistema UFSC.br

O site institucional ufsc.br é o portal oficial da Universidade Federal de Santa Catarina, uma das principais instituições de ensino superior do Brasil. O sistema funciona como ponto central de acesso a informações institucionais, serviços acadêmicos e comunicação oficial da universidade.

## 2.2 Público-Alvo

O site atende a um público diversificado e heterogêneo:

- **Estudantes**: Buscam informações sobre cursos, matrículas, horários, editais
- **Servidores**: Professores, técnicos e funcionários administrativos
- **Comunidade externa**: Pais, empresas, pesquisadores, imprensa
- **Calouros**: Novos estudantes que precisam de informações básicas
- **Usuários internacionais**: Pesquisadores e estudantes estrangeiros

## 2.3 Propósito e Funcionalidades Principais

O sistema tem como propósito principal:

- **Divulgação institucional**: Apresentar a missão, visão e estrutura da UFSC
- **Serviços acadêmicos**: Acesso a sistemas como SIGAA, Moodle, bibliotecas
- **Comunicação**: Notícias, eventos, editais e comunicados oficiais
- **Navegação institucional**: Acesso a departamentos, centros e campi
- **Serviços à comunidade**: Restaurante universitário, assistência estudantil, etc.

## 2.4 Importância para a UFSC

Como interface principal entre a instituição e seus públicos, o site ufsc.br desempenha papel crucial na experiência institucional. Problemas de IHC neste sistema afetam não apenas a eficiência de tarefas, mas também a percepção da qualidade institucional da UFSC.

---

# 3. METODOLOGIA DE ANÁLISE

## 3.1 Abordagem Metodológica

A análise foi realizada através de uma abordagem mista, combinando:

### 3.1.1 Análise Heurística
- Aplicação sistemática das 10 Heurísticas de Usabilidade de Jakob Nielsen
- Avaliação criteriosa de cada aspecto da interface
- Identificação de violações específicas às heurísticas

### 3.1.2 Análise Técnica
- Inspeção do código HTML/CSS/JavaScript do site
- Verificação de conformidade com WCAG 2.1
- Avaliação de performance e responsividade

### 3.1.3 Pesquisa com Usuários
- Observação de usuários reais utilizando o sistema
- Coleta de feedback informal sobre dificuldades encontradas
- Validação de problemas com estudantes e servidores da UFSC

## 3.2 Critérios de Avaliação

Cada problema identificado foi avaliado segundo:

- **Gravidade**: Impacto na experiência do usuário (Crítica/Alta/Média/Baixa)
- **Frequência**: Como o problema ocorre (Sempre/Frequentemente/Ocasionalmente/Raramente)
- **Persistência**: Facilidade de detecção e correção

## 3.3 Ferramentas Utilizadas

- **Navegadores**: Chrome, Firefox, Edge para testes cross-browser
- **Ferramentas de acessibilidade**: WAVE, axe DevTools
- **Captura de tela**: Para documentação visual dos problemas
- **Análise de código**: Inspeção de elementos e validação HTML

---

# 4. PROBLEMAS IDENTIFICADOS

## Problema 1: Navegação Complexa e Sobrecarga Cognitiva

### Descrição do Problema
O menu principal do site apresenta uma estrutura hierárquica excessivamente complexa, com múltiplos níveis de navegação e uma quantidade massiva de opções simultâneas. O menu possui mais de 50 links diretos visíveis, organizados em categorias que não seguem uma lógica intuitiva para o usuário comum.

### Evidências Visuais
**Figura 1: Menu principal do site ufsc.br - sobrecarga de opções**
*[Inserir screenshot do menu principal mostrando os 50+ links]*

### Impacto na Experiência do Usuário
- **Sobrecarga cognitiva**: Usuários ficam paralisados pela quantidade de opções
- **Dificuldade de localização**: Informações importantes ficam "perdidas" na massa de links
- **Frustração**: Usuários precisam fazer múltiplos cliques para encontrar o que procuram
- **Abandono**: Usuários podem desistir de encontrar informações específicas

### Heurísticas Violadas
1. **Heurística #6 - Reconhecimento em vez de recordação**: Usuários precisam "lembrar" onde estão informações específicas
2. **Heurística #8 - Estética e design minimalista**: Interface sobrecarregada com informações
3. **Heurística #3 - Controle e liberdade do usuário**: Usuários se sentem perdidos na navegação

### Fundamentação Teórica
Conforme Nielsen (1994), interfaces devem minimizar a carga cognitiva do usuário, apresentando informações de forma clara e hierárquica. Norman (2013) enfatiza que a navegação deve seguir modelos mentais intuitivos, evitando estruturas que exijam conhecimento prévio do sistema.

### Proposta de Correção
**Figura 2: Menu simplificado proposto**
*[Inserir screenshot do protótipo corrigido]*

- Redução do menu principal de 50+ para 6 itens principais
- Criação de seção "Acesso Rápido" com 8 serviços mais utilizados
- Cards visuais com ícones para identificação rápida
- Busca destacada e acessível
- Estrutura hierárquica clara e intuitiva

### Demonstração da Correção
Link para protótipo: `pages/homepage/` - Implementação funcional da navegação corrigida.

---

## Problema 2: Falta de Feedback Visual em Interações

### Descrição do Problema
Muitos elementos interativos do site não fornecem feedback visual claro quando o usuário interage com eles. Botões não mudam de estado ao passar o mouse, links não indicam claramente que são clicáveis, e ações do usuário não geram confirmação visual imediata.

### Evidências Visuais
**Figura 3: Links sem feedback visual no site original**
*[Inserir screenshot mostrando links estáticos sem hover states]*

### Impacto na Experiência do Usuário
- **Incerteza**: Usuários não sabem se clicaram corretamente ou se o sistema está processando
- **Frustração**: Múltiplos cliques desnecessários em elementos que não respondem visualmente
- **Acessibilidade**: Usuários com deficiência visual têm dificuldade em identificar elementos interativos
- **Eficiência reduzida**: Usuários perdem tempo tentando entender o estado do sistema

### Heurísticas Violadas
1. **Heurística #1 - Visibilidade do status do sistema**: Sistema não comunica claramente seu estado
2. **Heurística #4 - Consistência e padrões**: Elementos interativos não seguem padrões visuais consistentes
3. **Heurística #7 - Flexibilidade e eficiência de uso**: Falta de affordances claras reduz eficiência

### Fundamentação Teórica
Nielsen (1994) destaca que o sistema deve sempre informar ao usuário o que está acontecendo através de feedback apropriado. Norman (2013) enfatiza a importância de affordances visuais claras que indiquem como os elementos podem ser manipulados.

### Proposta de Correção
**Figura 4: Estados hover implementados no protótipo**
*[Inserir screenshot mostrando hover states funcionais]*

- Estados hover, focus e active em todos os elementos interativos
- Transições CSS suaves para feedback visual
- Indicadores de foco visíveis para navegação por teclado
- Carrossel com indicadores ativos e controles visíveis
- Efeitos de elevação em cards ao passar mouse

### Demonstração da Correção
Link para protótipo: `pages/homepage/` - Ver estados hover e feedback visual implementados.

---

## Problema 3: Hierarquia Visual Inconsistente

### Descrição do Problema
A página inicial apresenta múltiplos elementos competindo pela atenção do usuário sem uma hierarquia visual clara. Títulos, textos, imagens e call-to-actions têm pesos visuais similares, dificultando a compreensão do que é mais importante.

### Evidências Visuais
**Figura 5: Elementos competindo pela atenção visual**
*[Inserir screenshot da homepage original mostrando falta de hierarquia]*

### Impacto na Experiência do Usuário
- **Confusão visual**: Usuários não sabem onde focar a atenção
- **Tempo de leitura aumentado**: Informações importantes não são encontradas rapidamente
- **Fadiga visual**: Múltiplos elementos competindo causam cansaço
- **Perda de informações importantes**: Conteúdo relevante pode passar despercebido

### Heurísticas Violadas
1. **Heurística #8 - Estética e design minimalista**: Interface não prioriza informações essenciais
2. **Heurística #6 - Reconhecimento em vez de recordação**: Falta de padrões visuais claros
3. **Heurística #4 - Consistência e padrões**: Hierarquia não é aplicada consistentemente

### Fundamentação Teórica
Preece et al. (2015) destacam que a hierarquia visual é fundamental para guiar a atenção do usuário e facilitar a compreensão. O uso adequado de tipografia, espaçamento e contraste cria uma "arquitetura visual" que orienta o usuário.

### Proposta de Correção
**Figura 6: Hierarquia visual clara no protótipo**
*[Inserir screenshot mostrando tipografia hierárquica e organização visual]*

- Carrossel hero com título grande e destaque visual
- Sistema de tipografia claro (H1-H6 com tamanhos distintos)
- Grid system consistente para organização
- Contraste e espaçamento adequados entre seções
- Elementos importantes destacados com cores e tamanhos

### Demonstração da Correção
Link para protótipo: `pages/homepage/` - Ver hierarquia visual aplicada.

---

## Problema 4: Problemas de Acessibilidade

### Descrição do Problema
O site apresenta problemas de acessibilidade que dificultam o uso por pessoas com deficiência. Alguns textos têm contraste insuficiente com o fundo, elementos não são navegáveis via teclado, e falta estrutura semântica adequada para leitores de tela.

### Evidências Visuais
**Figura 7: Texto com contraste insuficiente**
*[Inserir screenshot mostrando problemas de contraste]*

### Impacto na Experiência do Usuário
- **Exclusão**: Usuários com deficiência visual não conseguem usar o site adequadamente
- **Conformidade legal**: Site pode não estar em conformidade com leis de acessibilidade
- **Usabilidade geral reduzida**: Problemas de acessibilidade afetam todos os usuários
- **Frustração**: Usuários que dependem de navegação por teclado ficam presos

### Heurísticas Violadas
1. **Heurística #1 - Visibilidade do status do sistema**: Elementos não são visíveis para todos os usuários
2. **Heurística #7 - Flexibilidade e eficiência de uso**: Falta de alternativas de acesso
3. **Princípios WCAG**: Violação de critérios de contraste (1.4.3) e navegação por teclado (2.1.1)

### Fundamentação Teórica
As WCAG 2.1 estabelecem que textos devem ter contraste mínimo de 4.5:1 para texto normal e 3:1 para texto grande. Nielsen (1994) enfatiza que sistemas devem ser acessíveis a todos os usuários, independentemente de suas capacidades.

### Proposta de Correção
**Figura 8: Contraste e navegação por teclado corrigidos**
*[Inserir screenshot mostrando indicadores de foco e melhor contraste]*

- Contraste de cores aumentado (azul #003366 sobre branco)
- Navegação por teclado com indicadores de foco visíveis
- Estrutura HTML semântica (header, nav, section, footer)
- Labels descritivos em elementos interativos
- Suporte a leitores de tela melhorado

### Demonstração da Correção
Link para protótipo: `pages/homepage/` - Testar acessibilidade implementada.

---

## Problema 5: Linguagem Técnica Não Adequada

### Descrição do Problema
O site utiliza terminologia técnica e jargão acadêmico sem explicações adequadas, assumindo que todos os usuários estão familiarizados com a estrutura organizacional da universidade. Termos como "PROEX", "PROGRAD", "CAGR" aparecem sem contexto.

### Evidências Visuais
**Figura 9: Siglas sem contexto no menu de navegação**
*[Inserir screenshot mostrando siglas técnicas no menu]*

### Impacto na Experiência do Usuário
- **Barreira de compreensão**: Usuários não entendem o que cada seção oferece
- **Frustração**: Necessidade de pesquisar termos para entender o site
- **Exclusão**: Usuários menos familiarizados com ambiente acadêmico se sentem excluídos
- **Ineficiência**: Múltiplos cliques para descobrir o significado de termos

### Heurísticas Violadas
1. **Heurística #2 - Compatibilidade com o mundo real**: Linguagem não corresponde ao conhecimento do usuário
2. **Heurística #6 - Reconhecimento em vez de recordação**: Usuários precisam "lembrar" o que cada sigla significa
3. **Heurística #10 - Ajuda e documentação**: Falta de explicações contextuais

### Fundamentação Teórica
Norman (2013) enfatiza que sistemas devem usar linguagem familiar ao usuário, seguindo convenções do mundo real. Nielsen (1994) destaca que informações devem aparecer em ordem natural e lógica para o usuário.

### Proposta de Correção
**Figura 10: Linguagem do usuário no menu corrigido**
*[Inserir screenshot mostrando nomes descritivos no menu]*

- Menu principal usa linguagem do usuário ("Ensino", "Pesquisa", "Extensão")
- Seção "Acesso Rápido" com nomes descritivos completos
- Textos introdutórios em linguagem clara e acessível
- Eliminação de siglas desnecessárias no menu principal
- Contexto fornecido para termos técnicos quando necessário

### Demonstração da Correção
Link para protótipo: `pages/homepage/` - Ver linguagem adequada implementada.

---

## Problema 6: Falta de Prevenção de Erros em Formulários

### Descrição do Problema
Formulários do site não possuem validação em tempo real, mensagens de erro claras, ou prevenção de erros comuns. Usuários só descobrem problemas após submeter o formulário, e mensagens de erro não são suficientemente descritivas.

### Evidências Visuais
**Figura 11: Formulário sem validação em tempo real**
*[Inserir screenshot de formulário do site original]*

### Impacto na Experiência do Usuário
- **Frustração**: Usuários precisam refazer formulários inteiros após descobrir erros
- **Perda de tempo**: Validação apenas no final do processo
- **Abandono**: Usuários podem desistir de preencher formulários longos
- **Confusão**: Mensagens de erro não explicam claramente como corrigir

### Heurísticas Violadas
1. **Heurística #5 - Prevenção de erros**: Sistema não previne erros antes que ocorram
2. **Heurística #9 - Ajudar usuários a reconhecer, diagnosticar e recuperar erros**: Mensagens de erro não são claras
3. **Heurística #1 - Visibilidade do status do sistema**: Validação não é visível durante o preenchimento

### Fundamentação Teórica
Nielsen (1994) destaca que é melhor prevenir erros do que depender de mensagens de erro. Validação em tempo real e feedback imediato reduzem frustração e aumentam eficiência. Preece et al. (2015) enfatizam a importância de mensagens de erro construtivas que guiem o usuário.

### Proposta de Correção
**Figura 12: Validação em tempo real implementada**
*[Inserir screenshot do formulário corrigido]*

- Validação em tempo real implementada
- Máscaras de entrada para CPF e telefone
- Mensagens de erro descritivas e acionáveis
- Feedback visual durante preenchimento
- Prevenção de erros comuns através de design

### Demonstração da Correção
Link para protótipo: `pages/codigo-validacao.html` - Ver código de validação implementado.

---

## Problema 7: Inconsistência Visual e de Padrões

### Descrição do Problema
O site apresenta inconsistências visuais entre diferentes páginas e seções. Botões têm estilos diferentes, espaçamentos variam, cores não seguem um padrão consistente, e elementos similares se comportam de forma diferente em contextos distintos.

### Evidências Visuais
**Figura 13: Inconsistências visuais entre páginas**
*[Inserir screenshot comparativo mostrando diferenças de estilo]*

### Impacto na Experiência do Usuário
- **Confusão**: Usuários não sabem o que esperar de elementos similares
- **Curva de aprendizado aumentada**: Cada página parece um novo sistema
- **Frustração**: Comportamentos inesperados quebram expectativas
- **Percepção de qualidade reduzida**: Inconsistência transmite falta de cuidado

### Heurísticas Violadas
1. **Heurística #4 - Consistência e padrões**: Interface não segue padrões consistentes
2. **Heurística #6 - Reconhecimento em vez de recordação**: Falta de padrões dificulta reconhecimento
3. **Heurística #3 - Controle e liberdade do usuário**: Inconsistência reduz sensação de controle

### Fundamentação Teórica
Nielsen (1994) enfatiza que usuários não devem se perguntar se palavras, situações ou ações diferentes significam a mesma coisa. Consistência reduz carga cognitiva e aumenta eficiência. Norman (2013) destaca que padrões consistentes criam affordances previsíveis.

### Proposta de Correção
**Figura 14: Design system consistente aplicado**
*[Inserir screenshot mostrando consistência visual]*

- Design system centralizado
- Paleta de cores consistente (azul UFSC #003366)
- Componentes reutilizáveis (botões, formulários, cards)
- Espaçamentos padronizados
- Tipografia consistente em toda a interface

### Demonstração da Correção
Link para protótipo: `pages/homepage/` - Ver design system consistente.

---

# 5. CONCLUSÃO

## 5.1 Síntese dos Achados

Esta análise crítica do site ufsc.br demonstrou que mesmo sistemas institucionais consolidados podem apresentar problemas significativos de IHC. Os 7 problemas identificados - desde navegação complexa até inconsistências visuais - impactam diretamente a experiência de usuários diversos, desde calouros até servidores experientes.

## 5.2 Importância da Análise de IHC

A experiência prática desta atividade reforça a importância da análise de IHC no desenvolvimento de sistemas:

### 5.2.1 Impacto na Usabilidade
Problemas de IHC não são meramente estéticos, mas impactam diretamente a eficiência, satisfação e sucesso na realização de tarefas. A navegação complexa identificada, por exemplo, pode impedir que usuários encontrem informações críticas.

### 5.2.2 Benefícios da Correção
As correções propostas demonstram que melhorias de IHC são viáveis e trazem benefícios imediatos: redução da carga cognitiva, aumento da acessibilidade, melhoria da eficiência e satisfação do usuário.

### 5.2.3 Aplicabilidade Geral
Os problemas identificados no ufsc.br são comuns em sistemas governamentais e empresariais. As soluções propostas podem ser aplicadas em diversos contextos, desde sites institucionais até aplicações corporativas.

## 5.3 Lições Aprendidas

Esta atividade consolidou importantes aprendizados:

1. **Teoria-Prática**: Princípios abstratos das heurísticas de Nielsen ganham concretude quando aplicados a sistemas reais.

2. **Pensamento Crítico**: Identificar problemas requer não apenas conhecimento técnico, mas também empatia com usuários e compreensão de contextos de uso.

3. **Iteração de Design**: Melhorias de IHC são processos iterativos que requerem prototipagem, teste e refinamento.

4. **Acessibilidade Universal**: Problemas de IHC frequentemente impactam usuários com deficiência, reforçando a importância do design inclusivo.

## 5.4 Recomendações Finais

Para a UFSC e outras instituições similares, recomenda-se:

- **Auditorias Regulares**: Análises periódicas de IHC para identificar problemas emergentes
- **Design Systems**: Implementação de sistemas de design consistentes e acessíveis
- **Testes com Usuários**: Validação de mudanças com usuários reais antes da implementação
- **Formação Contínua**: Treinamento da equipe de desenvolvimento em princípios de IHC

Esta experiência prática demonstrou que IHC não é um luxo, mas uma necessidade fundamental para sistemas que pretendem servir usuários de forma efetiva e inclusiva.

---

# 6. REFERÊNCIAS

KRUG, Steve. **Don't Make Me Think, Revisited: A Common Sense Approach to Web Usability**. 3. ed. Berkeley: New Riders, 2014.

NIELSEN, Jakob. **10 Usability Heuristics for User Interface Design**. Nielsen Norman Group, 1994. Disponível em: https://www.nngroup.com/articles/ten-usability-heuristics/. Acesso em: 15 nov. 2025.

NORMAN, Donald A. **The Design of Everyday Things: Revised and Expanded Edition**. New York: Basic Books, 2013.

PREECE, Jennifer; ROGERS, Yvonne; SHARP, Helen. **Interaction Design: Beyond Human-Computer Interaction**. 5. ed. Chichester: John Wiley & Sons, 2015.

SHNEIDERMAN, Ben; PLAISANT, Catherine; COHEN, Maxine; JACOBS, Steven; ELMQVIST, Niklas. **Designing the User Interface: Strategies for Effective Human-Computer Interaction**. 6. ed. Boston: Pearson, 2016.

WORLD WIDE WEB CONSORTIUM (W3C). **Web Content Accessibility Guidelines (WCAG) 2.1**. W3C Recommendation, 2018. Disponível em: https://www.w3.org/WAI/WCAG21/quickref/. Acesso em: 15 nov. 2025.

---

**Link do Protótipo:** [Inserir link do GitHub Pages/GitHub Repo público]

**Data de entrega:** 01/12/2025

**Palavras-chave:** IHC, Usabilidade, Acessibilidade, Análise Heurística, Design de Interface, UFSC
