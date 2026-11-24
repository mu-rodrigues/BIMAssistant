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


### Decisão 008

Não criar o arquivo ARCHITECTURE.md neste momento.

Motivo:

A arquitetura atual é simples e já está adequadamente documentada no Master Document. A criação de um documento dedicado neste estágio aumentaria a burocracia sem gerar ganho real para o projeto.

### Decisão 009

Iniciar o desenvolvimento do primeiro projeto C# do BIM Assistant focado exclusivamente na lógica da funcionalidade de pesquisa e substituição, sem dependência da Revit API.

Motivo:

Permitir aprendizado gradual de C# enquanto se desenvolve uma funcionalidade real do produto.

### Decisão 010

As especificações detalhadas das funcionalidades serão mantidas e evoluídas dentro do arquivo FEATURES.md.

Motivo:

Neste estágio do projeto, a complexidade ainda não justifica a criação de documentos específicos para cada funcionalidade.

A documentação deverá evoluir junto com o desenvolvimento, priorizando implementação e validação prática.