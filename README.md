# Desafio Back-end

## Se liga aqui

- Crie um repositório no seu GitHub **sem citar nada relacionado a Paggue**.
- Faça seus commits no seu repositório.
- Envie o link do seu repositório para o email **dev@paggue.io**.
- Dê uma olhada nos [links](#links).
- Fique à vontade para perguntar qualquer dúvida no email **dev@paggue.io**.

### Como é que eu envio o desafio por email?

#### **Desafio Back-end**

Envie um email com as seguintes informações:

- Seu Nome
- Whatsapp
- Link do repositório
- Link da API

### Tenho que utilizar framework?

Sim, mas fique à vontade para escolher o framework.

- Lembre-se, decida por aquele com o qual estará mais seguro em apresentar e conversar com a gente na entrevista.
- O [Laravel](https://laravel.com/) será um grande diferencial, então **sugerimos** que utilize.

## O que fazer para mandar bem?

- Código limpo e organizado (nomenclatura, etc)
- Conhecimento de padrões (PSRs, design patterns, SOLID)
- Apresentar soluções que domina e saber argumentar suas escolhas
- Tratamento de erros
- Modelagem de Dados
- Arquitetura (pensar antes de escrever)
- Cuidado com a segurança!!!

## O que não pode faltar?

- Uso do Docker
- Postgres ou MySQL
- Testes unitários e testes de integração com coverage de 80% da pasta app
- Collection completa do Postman com exemplos salvos

## Como eu vou me destacar?

- Ambiente em produção, aplicação em nuvem. Dê preferência aos serviços da AWS
- Uso de Design Patterns
- Documentação
- Proposta de melhoria na arquitetura
- **PHP/Laravel**
- Conhecimento da AWS (S3, EC2, ELB, Lambda...)
- Ambiente de desenvolvimento com xdebug no Docker

## E qual é o meu desafio?

Atualmente o mercado de eventos vem crescendo muito, e um sistema de gestão para o mesmo é de grande valia, podendo ter chance de se destacar no mercado.
Com isso o sistema deve possuir:

- Signup
  - Telefone, cpf/cnpj, senha, nome
- Autenticação e permissão, os usuários devem poder se autenticar e acessar apenas recursos específicos
  que serão determinados pelo perfil de acesso. [Permissions](#links)

- Tipos de perfis de acesso: admin, produtor de eventos e cliente

- CRUDs: produtor, evento, setores, lote, ingressos e cupom de desconto:
  - **Produtor:** agência responsável por realizar os eventos. Esse deve possuir acesso ao sistema para gerenciar os eventos
  - O evento deve conter um banner, esse arquivo deve ser salvo em nuvem quando a aplicação estiver em produção (recomendamos o uso da AWS S3) 

- Venda de ingressos online, integrando com o pix web da Paggue para realizar o pagamento

- Após o Pagamento criado o mesmo deve ser processado em uma sub-rotina [Job](https://laravel.com/docs/12.x/queues)

- Após o pagamento processado deve ser enviado ao administrador e ao cliente uma notificação (email, sms) por um serviço
  de terceiros.

- Integração com a Paggue
    - Sua aplicação deve utilizar a API da Paggue para gerar o PIX para seu cliente realizar o pagamento do
      Produto/ingresso
    - Sua aplicação deve estar pronta para receber notificações (webhooks) referente ao pagamento realizado por seu
      cliente e finalizar o pedido.

- Os serviços de terceiros podem estar eventualmente indisponíveis

### Bonus:

- Aparecer somente um lote por setor, enquanto houver ingresso disponível para ele, caso ocorra seu esgotamento ou passar
  a data de seu encerramento,
  o próximo lote deve ficar disponível, caso exista
- Deve ser enviado um email também ao administrador após a criação de um evento por qualquer produtor

**Todas etapas da implementação devem conter testes automatizados**

#### Para realizar a integração com a Paggue você deve possuir um cadastro.

- Acesse [paggue.io](https://register.paggue.io) e faça seu cadastro
- Acesse o menu **configurações->integrações** e gere suas credenciais.
- Documentação da API [go.paggue.io/developers](https://go.paggue.io/developers)
- Para o recebimento dos webhooks no seu software fique atento para realizar a verificação da assinatura enviada no
  header.

### Deixe no seu Readme instruções de como rodar seu projeto, e como utilizar sua aplicação.

## Atenção

> Importante ressaltar que esse teste é qualitativo e não quantitativo, vamos levar em consideração a qualidade do
> código e não o número de etapas concluídas;

> Porém o número de etapas entregues com qualidade vai ser um ponto avaliativo para a senioridade

> Não iremos avaliar:
> - Frontend (só avaliaremos a API Restful)

## Links

- [Paggue](https://paggue.io/)
- [API Restful](https://www.devmedia.com.br/rest-tutorial/28912)
- [Laravel](https://laravel.com/)
- [Laravel Permission](https://spatie.be/docs/laravel-permission/v5/introduction)
- [Bref](https://bref.sh/)

Boa sorte!

### 🔹 Requisitos Essenciais:
> - ✅ Experiência com Laravel (APIs RESTful e aplicações web).
> - ✅ Conhecimento em bancos de dados relacionais (MySQL, PostgreSQL, SQL Server).
> - ✅ Experiência com Eloquent ORM e otimização de queries.
> - ✅ Testes automatizados com PHPUnit/Pest.
> - ✅ Autenticação e segurança com Laravel Sanctum, Passport, JWT.
> - ✅ Conhecimento de arquitetura MVC, SOLID e boas práticas.
> - ✅ Versionamento com Git/GitHub (Git Flow).
> - ✅ Trabalhar com filas e jobs assíncronos (Redis, Laravel Queues).
> - ✅ Experiência na construção de APIs (documentação, versionamento, rate limiting).

### 🚀 Diferenciais:
> - 🔹 Experiência com Laravel Octane para alta performance.
> - 🔹 Conhecimento em microserviços e arquitetura distribuída.
> - 🔹 Experiência com Docker e containers.
> - 🔹 Conhecimento em CI/CD para automação de deploys.
> - 🔹 Aplicação de design patterns (Repositório, Service Layer, Factory).
> - 🔹 Mensageria com Kafka, SQS para comunicação assíncrona.
> - 🔹 Conhecimento em DevOps (AWS, Kubernetes, Terraform).

