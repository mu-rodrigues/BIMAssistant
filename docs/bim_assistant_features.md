# Funcionalidades

## Localização e Troca

### Objetivo

Permitir a localização, filtragem, análise e alteração de elementos do projeto através de diferentes critérios de pesquisa.

A funcionalidade servirá como base para futuras ferramentas do BIM Assistant, incluindo operações de substituição de parâmetros, validações automáticas e comandos assistidos por IA.

### Visão Geral

Diferente de uma ferramenta tradicional de "Find and Replace", o BIM Assistant deverá funcionar como um sistema avançado de pesquisa e seleção de elementos.

O objetivo é permitir que o usuário encontre conjuntos específicos de elementos através de filtros sucessivos antes de executar qualquer ação.

Fluxo esperado:

Pesquisa → Filtragem → Validação → Ação

### Pesquisa

---

#### Método 1 - Pesquisa por Parâmetro

Permitir localizar elementos através de parâmetros.

Exemplos:

- Sistema = Elétrico
- Fabricante = Empresa X
- Ocupação > 40%
- Descrição contém "Cabeamento"

Status: Em desenvolvimento

---

#### Método 2 - Pesquisa por Categoria

Permitir localizar todos os elementos de uma categoria específica.

Exemplos:

- Portas
- Janelas
- Conduítes
- Tubulações
- Eletrocalhas

Status: Em desenvolvimento

---

#### Método 3 - Pesquisa por Elemento Selecionado

Permitir utilizar um elemento existente como referência para pesquisa.

Fluxo:

1. Usuário seleciona um elemento.
2. O sistema identifica suas características.
3. O sistema pesquisa elementos semelhantes.

Exemplo:

Usuário seleciona:

- Categoria: Porta
- Família: Porta de Madeira Bruta
- Largura: 0,80m
- Altura: 2,10m

O sistema procura elementos equivalentes.

Status: Planejado

##### Critérios de Comparação

Durante a pesquisa por elemento de referência, o usuário poderá definir quais informações serão consideradas.

###### Apenas Parâmetros da Família

Compara apenas dados pertencentes à família.

Exemplo:

- Altura
- Largura
- Material

Status: Planejado

###### Apenas Parâmetros de Projeto

Compara apenas informações preenchidas no projeto.

Exemplo:

- Sistema
- Pavimento
- Setor

Status: Planejado

###### Ambos

Combina parâmetros da família e do projeto.

Status: Planejado

---

### Sistema de Filtros

A pesquisa poderá receber filtros de acordo com os métodos apresentados, conforme o próprio sistema de filtros do Revit e sistema de pesquisa do Navisworks.

### Resultados da Pesquisa

Após a execução da pesquisa o sistema deverá apresentar:

- Quantidade de elementos encontrados;
- Lista dos elementos;
- Categoria;
- Família;
- Tipo;
- Parâmetros relevantes.

Status: Em desenvolvimento

### Operações

Após localizar os elementos, o usuário poderá executar ações.

---

#### Substituição de Valores

Replace tradicional.

Exemplo:

Sistema

EL

↓

ELETRICO

Status: Em desenvolvimento

---

#### Alteração de Parâmetros em Massa

Modificar um parâmetro em todos os elementos encontrados.

Status: Planejado

---

#### Seleção de Elementos

Selecionar automaticamente os elementos encontrados dentro do projeto.

Status: Planejado

---

#### Isolamento em Vista

Destacar ou isolar elementos encontrados.

Status: Futuro

---

### Integração com IA

A IA deverá utilizar esta funcionalidade como ferramenta interna.

Exemplo:

>> Usuário:
>>
>> "Encontre todos os conduítes com Sistema igual a 'EL'."
>
> IA:
>
> Executa uma pesquisa utilizando os filtros disponíveis.

---

>> Usuário:
>>
>> "Troque 'EL' por 'ELETRICO'."
>
> IA:
>
> Utiliza os resultados encontrados e executa a operação de substituição após confirmação do usuário.
