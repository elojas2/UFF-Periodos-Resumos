# Aula 1


O que é engenharia de software?

	abordagem sistematica, disciplinada e quantificavel ao desenvolvimento, operacao e manutencao de software


Software x Hardware

	Hardware -> manufaturado
		- alto custo de reprodução 
		- pode enguiçar 
		- defeitos podem vir tanto da concepção quanto da produção 
		- pode ser substituido na totalidade ou em partes
	
	Software -> desenvolvido
		- alto custo de criação 
		- baixo custo de reprodução 
		- não enguiça, mas deteriora
		- defeitos no produto usualmente sao consequencias de problemas no processo de desenvolvimento 


Elementos da ES

	Processo
		- Define os passos gerais para desenvolvimento e manutenção do software
		- serve como uma estrutura de encadeamento de metodos e ferrramentas

	Metodos
		- sao os how to's de como fazar um passo especifico do processo

	Ferramentas
		- automatizam o processo e os metodos


Ciclo de vida Cascata

	- Comunicacao
		- planejamento
			- modelagem
				- construcao
					- implantacao
	
	Util quando os requisitos sao estaveis e bem definidos / Nao lida bem com incertezas / Fornece pouca visibilidade do estado do projeto (muito tempo para a primeira entrega e dificuldade para ter feedback do cliente)


Ciclo de vida Incremental

	 Coloca grafico
				comunicacao->planejamento->modelagem->construcao->implantacao
		comunicacao->planejamento->modelagem->construcao->implantacao
	comunicacao->planejamento->modelagem->construcao->implantacao
	 
	* Faz entregas incrementais do software (cada incremento eh construido via um mini cascata / cada inscremento eh um software operacional)
	* Versoes anteriores ajudam a refinar o plano (feedback constante)
	* Diminuicao da ansiedade do cliente


Ciclo de vida RAD


	Funcionamento equivalente ao cascata mas ele tem algumas diferencas como

	Visa entregar o sistema completo em 60 a 90 dias
	 Multiplas equipes trabalham em paralelo na modelagem e construcao
	 Assume a existencia de componentes reutilizaveis e geracao de codigo

	  Difil de ser utilizado em dominios novos ou instaveis


Prototipagem

	Utilizado como auxilio a outros modelo de ciclo de vida
	
	Bem util 
		- para validar um requisito obscuro com o cliente 
		- verificar o desempenho de um algoritmo especifico

	Deveria ser jogado fora no final
		- Prototipos nao sao produtos
		- Usualmente os clientes desejam colocar prototipos em producao


Ciclo de vida Espiral

	Foco principal no gerenciamento de riscos
	A cada ciclo 
		- o conhecimento aumenta
		- o planejamento é refinado
		- produto gerado no ciclo anterior é evoluído (nao jogado fora)
	 
	Cada ciclo evolui o sistema, mas nao necessariamente entrega um software operacional
		- modelo em papel
		- prototipo
		- versoes do produto
		- etc