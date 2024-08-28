# 📅 Project Ignite Call
Schedule Call é um aplicativo de agendamento de reuniões que se integra com o Google Calendar, permitindo que os usuários agendem reuniões apenas nos horários disponíveis definidos pelo administrador.

# 🚀 Tecnologias Utilizadas
Next.js: Framework React para desenvolvimento web.
Docker: Usado para criar uma instância local do banco de dados.
Google Calendar API: Integração para sincronização de eventos.
# 🛠️ Pré-requisitos
Antes de começar, você vai precisar ter instalado em sua máquina as seguintes ferramentas:

Git
Node.js
Docker
Docker Compose
Além disso, é recomendável usar um bom editor para trabalhar com o código, como o VSCode.

📦 Clonando o Repositório
bash
Copiar código
# Clone este repositório
git clone https://github.com/seuusuario/schedule-call.git

# Acesse a pasta do projeto
cd schedule-call
🐳 Configuração do Docker
Crie uma imagem Docker para o banco de dados local:

Certifique-se de que você tenha o Docker instalado e em execução. No diretório raiz do projeto, você encontrará um arquivo docker-compose.yml (caso contrário, crie um conforme necessário).

Execute o Docker Compose para subir o banco de dados:

bash
Copiar código
docker-compose up -d
Este comando irá construir e iniciar os contêineres definidos no arquivo docker-compose.yml.

# 🔧 Instalação das Dependências
bash
Copiar código
# Instale as dependências
npm install
# 🔑 Configuração das Variáveis de Ambiente
Antes de iniciar o projeto, você precisará configurar suas variáveis de ambiente. Crie um arquivo .env.local na raiz do projeto e adicione suas credenciais da Google API e outras configurações necessárias:

plaintext
Copiar código
GOOGLE_CLIENT_ID=seu_google_client_id
GOOGLE_CLIENT_SECRET=seu_google_client_secret
NEXT_PUBLIC_API_URL=http://localhost:3000
DATABASE_URL=postgres://user:password@localhost:5432/database_name
Certifique-se de substituir os valores de exemplo pelas suas próprias credenciais e configurações.

▶️ Rodando a Aplicação
bash
Copiar código
# Inicie o servidor de desenvolvimento
npm run dev
A aplicação estará disponível em http://localhost:3000.

# 🧪 Rodando os Testes
Caso tenha testes configurados, você pode rodá-los com:

bash
Copiar código
# Execute os testes
npm run test
📝 Licença
Este projeto está sob a licença MIT. Para mais detalhes, veja o arquivo LICENSE.
