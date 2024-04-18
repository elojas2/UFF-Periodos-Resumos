# Aula 2


### Analise vs Projeto


#### Principais funcoes

	Analise
		- identificar as funcionalidades e entidades do sistema
		- encontrar abstracoes adequadas para representar o problema

	Projeto
		- atribuir responsabilidades as entidades do sistema
		- encontrar abstracoes adequadas para representar a solucao


## Requisitos de um sistema

    - Descricoes/restricoes dos servicoes que o sistema deve prestar a sua operacao
    - Reflete as necessidades dos clientes 


#### Engenharia de Requisitos

    - Processo de descoberta, analise, documentacao e conferencia desses servicoes e restricoes

####    Requisitos de usuarios vs Requisitos de sistema
                    Usuarios                    |              Sistema             
    ______________________________________________________________________________
    Declaracoes em linguagem natural            | Descricao detalhada do que o
    acompanhando de diagramas sobre o que       | Sistema deve fazer, podendo
    o usuario deve esperar do sistema.          | ter infos tecnicas. Escritas   
    Escritos da perspectiva do usuario final,   | a partir da perspectiva do
    descrevendo o que o sistema *deve*          | desenvolvedor.
    fazer e não *como* fazer.                   |




####    Requisitos funcionais vs Requisitos nao funcionais
    
```
                Funcionais             |            Não funcional
    ------------------------------------------------------------------------        
    São funcionalidades que um sistema | Caracteristicas que o sistema deve  
    deve ser capaz de executar.        | ter mas que não estão diretamente
    Exemplo: O sistema deve permitir   | relacionadas à funcionalidade especifica 
    que o usuario logue com um nome    | do sistema. Exemplos: Seguranca, 
    de usuario e senha.                | usabilidade, conformidade...
                                       | Para ficar mais claro, algo nao funcional é 
                                       | um sistema ser capaz de suportar 1000
                                       | simultaneos. Outro exemplo é o sistema 
                                       | criptografar senhas de usuarios para 
                                       | garantir segurança.
```     
     
    
    
####    Alguns exemplos:
        Requisito do produto
            - sistema ficar disponivel para todas as unidades durante o expediente normal (segunda-sexta, 8:30h-17:30h)
            - tempo do sistema off não pode passar de 5 segundos em qualquer dia

        Requisito organizacional
            - uso do sistema deve ser restrito aos funcionaios da empresa
        
        Requisito externo
            - deve garantir privacidade do usuario, engual diz a LGPD
    

#### Elicitação

    Tem como objetivo entender o que o cliente espera do software, porém
    surge problemas como incertezas do cliente, volatibilidade dos requisitos.


#### Tecnicas de Elicitação

* Entrevistas
* Workshops
* Reunioes de brainstorming
* Prototipacao
* Pesquisa de mercado
* Analise de documentacao existente
