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

#### Tipos de requisitos de Elicitação

Normal:
* cliente lembra de falar
* cliente espera encontrar esse requisito no sistema

Requisito esperado:
* requisito implicito
* cliente nao lembra de falar
* cliente ficara insatisfeito se o requisito nao estiver no sistema

Requisito excitante:
* cliente nao lembra de falar
* cliente nao espera encontrar esse requisito no sistema
* cliente ficara satisfeito se esse requisito estiver no sistema


Elicitacao - escolha dos usuarios fonte

* lembre-se que a regra de Pareto (80-20) aparenta ser valida
    - 20% dos requisitos satisfazem a 80% dos usuarios
    - escolher um usuario muito especialista pode levar a priorizacao de requisitos que nunca serao utilizados


##### Requisitos funcionais


* Narrativa livre -> sistema deve mostrar uma mensagem de status


* Requisitos nao funcionais = atributos de qualidade



* Disponibilidade
     - O sistema deve ficar disponivel 99,5% do tempo nos dias uteis


* Eficiencia
     - em condicoes de pico de uso, deve ter uma reserva de 25% de capacidade de processamento e memoria


* Flexibilidade
     - Um novo tipo de sensor deve poder ser configurado no sistema em menos de 3 horas 


* Integridade
     - Transacoes historicas dos consumidores so poderao ser vistas por usuarios com privigelios de "auditor"


* Interoperabilidade
     - O sistema deve ser capaz de importar dados tanto do MS Office quanto do OpenOffice


* Confiabilidade
     - Em cada 1000 execucoes, nao mais do que 2 podem apresentar falhas de software.



* Robustez
     - Se acontecer uma falha antes do usuario salvar, o sistema deve recuperar uma versao nao salva com perda de conteudo menor que 1 minuto de trabalho


* Usabilidade
     - Um usuario treinado deve ser capaz de submeter um pedido de compra em menos que 5 minutos
     - Um usuario nao treinado deve ser capaz de submeter um pedido de compra em menos que 30 minutos

     
* Manutenibilidade
     - Todos os metodos devem ser documentados utilizando a notacao Javadoc
     - Todos os metodos devem ter ate 30 linhas de codigo

     
* Portabilidade
     - O sistema deve poder ser executado em sistema operacional windows e linux, nas arquiteturas i386, aix e sparc


* Reusabilidade
     - O controle de usuarios deve reutilizar componentes de autenticacao ja utilizados no sistema PORTMAP


* Testabilidade
     - A complexidade ciclomatica maxima de um modulo nao pode ser maior que 20



#### Elaboracao 


Tem como objetivo explicitar o conhecimento obtido na concepcao e elicitacao, alem disso, transformar narrativas de linguagem natural para uma forma estruturada (uml), o resultado esperado sao os caos de uso e classes conceituais.


#### Negociacao

Tem como objetivo priorizar e identificar os riscos dos requisitos, alem de eliminar, combinar e modificar os requisitos chegando em um consenso sobre a lista final de requisitos. 

Costuma ter conflitos entre os representantes do cliente com requisitos contraditorio e prioridades, alem desse, costuma ter conflito entre o cliente e a equipe Dev em relacao ao custo e ao prazo (old)



#### Especificacao

Tem como objetivo produzir a especificacao de requisitos (regras de negocio, requisitos funcionais e nao funcionais, podendo incluir casos de uso e classes conceituais)



#### Validacao

Tem como objetivo assegurar que a especificacao de requisitos esta precisa, costuma ter problemas de ambiguidade, incocistencia, imissao e erro.

Deve ser feito perguntas como

* Os requisitos estao claros?
* O requisito e testavel? Os testes foram especificados?


#### Gerenciamento

Tem objetivo de controlar as mudancas nos requisitos e permitir a analise de impacto das mudancas



### 10 principios de engenharia de requisitos

1. Escutar
2. Se preparar antes da reuniao
3. Importante ter um mediador
4. Comunicacao face a face e o ideal
5. Tome nota das decisoes
6. Estimular colaboracao
7. Manter o foco
8. Se algo estiver obscuro, desenhe!
9. Siga em frente!
10. Negociacao nao eh um jogo 