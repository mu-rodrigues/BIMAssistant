# Roadmap

## Fase 1 - Fundamentos

- [x] Definição da ideia
- [x] Criação do GitHub
- [x] Estruturação inicial do projeto
- [x] Instalar Git
- [x] Aprender GitHub Flow
- [ ] Aprender C#

## Fase 2 - Desenvolvimento Base

- [ ] Primeiro projeto C#
- [ ] Primeiro programa funcional
- [ ] Estrutura do plugin Revit
- [ ] Integração com Revit API

## Fase 3 - MVP

- [ ] Find and Replace
- [ ] Interface gráfica
- [ ] Integração IA
- [ ] Demonstração interna

## Fase 4 - Evolução

- [ ] Biblioteca
- [ ] Atualização de famílias
- [ ] Criação de schedules
- [ ] Quantitativos
- [ ] Filtros automáticos

# Aprendizados Importantes

## Lembretes

- Resolver problemas antes de adicionar IA.
- Criar funcionalidades primeiro.
- A IA apenas utiliza funcionalidades existentes.
- Priorizar simplicidade.
- Construir um MVP antes do produto final.

# Histórico de Decisões

## 23/11/2026

### Decisão 001

Não utilizar MCP na primeira versão.

Motivo:

Complexidade desnecessária para os objetivos iniciais.

### Decisão 002

A IA será responsável apenas pela interpretação dos comandos.

A execução será realizada pelo plugin.

### Decisão 003

O MVP será baseado em Find and Replace de parâmetros.

Motivo:

Função simples, demonstrável e com potencial para integração com IA.

### Decisão 004

O projeto permanecerá público durante a fase de estudos.

Motivo:

Não existem informações proprietárias sendo utilizadas neste estágio.

## 24/11/2026

### Decisão 005

O aprendizado de programação será tratado separadamente do desenvolvimento do BIM Assistant.

Motivo:

Conhecimentos fundamentais de C# pertencem ao desenvolvedor e não ao produto, evitando que o repositório principal seja utilizado como ambiente de estudos genéricos.

### Decisão 006

A inteligência artificial será considerada uma camada complementar do sistema.

Motivo:

As funcionalidades devem existir e funcionar independentemente da presença da IA.

A IA será responsável por interpretar solicitações e direcionar comandos para funcionalidades já implementadas no plugin.

### Decisão 007

A arquitetura inicial utilizará o fluxo:

Usuário → Interface → Plugin → Revit API

e futuramente:

Usuário → IA → Plugin → Revit API

Motivo:

Reduzir complexidade nas fases iniciais e permitir evolução gradual da solução.
