Vaga: Desenvolvedor Delphi

Avaliação Remota

# Etapa 1: Avaliação de Conhecimentos em SQL

	Estrutura do Banco de Dados:
	
	Utilize a versão gratuita do SQL Server (Express) - disponivel em https://www.microsoft.com/pt-br/sql-server/sql-server-downloads
	
	Crie uma estrutura de banco de dados com no mínimo 4 tabelas, cada uma contendo:

		a) Chave primária.

		b) Chave estrangeira.

		c) CONSTRAINT para validar um campo inteiro para ser maior que zero (quando necessário).

		d) Campo DATETIME com valor default para o momento da inserção.
		
		e) Tabelas básicas:
			-> Obra
				Campos básicos:
					ID da Obra (Chave primária)
					Nome da Obra (varchar)
					Código ISWC (varchar)					
					Idioma (varchar)
					Data de Lancamento (datetime)
					Data de Inclusão (datetime)
					* Obs: Uma obra poderá ser composta por vários titulares.
						   Uma obra poderá ser ter vários fonogramas. 	
						
			-> Fonograma
				Campos básicos:
					ID do Fonograma (Chave primária)
					Nome do Fonograma (varchar)
					Código ISRC (varchar)
					Duracao min (int)
					Duracao seg (int)
					Data de Inclusão (datetime)
					Flag para indicar ser é nacional ou estrangeira (char)					
					ID da Obra (Chave estrangeira referenciando a tabela de Obra)
					* Obs: Um fonograma poderá ter apenas uma obra.
					
			-> Titular
				Campos básicos:
					ID do Titular (Chave primária)
					Nome do Titular (varchar)
					Nacionalidade (varchar)
					Data de Nascimento (datetime)
					CPF (varchar)
					Sexo (char)
					Estado Civil (char)
					Lougradouro (varchar)
					Numero (varchar)
					Complemento (varchar)
					Bairro (varchar)
					CEP (varchar)
					Cidade (varchar)
					UF (varchar)
					Pais (varchar)
					Data de Inclusão (datetime)
					Flag para indicar se o titular estar ativo (char)
					* Obs: Um titular poderá compor várias obras.


	Inserção de Registros de Exemplo:

		Insira registros de exemplo em todas as tabelas criadas.

	Scripts para Consultas:

		a) Retorne 10 registros da tabela que possui o campo DATETIME ordenado de forma decrescente.

		b) Retorne todos os registros de todas as tabelas utilizando JOIN.

		c) Delete todos os registros da tabela que possui o campo DATETIME que foram inseridos em um determinado intervalo de horas.
		
		d) Delete todos os fonogramas de um titular.


# Etapa 2: Avaliação de Lógica

	Elabore um algoritmo, utilizando pseudolinguagem (ou mesmo pascal), que ao receber um número qualquer apresente a soma do próprio número com os 100 subsequentes.


# Etapa 3: Avaliação de Conhecimentos de Sintaxe do Delphi

	Prático

	- Desenvolvimento de um Programa em Delphi:

		Crie um programa em Delphi com uma tela de cadastro contendo as funcionalidades de Inserir, Editar e Apagar, confirmados pelos botões "Gravar" e "Cancelar". 
		Use a tabela "TITULAR" criada na etapa 1.

	- Recursos Adicionais no Programa:

		-> Desenvolva a tela "Main" do projeto com um componente "MainMenu", contendo a opção "Cadastro" e sub-opção "Titulares...".

		-> Utilize um "Data Module" para conectar-se com o BD, sendo o meio de ligação entre os componentes de consulta e execução e o BD.

		-> Realize as validações:

			Nome preenchido.

			Validação do formato e validade da data, se preenchidas.

			O componente que captura o sexo do titular só pode aceitar os caracteres "M" ou "F".

			Não permitir inserção de um nome já existente no BD, emitindo um alerta ao usuário.

		-> Tela Base de Cadastro:

			Crie uma tela base de cadastro que servirá de herança para a tela de cadastro de titulares. 
			Esta tela terá um DataSet e, no mínimo, os botões básicos (Inserir, Editar e Apagar). 
			O botão "Apagar" deve ter sua funcionalidade programada nesta tela base, deletando o registro vigente no DataSet.

	    -> Utilize uma API para preencher o endereço do titular ao digitar o CEP.
		   Pode usar API "ViaCEP" https://viacep.com.br/


# Etapa 4: Entrega do Desafio

	-> A entrega de todas as etapas deverão ser versionado no github (https://github.com/Uniao-brasileira-dos-Compositores/desafio-analista-delphi),
	   bem como um backup zipado do banco de dados.
   
   
- Prazo de Resposta: 3 dias.

**IMPORTANTE**: Crie um repositorio no github e envio o link para avaliação.
