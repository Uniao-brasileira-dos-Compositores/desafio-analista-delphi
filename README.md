
# Vaga: Desenvolvedor Delphi

## Avaliação Remota

### Etapa 1: Avaliação de Conhecimentos em SQL

#### Estrutura do Banco de Dados

Crie uma estrutura de banco de dados com no mínimo 4 tabelas, cada uma contendo:
- a) Chave primária.
- b) Chave estrangeira.
- c) CONSTRAINT para validar um campo inteiro para ser maior que zero.
- d) Campo `DATETIME` com valor default para o momento da inserção.

#### Inserção de Registros de Exemplo

Insira registros de exemplo em todas as tabelas criadas.

#### Scripts para Consultas

1. Retorne 10 registros da tabela que possui o campo `DATETIME` ordenado de forma decrescente.
2. Retorne todos os registros de todas as tabelas utilizando `JOIN`.
3. Delete todos os registros da tabela que possui o campo `DATETIME` que foram inseridos em um determinado intervalo de horas.

### Etapa 2: Avaliação de Lógica

Elabore um algoritmo, utilizando pseudolinguagem, que ao receber um número qualquer apresente a soma do próprio número com os 100 subsequentes.

### Etapa 3: Avaliação de Conhecimentos de Sintaxe do Delphi

#### Prático

##### Desenvolvimento de um Programa em Delphi

Crie um programa em Delphi com uma tela de cadastro contendo as funcionalidades de Inserir, Editar e Apagar, confirmados pelos botões "Gravar" e "Cancelar". Uma tabela no banco de dados SQL Server deve ser criada com o nome de `funcionarios`.

##### Recursos Adicionais no Programa

- Desenvolva a tela "Main" do projeto com um componente `MainMenu`, contendo a opção "Cadastro" e sub-opção "Funcionários...".
- Utilize um `Data Module` para conectar-se com o BD, sendo o meio de ligação entre os componentes de consulta e execução e o BD.

##### Realize as Validações

- Nome preenchido.
- Validação do formato e validade da data, se preenchidas.
- O componente que captura o sexo do funcionário só pode aceitar os caracteres "M" ou "F".
- Não permitir inserção de um nome já existente no BD, emitindo um alerta ao usuário.

##### Tela Base de Cadastro

Crie uma tela base de cadastro que servirá de herança para a tela de cadastro de funcionários. Esta tela terá um DataSet e, no mínimo, os botões básicos (Inserir, Editar e Apagar). O botão "Apagar" deve ter sua funcionalidade programada nesta tela base, deletando o registro vigente no DataSet.

##### Acrescentar Obra, Fonograma e Titular

Adicione à estrutura do banco de dados as tabelas de Obra, Fonograma e Titular, incluindo as relações necessárias com as outras tabelas.

###### Campos para Tabela de Obra

- ID_Obra (Chave primária)
- Nome_Obra (varchar)
- Data_Lancamento (datetime)
- ID_Titular (Chave estrangeira referenciando a tabela de Titular)

###### Campos para Tabela de Fonograma

- ID_Fonograma (Chave primária)
- Nome_Fonograma (varchar)
- Duracao (int)
- ID_Obra (Chave estrangeira referenciando a tabela de Obra)

###### Campos para Tabela de Titular

- ID_Titular (Chave primária)
- Nome_Titular (varchar)
- Nacionalidade (varchar)
- Data_Nascimento (datetime)

#### Observações

- Envie as fontes e um backup do banco de dados compactados.
- Prazo de Resposta: 3 dias.

**IMPORTANTE**: Crie um repositorio no github e envio o link para avaliação.
