API 6º Semestre ADS
DomRock AI - Auxia
logo da Buzz Tech

Buzz Tech
| Desafio | Solução | Backlog do Produto | DoR | DoD | Cronograma de Sprints | Tecnologias | Manual de Instalação | Equipe |

Status do Projeto: Concluído ✅

Relatório de Testes: PDF 📊

Pasta de Documentação: Link 📄

Video do Projeto: Youtube 📽️

🏅 Desafio
O desafio consiste em criar uma aplicação web de avaliação de respostas de LLM. A aplicação deve permitir enviar um prompt para 2 (dois) LLMs via API simultaneamente. A seguir, a aplicação deve apresentar as 2 (duas) respostas obtidas. Para cada resposta, a aplicação apresenta os itens de avaliação das respostas e, ao final, a aplicação apresenta uma escala de comparação das duas respostas para que o usuário possa definir qual das duas respostas foi a melhor e justificar. Todas essas informações devem ser gravadas em um banco de dados que servirá para futuros retreinamentos dos LLMs.

🏅 Solução
O AUXIA - Auxiliary AI Training, permitirá que os usuários enviem prompts para múltiplos modelos de IA, comparem suas respostas, avaliem cada uma segundo critérios objetivos, escolham a melhor resposta e justifiquem suas decisões. Esse processo garantirá um aprendizado por reforço eficiente, possibilitando o aprimoramento contínuo dos modelos utilizados através dos dados persistidos de cada avaliação.

📋 Backlog do Produto
Rank	Prioridade	User Story	Story Points	Sprint	Requisito do Cliente	Status
1	Alta	Como usuário, quero uma interface para inserir um prompt, para que eu possa enviá-lo às LLMs e obter suas respostas	14	1	R02	✅
2	Alta	Como usuário, eu quero enviar um prompt para dois modelos de IA simultaneamente, para que eu possa avaliar suas respostas posteriormente.	47	1	R01/R09	✅
3	Alta	Como usuário, eu quero visualizar as respostas das LLMs de forma clara e acessível, para que eu possa analisá-las em critérios.	28	1	R03	✅
4	Alta	Como usuário, eu quero uma interface para poder avaliar cada resposta individualmente através de critérios definidos, para que eu possa analisar a qualidade das respostas geradas	22	1	R03	✅
5	Alta	Como usuário, eu quero uma interface para poder escolher a melhor resposta entre as duas geradas pelas LLMs, para que o sistema registre minha decisão e justificativa.	29	1	R04	✅
6	Alta	Como Administrador, eu quero que as avaliações dos usuários sobre as LLMs sejam armazenadas em um BD, para que possam ser utilizadas em processos de fine-tunning futuramente.	41	1	R05	✅
7	Alta	Como usuário, eu quero ser alertado caso minha escolha entre LLM1 e LLM2 não esteja coerente com minha avaliação, para que eu possa revisar minha decisão antes de finalizar.	3	2	R04	✅
8	Alta	Como usuário, eu quero que as respostas das LLMs sejam enriquecidas com informações relevantes da base de dados (vetorizada), para que sejam mais precisas	5	2	R07	✅
10	Alta	Como Administrador, eu gostaria de ser o primeiro usuário do sistema, já devidamente pré inserido no banco de dados, para que possa acessar a aplicação.	44	1	R06	✅
11	Média	Como Administrador, eu quero cadastrar novos usuários na plataforma, para que somente pessoas autorizadas possam acessá-la.	17	3	R06	✅
12	Média	Como usuário, eu quero acessar a aplicação através de uma interface de login, para que somente usuários autorizados possam utilizar o sistema.	13	3	R06	✅
13	Média	Como usuário autorizado, eu quero acessar o sistema através de um login, para utilizar a aplicação.	23	3	R06	✅
14	Média	Como usuário autenticado, eu quero poder fazer o logout da aplicação de forma segura, para que meus dados não fiquem acessíveis a terceiros.	18	3	R06	✅
15	Média	Como usuário, eu quero poder revisar minha escolha antes de submetê-la, para que eu tenha certeza de que minha decisão está correta.	2	2	R04	✅
16	Média	Como Administrador, eu quero visualizar a lista de usuários cadastrados, para que eu possa gerenciar quem tem acesso ao sistema.	20	3	R06	✅
17	Média	Como Administrador, eu quero redefinir a senha de um usuário, para que eu possa ajudá-lo caso ele não consiga acessar a conta.	18	3	R06	✅
18	Média	Como Administrador, eu quero excluir usuários do sistema, para que possa revogar o acesso de usuários a aplicação.	13	3	R06	✅
19	Baixa	Como usuário, eu quero ser informado com mensagens de erro caso ocorra demora excessiva no envio do prompt ou na resposta das LLMs, ou outros erros, para que eu possa entender o problema e tentar novamente.	2	2	R03	✅
21	Baixa	Como usuário, eu quero poder receber mensagens claras sobre o status das avaliações, para ter certeza de que minha avaliação foi registrada corretamente.	2	2	R03	✅
22	Baixa	Como usuário, eu quero poder voltar para telas anteriores durante o processo de avaliação, para que eu possa corrigir informações antes de enviar a decisão final.	1	2	R03/R04	✅
24	Baixa	Como usuário, eu quero editar meus dados pessoais, para que eu possa manter minhas informações atualizadas.	16	3	R06	✅
🏃‍ DoR - Definition of Ready
User Stories com Critérios de Aceitação
Subtarefas divididas a partir das US
Design no Figma
Modelagem do Banco de Dados
Diagrama de Rotas
Banco de Dados Vetorizado do Cliente
🏆 DoD - Definition of Done
Manual de Usuário
Manual da Aplicação
Documentação da API (Application Programming Interface)
Código completo
Vídeos de cada etapa de entrega
📅 Cronograma de Sprints
Sprint	Período	Documentação
🔖 SPRINT 1	10/03 - 30/03	Sprint 1 Docs
🔖 SPRINT 2	07/04 - 27/04	Sprint 2 Docs
🔖 SPRINT 3	05/05 - 25/05	Sprint 3 Docs
💻 Tecnologias
         
