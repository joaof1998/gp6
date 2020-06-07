# Garrafeira do ribatejo
Projeto de Engenharia de Software

# Elementos do projeto:

## Declaração do problema
	A Garrafeira do ribatejo é uma empresa que se dedica ao comércio de vinhos e bebidas espirtuosas tendo um loja fisca onde tambem é o armazem das encomendas online.

	Com um atendimento personalizado e eficaz para clientes e para revendedores, tendo tambem um catalogo muito diversificado na sua área de négocio e uma rapida expedição de encomendase pretende desenvolver um sistema de informção que tem como objetivo fazer a gestaão de encomendas e servir de catalogo.


## Requisitos funcionais

- FR1: O cliente pode se dirigir a loja para adiquirir o produto e efetuar pagamento ao colaborador;
- FR2  O cliente ao entrar no website pode fazer o login ou registar-se para poder usufruir de todas as funcionalidades;
- FR3: O cliente pode realizar a encomenda online no site e pagar atrabés dos métodos de pagamento disponiveis; 
- FR4: Fica disponivel na área de cliente o produto encomendado e uma cópia da fatura original;
- FR5: A aplicação de gestão da Garrafeira do Ribatejo gere os stocks e da um alerta e procede fazendo a encomenda ao fornecedor quando atinge uma quantidade mínima de stock;


## Requisitos não funcionais 

- NFR1: O website deve ser intuitivo para utilizar e a interface deve ser simples de utilizar;
- NFR: Conformidade com orientações -  O design  da aplicação deve estar otimizado para os mais variados dispositivos;
- NFR: Operações - o website tem de comunicar com base de dados;
- NFR: Plataforma - A aplicação tem que ser desenvolvida em HTML;
- NFR: Autenticação - os clientes são obrigados a fazer o login para facilidade de acesso e tambem para confirmar a sua identidade; 
- NFR: Operações - o website tem de comunicar com base de dados;
- NFR: Segurança - os clientes tem restrições de acesso aos dados que comprometam as infomações sobre os outros utilizadores;

7
## restrições de acordo com o projeto

- Disponiblidade: Vai estar disponivel através de qualquer browser nos seguintes equipamentos
		- Computador;
		- Tablet;
		- Smartphone;
- Acessibilidade: O site só pode ser consultado na Península Ibérica;
- Requesitos Legais: o website tem de cumprir com todas as normas e leis aplicadas no pais de consulta;

## Atividades a desenvolver

### Identificar atores

**Colaborador Loja**: Funcionário da Garrafeira do Ribatejo responsável pelo atendimento ao publico.

**Colaborador Logística**: Funcionário da Garrafeira do Ribatejo responsável pelo tratamento, processamento e envio de encomendas.

**Cliente**: Pessoa que encomenda produtos.

**Cibernauta**: Todo aquele que, através da Internet, consulta as páginas da Garrafeira do Ribatejo.

**Administrador de Sistemas**: Responsável por toda a gestão do sistema informático.

- Cenário 1: O cliente dirige-se as instalações da garrafeira do Ribatejo e faz a encomenda. O colaborador regista e realiza o pedido do cliente;
- Cenário 2: O cliente acede ao website, faz login e realiza o pedido. No cesto de compras o cliente confirma os seus dados e executa o pagamento para confirmar a encomenda;

### Identificar casos de uso

*Caso de Uso: **Efetuar pré-registo***: 
 
 1. O cibernauta utiliza o sistema de informação da página da Internet da Garrafeira do Ribatejo para efetuar o pré-registo, e solicita a sua validação.
 2. O cibernauta tem que indicar o nome de utilizador, password, nome, morada, telefone e numero de contribuinte.


*Caso de Uso: **Consultar Produtos***:
   
1. O cibernauta, o cliente e o colaborador loja utilizam o sistema de informação para consultar os produtos.
2. O catálogo é apresentado com a seguinte forma: referência, seguida da categoria, do produto e do preço.  


*Caso de Uso: **Atualizar Dados Cliente***:

1. O cliente utiliza o sistema de informação da página da Internet da Garrafeira do Ribatejo para alterar os seus dados.
2. **_Includes_** _Fazer Autenticação_.


*Caso de Uso: **Consultar Encomendas***:

