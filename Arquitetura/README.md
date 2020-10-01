# Arquitetura física

Nesse diagrama demonstramos como será a arquitetura física do nosso
sistema distribuído, e-commerce, desde a conexão do usuário até nossos sistemas
de banco de dados.

O Loadbalancer é responsável por fazer o balanceamento de conexões de
usuários simultâneos utilizando nosso sistema. Podendo impedir usuários de se
conectarem ao site ou de usar uma determinada função do sistema se o fluxo estiver
muito grande.

O usuário conecta no webserver, tendo acesso somente ao WebSite,
podendo utilizar de forma coerente todos suas funcionalidades. Essas
funcionalidades são os módulos que são independentes entre si, e executam
funções diferentes. Esses módulos que são os servidores de aplicação, estão
conectados ao banco de dados, que por sua vez possui um backup e está
armazenado na nuvem.

![arc fisica correcao](https://user-images.githubusercontent.com/71103252/94868467-9a0a6c80-0419-11eb-8b2b-cfd71c5125e6.png)

# Arquitetura lógica 

Neste diagrama está demonstrado a arquitetura lógica.

Separamos o sistema em camadas, primeiramente é a camada de interface
do usuário, o cliente terá apenas acesso a esta camada, onde ele poderá utilizar as
funções dos módulos do website, sem se preocupar com as complexidades por trás
do sistema.

A segunda camada é a de processamento de dados, onde definimos os
módulos que farão parte do nosso sistema. Cada um possui suas funções
independentes, porém são necessário para a funcionalidade do sistema como um
todo. Dentro dessa camada, além dos módulos desenvolvido por nós, também
teremos aplicações de terceiros para a funcionalidade do sistema.

Já a camada de armazenamento de dados, será onde todas as informações
dos usuários do sistema ficará armazenados, e também informações sobre os
produtos. Colocamos um banco de dados de backup para garantir a operabilidade
do sistema em caso de nosso banco principal falhar.

![arc logica](https://user-images.githubusercontent.com/71103252/94868746-287eee00-041a-11eb-8022-3f53e08f9abd.jpg)


