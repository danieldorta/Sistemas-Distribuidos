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
