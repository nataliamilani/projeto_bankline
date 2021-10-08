# Projeto final referente a matéria de Microservices & Serverless Architecture
## Curso: MBA em Full Stack Developer

**Aplicação:** projeto_bankline

**Visão geral:**
Este repositório, é considerado o projeto final a ser executado, para validações dos microserviços em funcionamento.
Nele contem todas as aplicações configuradas no arquivo de docker composer que encontra-se na pasta raíz.
Fizemos o compilado das aplicações neste repositório para facilitar a subida das aplicações, caso tenha necessidade de executar na máquina local, assim todas as imagens serão baixadas diretamente do Docker Hub.

**Requisitos minimos de instalação:**
- Docker desktop

**Tecnologias utilizadas:**
- Docker
- Spring Boot
- Java 11
- Maven
- Junit
- Swagger

**Monitoração:**
- Prometheus

**Segurança:**
- API Gateway

**Disponibilidade:**
- Eureka

**Postman - link para import na plataforma - URL localhost:**
- https://www.getpostman.com/collections/f8eea8546a1af821ef31

**OBS:** As aplicações que encontram-se compiladas neste projeto, são as mesmas dos repositórios abaixo:
- eureka (https://github.com/nataliamilani/eureka) já estar online para receber os registros;
- api-gateway (https://github.com/nataliamilani/api-gateway);
- prometheus (https://github.com/nataliamilani/prometheus);
- debito (https://github.com/nataliamilani/credito);
- credito (https://github.com/nataliamilani/credito);
- conta-corrente (https://github.com/nataliamilani/conta-corrente);
- investimento (https://github.com/nataliamilani/investimento);
- fatura (https://github.com/nataliamilani/fatura);

Para subir os containers deste projeto, basta utilizar o comando "docker-compose up", no diretório raiz da aplicação via terminal, após clonar o repositório na máquina local.

**Os serviços também estão disponivéis em um servidor GCP (Google Cloud Platform):** 
- Para visualizar a disponibilidade das aplicações, favor acessar: http://35.199.91.25:8761/
- Para visualizar o monitoramento das aplicações favor acessar: http://35.199.91.25:9090/targets 
- Para acessar os endpoints das aplicações através do servidor segue um exemplo:
	http://35.199.91.25:9000/debito/debito/listar/contas
	http://35.199.91.25:9000/{nome_container_app}/{rota_controller}
OBS: no servidor para acessar os endpoints das aplicações, apenas a porta 9000 (porta api-gateway) estará disponível

**Postman - Os arquivos de collection e environment das aplicações com as URL da Google Cloud, encontra-se no link abaixo:**
https://github.com/nataliamilani/collection_projeto-bankline
