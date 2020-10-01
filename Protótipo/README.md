# Protótipo

## Tema: 

Criação de um serviço de E-Commerce (Loja de Óculos Masculino via Browser).

## Tecnologias: 

Java, MySQL, Cloud, HTML, Internet.

## Diagrama

Diagrama mostrando como será feito o acesso no nosso sistema, onde o
usuário será responsável por fazer seu cadastro e logar no site. Ele também poderá
navegar pela página para selecionar os seus produtos e adicioná-los ao carrinho. Ao
fazer checkout ele será redirecionado para o sistema de pagamentos, que de inicio
iremos utilizar a ferramenta do PayPal. O administrador será responsável por
controle do sistema, fazendo alterações em preços de produtos, ou retirar e
adicionar produtos em caso de falha de sistema, podendo também fazer alterações
no estoque que sejam justificadas.


![image](https://user-images.githubusercontent.com/71103252/94869058-d68a9800-041a-11eb-8633-3f30b98b490e.png)

## Descrição das funções:

Temos como objetivo criar um sistema distribuído de um E-commerce, mais
especificamente uma loja de óculos masculino.

Em nosso sistema utilizaremos um site feito em HTML. Na aba de seleção de
produtos, o usuário pode adicionar seus produtos no carrinho e também “logar” ou ir
direto para o carrinho para realizar o seu check out. No carrinho, o usuário vai poder
ver seu valor total da compra, as quantidades de seus produtos, realizar alterações e
prosseguir para o pagamento, onde será preciso realizar login, informar seus dados
de pagamento e endereço.

Iremos criar uma aplicação em Java para fazer a comunicação entre o cliente
e os serviços de pagamentos. Java também será usado para criarmos nossas
aplicações para comunicação entre servidores, banco de dados, nuvem e usuários.

Os dados cadastrais fornecidos pelos clientes serão armazenados em um
banco de dados MySql, que terá seu próprio servidor na nuvem, de forma
transparente, para garantir a segurança dos dados e garantir a disponibilidade.

Em outro banco de dados, será feito o armazenamento dos produtos, para
controle de estoque, também armazenados na nuvem.

Todos nossos serviços e servidores estarão se comunicando pela Internet,
através dos seus protocolos mais utilizados.

Pretendemos utilizar servidores independentes para cada aplicação, para nos
garantir certa segurança as falhas que podem ser causadas, porém se tivermos um
bom servidor na nuvem que nos garanta escalabilidade, e seja funcional, esse não
será um grande problema.

