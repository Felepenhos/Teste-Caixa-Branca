# Teste-Caixa-Branca

A técnica de caixa-branca atenta mais ao funcionamento interno do sistema. Também conhecido como
teste estrutural ou teste de caixa de vidro tem como foco testes que são aplicados nas estruturas internas
dos sistemas. Ao contrário do que ocorre nos testes de caixa-preta, a aplicação dos testes de caixa-branca
fornece resultados que possibilitam uma análise diretamente relacionada ao código-fonte do sistema em

![Captura de tela 2023-10-09 215614](https://github.com/Felepenhos/Teste-Caixa-Branca/assets/116446769/bdebb4bc-8879-4980-bc58-6cb71e704c1f)

# 1.A DOCUMENTAÇÃO FOI DESCRITA NO CÓDIGO? 
A Documentação não esta descrita da maneira corretamente dentro do Código . 

# 2. AS VARIÁVEIS E CONSTANTES POSSUEM BOA NOMENCLATURA? 

O Codígo poderia estar melhor em suas nomenclaturas para facilitar a sua intrepetação , como melhorar o nome do pacote , das suas classes ,
seus metodos , variavéis , e alguns comentários . 

# 3 EXISTEM LEGIBILIDADE E ORGANIZAÇÃO NO CÓDIGO?

Sobre a sua Legebilidade o código está bem formatado e segue a maneira da  formatação Java , o que facilita bastante . Sobre a sua organaziação 
O código está bem organizado dentro do pacote login . 

# 4 TODOS OS NULLPOINTERS FORAM TRATADOS?

Sim todos os Nullpointers foram tratado dentro do codígo , porém podem fazer algumas melhorias para melhorar o tratamento de exceções.

# 5 A ARQUITETURA UTILIZADA FOI DEVIDAMENTE RESPEITADA?
Para aquilo que se pede a arquitetura foi devidamente respeitada . 

# 6 AS CONEXÕES UTILIZADAS FORAM FECHADAS?

Não tem tratamento explícito para fechar as conexões com o banco de dados. Isso pode resultar em vazamento de recursos e problemas de desempenho , é recomendando usar o  finally para garantir que as conexões sejam fechadas, independentemente de ocorrer uma exceção.

# 7 ERROS DO CÓDIGO 
1. Variavel ur1 não declarada
2. Concatenação de Strings.
3.  Injeção de SQL
4.  Nomes de Classes e Métodos:
5.  Falta de Fechamento de Conexão:

# GRAFO 

![1](https://github.com/Felepenhos/Teste-Caixa-Branca/assets/116446769/23438986-2565-42d1-b31c-47c52185b3e4)

# Calculo 
+ Nós = 14
+ Arestas =16
+ 16-14= 4 Caminhos Possivel 

# Caminhos 
+ 1 = 1;2;3;4;5;6;
+ 2 = 1;3;4;5;6;7;8;9;10;11;12;14;
+ 3 = 1;3;4;5;6;7;8;9;10;11;12;13;
+ 4 = 1;3;4;5;6;7;8;9;10;11;14;

# Tecnologia 
Linguagem de Programação Java 

# IDE 
APACHE NETBEANS IDE 17

# ULTIMA ATUALIZAÇÃO 09/10/2023