1. O cliente utiliza o sistema de informação da Garrafeira do Ribatejo para consultar o estado da encomenda.
2. **_Includes_** _Fazer Autenticação_.


*Caso de Uso: **Efetuar Encomendas Internet***: 

1. O cliente utiliza o sistema de informação da página da Internet da Garrafeira do Ribatejo para efetuar uma encomenda.
2. **_Includes_** _Fazer Autenticação_.
3. O cliente escolhe os produtos que pretende.
4. Para cada produto escolhido o sistema verifica o seu custo e adiciona-o ao total da encomenda.
5. O pedido é registado no sistema de informação.
6. O colaborador logística recebe o pedido através do sistema de informação processa a encomenda.


*Caso de Uso: **Validar Registo***:

1. O administrador de sistema verifica através do sistema de informação o pré-registo do cibernauta
2. Envia um email com o link de validação da conta.


*Caso de Uso: **Efetuar Encomendas***:

1. O cliente dirige-se ao balcão da loja Garrafeira do Ribatejo para efetuar uma encomenda.
2. O colaborador loja regista e encomenda do cliente no sistema de informação.
3. O cliente escolhe os produtos que deseja.


*Caso de Uso: **Expedição de Encomendas***:

1. O funcionário logística recebe o pedido de encomenda através do sistema de informação.
2. Caso o produto esteja em stock, o funcionário logística processa a encomenda.
3. Caso haja rutura de stock o funcionário logística informa o administrador de sistemas.
4. Por fim, o funcionário logística expede a encomenda.


*Caso de Uso: **Receber Pagamento***:

1. O colaborador loja quando completa a encomenda, recebe o pagamento da mesma.
2. Quando o cliente finaliza a encomenda utilizando o sistema de informação da página da Internet da Garrafeira do Ribatejo, é gerado referencias para pagamento.
3. O cliente faz o pagamento através de uma das modalidades disponíveis: à cobrança, referências multibanco, transferência bancária ou paypal.
4. **_Includes_** _Emitir Fatura_

### Diagramas de Casos de Uso
Diagrama de caso de uso Sistema da Garrafeira do Ribatejo.
![Digrama de Casos de Uso](GP6_projetoES\1.ElementosProjeto\images\casosdeuso.png"Diagrama_Casos_de_Uso")

### Diagrama de Classes
![Diagrama Classes](GP6_projetoES\1.ElementosProjeto\images\diagramadeclasses.jpg"Diagrama_classes")

#### Descrição das Classes

**Cliente**:

Representa um cliente da Garrafeira do Ribatejo que fez o Pré-Registo através da Internet para poder efetuar encomendas através do site. O cliente é caracterizado por único código, nome, morada e numero de contribuinte. Possui um username e um password únicas para efetuar encomenda através da Internet.

**Loja**:

Representa uma loja Garrafeira do Ribatejo. A loja é caracterizada por único código, nome e localização e é constituída por uma área de atendimento ao publico assim como um armazém.

**Funcionário**:

Representa os funcionários que trabalham na Garrafeira do Ribatejo. Estes são caracterizados por numero de identificação, nome e categoria profissional.

**Encomenda**:

Representa uma encomenda efetuada pela Internet na Garrafeira do Ribatejo. A encomenda é caracterizada por um numero de encomenda e pelo estado em que se encontra (recebida, expedida ou entregue). A cada encomenda corresponde pelo menos uma fatura.

**detalheEncomenda**:

Representa o código de um produto de uma determinada encomenda. Cada detalheEncomenda é caracterizado por uma quantidade e preço unitário.

**Preço**:

Representa a tabela de preços que um determinado Produto pode assumir. O Preço é caracterizado por tipo, normal ou promoção e valor.

**Fatura**:

Representa uma fatura referente a uma determinada encomenda. É caracterizada por um numero de fatura, data e total.

**itemFatura**:

Representa a referência a um produto de uma determinada fatura, que por sua vez corresponde a um item de uma determinada encomenda.

**Produto**:

Representa a classe de produtos disponíveis ao clientes na Garrafeira do Ribatejo . Um produto é caracterizado por uma referencia, categoria e descrição.



## Desenvolver o protótipo com baixa fidelidade relativo a um requisito funcional;


