# Fake Shop


## Variável de Ambiente
DB_HOST	=> Host do banco de dados PostgreSQL.

DB_USER => Nome do usuário do banco de dados PostgreSQL.

DB_PASSWORD	=> Senha do usuário do banco de dados PostgreSQL.

DB_NAME	=>	Nome do banco de dados PostgreSQL.

DB_PORT	=>	Porta de conexão com o banco de dados PostgreSQL.


** DEFINIÇÕES IMPORTANTES: ** 

O que é um Proxy?

Um proxy é como um intermediário entre você (ou sua aplicação) e outros servidores. Ele funciona assim:
Quando você faz uma solicitação para acessar algo na internet (como um site), o proxy recebe essa solicitação.
O proxy, então, encaminha o pedido ao servidor correto.
Quando o servidor responde, o proxy entrega a resposta de volta para você.

O que é um Load Balancer?

Um load balancer (ou balanceador de carga) é como um gerente que distribui tarefas para várias pessoas em uma equipe para garantir que ninguém fique sobrecarregado.
No contexto de sistemas:
Ele distribui as solicitações dos usuários entre vários servidores.
Isso garante que o sistema continue rápido e disponível, mesmo que muitos usuários o acessem ao mesmo tempo.



** Comandos importantes **

// Install
choco install kubernetes-cli
choco install k3d

// Create
k3d cluster create 
k3d cluster create meucluster --servers 3 --agents 3

// Listar
kubectl get nodes
k3d cluster list

// Delete
k3d cluster delete meucluster



** Componentes **

Pod - menor objeto 

replicaset - controlador do pod

deployment - gerenciamento de replicaset

service - expor os pods




kubectl get deployment

kubectl get pod -o wide

