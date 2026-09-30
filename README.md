# Q1

Mesmo usando um hash determinístico, os valores dos ecentos são sorteados aleatoriamente, portanto, a distribuição altera a cada execução. 

O código busca procar o que foi dito na ADR #0002 sobre a arquitetura baseada em células.

Assim, o codigo busca simular um ambiente de distribuição de clientes onde cada celula possui seu armazenamento local, onde processos pendentes

Entretanto, o programa realmente não possui uma saída deterministica, baseado num sistema real.

# Q2

O Roteador, durante a escolha de Células, utiliza um único critério, sendo este o de 'camada fina', onde o Roteador utiliza como critério apenas a chave de partição. 
Quando a célula está fora, esses clientes têm seus processos executados em armazenamento local e, com o retorno da rede, os dados são sincronizados.

# Q3

As UBS, como afirmado no diagrama ```c4-conteineres.png```, têm a mesma lógica das UPAs, no bloco ```Célula Local da UBS/UPA```. Esse tratamento proporciona a funcionalidade correta em ambas as instituições.

# Q4

A estrutura geral do sistema é definida pela ADR #002, já que esta aborda a Arquitetura Baseada em Células, vidando evitar que, em casos onde ocorra queda de conexão externa, o sistema não fique completamente indisponível. 


# Q5

O envelope fornecido determina um orçamento robusto. Com essa informação, é seguro afirmar que Blue Green cabe no orçamento do nosso grupo.
