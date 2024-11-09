🚀 Projeto WebSocket com Express, MySQL, GitHub Actions e Terraform
Este projeto implementa um servidor WebSocket com Express para comunicação em tempo real e armazena os dados em um banco MySQL. O deploy é feito em uma instância EC2 da AWS com automação de infraestrutura usando Terraform e GitHub Actions.

🛠 Tecnologias Utilizadas
Node.js
Express
WebSocket
MySQL
Terraform
GitHub Actions
AWS EC2
🚀 Como o Projeto Foi Desenvolvido
Servidor HTTP com Express
Utilizamos Express para criar um servidor HTTP que lida com as conexões WebSocket, facilitando a comunicação em tempo real entre clientes.

Comunicação WebSocket
Através de WebSocket, os clientes podem trocar mensagens em tempo real. Isso é ideal para aplicações como chats, notificações em tempo real e dashboards dinâmicos.

Integração com MySQL
O banco MySQL armazena dados persistentes. Toda comunicação importante é armazenada e pode ser recuperada, permitindo histórico e continuidade nas interações.

Automação com GitHub Actions e Terraform

GitHub Actions: Configurado para realizar o CI/CD. Ao enviar um novo commit para o repositório, uma ação automatizada é executada, preparando o projeto para o deploy.
Terraform: Responsável por criar e configurar a infraestrutura na AWS. O Terraform define a instância EC2, configura variáveis e provisiona recursos necessários para rodar o servidor WebSocket.
Deploy em EC2 da AWS
A infraestrutura é gerenciada pelo Terraform, que cria a instância EC2, configura a rede e as permissões de segurança, e instala as dependências do ambiente. O GitHub Actions executa o pipeline de deploy, enviando a aplicação para a instância EC2 após qualquer mudança relevante no código.

🔑 Principais Funcionalidades
Comunicação em Tempo Real com WebSocket
Transmissão de mensagens em tempo real entre os clientes conectados.

Banco de Dados Persistente
MySQL garante armazenamento de dados, como histórico de mensagens e informações do cliente.

Automação de Infraestrutura
O uso de Terraform e GitHub Actions facilita o deploy contínuo e o gerenciamento da infraestrutura em AWS.

Monitoramento de Conexões
O servidor gerencia automaticamente as conexões ativas, enviando atualizações apenas para os usuários conectados.