# BIM Assistant - Master Document

## Informações Gerais

**Nome do Projeto:** BIM Assistant

**Tipo:** Plug-in para Autodesk Revit

**Linguagem Principal:** C#

**Ambiente de Desenvolvimento:** Visual Studio Code

**Controle de Versão:** Git + GitHub

**Status:** Estudo e Prototipação

## Visão do Projeto

O BIM Assistant é um plug-in para Autodesk Revit desenvolvido com foco em automação de tarefas, gerenciamento de bibliotecas e assistência técnica ao usuário.

A inteligência artificial deve atuar como uma camada complementar do sistema, auxiliando na execução e interpretação de comandos, sem substituir as funcionalidades implementadas pelo próprio plug-in.

O objetivo é reduzir tarefas repetitivas, facilitar a manipulação de dados e fornecer suporte técnico contextualizado para usuários de diferentes níveis de experiência.

## Problema que o Projeto Busca Resolver

Durante o desenvolvimento de projetos em Revit existem diversas atividades repetitivas e suscetíveis a erros humanos, como:

- Alteração de parâmetros em massa
- Criação de tabelas
- Organização de bibliotecas
- Carregamento de famílias
- Atualização de famílias
- Configuração de filtros
- Verificação de inconsistências
- Extração de quantitativos

Atualmente essas tarefas exigem grande quantidade de trabalho manual, experiência do usuário e conhecimento da ferramenta.

## Objetivo Principal

Criar um assistente BIM capaz de conectar:

Usuário → Inteligência Artificial → Plugin → Revit API → Modelo

permitindo que o usuário utilize linguagem natural para executar funcionalidades desenvolvidas dentro do próprio plugin.

## Filosofia do Projeto

A IA não executa ações diretamente no Revit.

A IA atua como interpretadora de comandos.

### Arquitetura Inicial

Fluxo simplificado previsto para o projeto:

Usuário
↓
Interface do Plugin
↓
Camada de Comandos
↓
Revit API
↓
Modelo Revit

Fluxo com IA:

Usuário
↓
Chat BIM Assistant
↓
Interpretador de Linguagem Natural
↓
Camada de Comandos
↓
Revit API
↓
Modelo Revit

### Exemplo:

>
>> Usuário:
>>
>> "Troque o valor do parâmetro Sistema de 'EL' para 'ELETRICO'."
>
>> IA:
>>
>> "Entendi. Deseja executar uma substituição do parâmetro Sistema?"
>
>> Usuário
>>
>> "Sim."
>
> Plugin:
>
> Executa a modificação após confirmação.
>

## Funcionalidades Planejadas

### Biblioteca

#### Famílias

Permitir a busca, carregamento e atualizações de famílias diretamente da biblioteca.

Status: Em estudo

#### Tags

Permitir localizar famílias através de palavras-chave.

Exemplo:

*estrutura*

*elétrica*

*hidráulica*

Status: Em estudo

---

### Parâmetros

#### Localização e Substituição

Localizar e substituir valores de parâmetros.

Status: Em desenvolvimento (MVP)[^1]

[^1]: MVP ou Produto Mínimo Viável, é a menor versão de um projeto que resolve um problema real de ponta a ponta para um usuário. Não é sistema pela metade: é o mínimo necessário para a solução de um único problema.

#### Criação

Criar parâmetros a partir de arquivos compartilhados.

Status: Em estudo

#### Inserção

Adicionar parâmetros automaticamente em famílias selecionadas.

Status: Em estudo

---

### Tabelas

#### Criação

Gerar tabelas automaticamente.

Status: Em estudo

#### Quantitativos

Gerar relatórios quantitativos.

Status: Em estudo

#### Exportação

Exportar dados para planilhas.

Status: Em estudo

---

### MEP

### Interferências

Analisar conflitos entre elementos.

Status: Em estudo

### Conectividade

Validar conexões entre componentes.

Status: Em estudo

### Inconsistências

Detectar elementos com parâmetros incorretos ou ausentes.

Status: Em estudo

---

### Inteligência Artificial

#### Assistente Conversacional

Chat integrado ao plugin.

Status: Planejado

#### Explicações

Explicar funcionalidades do Revit.

Status: Em estudo

#### Processos

Ensinar processos BIM.

Status: Em estudo

#### Linguagem Natural

Transformar comandos em ações do plugin.

Status: Planejado

#### Consulta de Documentação

Permitir consultas contextualizadas sobre o Revit utilizando documentação oficial da Autodesk.

Exemplos:

- Como utilizar parâmetros compartilhados?
- Como funcionam schedules?
- Como criar filtros de vista?
- Explicação de ferramentas da versão utilizada pelo usuário.

Status: Planejado

## Primeira Demonstração

Objetivo:

Demonstrar a viabilidade da utilização de IA integrada ao Revit.

Escopo:

- Interface simples.
- Ferramenta de Find and Replace.
- Chat com IA.
- Interpretação de linguagem natural.