📖 Manual de Instalação
🛠 Pré-requisitos
Git (Download)

Python 3.9+ (Download)

Node.js 16+ (Download)

Poetry (opcional para o backend) (Download)

1. Clonar o Repositório Principal
git clone --recurse-submodules https://github.com/BuzzTech-API/API_ADS_6SEMESTE_2025.1.git
cd API_ADS_6SEMESTE_2025.1
Observação: Se já tiver clonado sem os submódulos, execute:

git submodule update --init --recursive
2. Configuração do Backend (auxia-backend)
1° Adicione as variáveis no .env

2° Inicialize o Banco de dados MongoDB no localhost:

3° Coloque a base de dados vetorizada ./client dentro da raíz do backen:

4° Instale e Inicie a aplicação:

Opção A: Com Poetry

cd ./auxia-backend
poetry shell
poetry install
make run
Opção B: Com Ambiente Virtual Python

cd ./auxia-backend
python3 -m venv venv
source venv/bin/activate # se você usa linux
venv/Scripts/activate 	 # se você usa windows
pip install -r requirements.txt
fastapi dev ./auxia/main.py
Saída Esperada:
Servidor rodando em http://localhost:8000 (acesse http://localhost:8000/docs para a UI do Swagger).

3. Configuração do Frontend (auxia-frontend)
cd ../auxia-frontend/auxia
npm install
npm run dev
Saída Esperada:
Frontend rodando em http://localhost:5173.

🎓 Equipe
Membro	Função	Github	Linkedin
Ivan Duarte	Product Owner		
Vitor Lima	Scrum Master		
Isaque da Silva	Desenvolvedor		
Joice Araujo	Desenvolvedor		
Jonas Alves	Desenvolvedor		
Pedro Davi	Desenvolvedor		
Rafael Motta	Desenvolvedor		
