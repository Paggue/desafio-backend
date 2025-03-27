# Desafio Back-end

## Se liga aqui

- Crie um repositório no seu GitHub **sem citar nada relacionado a Paggue**.
- Faça seus commits no seu repositório.
- Envie o link do seu repositório para o email **dev@paggue.io**.
- Dê uma olhada nos [links](#links).
- Fique à vontade para perguntar qualquer dúvida no email **dev@paggue.io**.

### Como é que eu envio o desafio por email?

#### **Desafio Back-end**

> Seu Nome
>
>Whatsapp
>
>Link do repositório
>
>Link da API

### Tenho que utilizar framework?

Sim, mas fique avontade para escolher o framework.

- Lembre-se, decida por aquele com o qual estará mais seguro em apresentar e conversar com a gente na entrevista
- O [Laravel](https://laravel.com/) será um grande diferencial, então **sugerimos** que utilize.

## O que fazer para mandar bem?

- Código limpo e organizado (nomenclatura, etc)
- Conhecimento de padrões (PSRs, design patterns, SOLID)
- Apresentar soluções que domina e saber argumentar suas escolhas
- Tratamento de erros
- Modelagem de Dados
- Arquitetura (pensar antes de escrever)
- Cuidado com a segurança!!!

## Oq não pode faltar?

- Uso do Docker
- Postgres ou Mysql
- Testes unitários e testes de integração com covarege de 80% da pasta app
- Collection completa do postman com exemplos salvos

## Como eu vou me destacar?

- Ambiente em produção, aplicação em nuvem. Dê preferência os serviços da AWS
- Uso de Design Patterns
- Documentação
- Proposta de melhoria na arquitetura
- **PHP/Laravel**
- Conhecimento da AWS (S3, EC2, ELB, Lambda...)
- Ambiente de desenvolvimento com xdebug no docker

## E qual é o meu desafio?

Atualmente o mercado de eventos vem crescendo muito, e um sistema de gestão para o mesmo é de grande valia, podendo ter chance de se destacar no mercado.
Com isso o sistema deve possuir:

- Signup
  - Telefone, cpf/cnpj, senha, nome
- Autenticação e permissão, os usuários devem poder se autenticar e acessar apenas recursos especificos
  que seram determinados pelo perfil de acesso. [Permissions](#links)

- Tipos de perfis de acesso: admin, produtor de eventos e cliente

- CRUDs: produtor, evento, setores, lote, ingressos e cupom de desconto:
  - **Produtor:** agencia responsável por realizar os eventos. Esse deve possuir acesso ao sistema para gerenciar os eventos
  - O evento deve conter um banner, esse aquivo deve ser salvo em nuvem quando a aplicação estiver em produção (recomendamos o uso da AWS S3) 

- Venda de ingressos online, integrando com o pix web da Paggue para realizar o pagamento

- Após o Pagamento criado o mesmo deve ser processado em uma sub-rotina [Job](https://laravel.com/docs/12.x/queues)

- Após o pagamento processado deve ser enviado ao administrador e ao cliente uma notificação (email, sms) por um serviço
  de terceiros.

- Integração com a Paggue
    - Sua aplicação deve utilizar a Api da paggue para gerar o PIX para seu cliente realizar o pagamento do
      Produto/ingresso
    - Sua aplicação deve estar pronta para receber notificações(webhooks) referente ao pagamento realizado por seu
      cliente e finaliazar o pedido.

- Os serviços de terceiros podem está eventualmente indisponível

#### **Bonus:**

- Aparecer somente um lote por setor, enquanto houver ingresso disponível para ele, caso ocorra seu esgotamento ou passar
  a data de seu encerramento,
  o proximo lote deve ficar disponivel, caso exista
- Deve ser enviado um email também ao administrador após a criação de um evento por qualquer produtor

#### **Todas etapas da implementação deve conter testes automátizados**

#### Para realizar a integração com a Paggue você deve possuir um cadastro.

- Acesse [paggue.io](https://register.paggue.io) e faça seu cadastro
- Acesse o menu **configurações->integraçoes** e gere suas credenciais.
- Documentação da Api [go.paggue.io/developers](https://go.paggue.io/developers)
- Para o recebimento dos webhooks no seu software fique atento para ralizar a verificação da assinatura envida no
  header.

### Deixe no seu Readme intruções de como rodar seu projeto, e como utilizar sua aplicação.

## Atenção

> Importante ressaltar que esse teste é qualitativo e não quantitativo, vamos levar em consideração a qualidade do
> código e não o número de etapas concluídas;

> Porem número de etapas entregues com qualidade vai ser um ponto avaliativo para a senioridade

> Não iremos avaliar
> - Frontend (só avaliaremos a API Restful)

## Links

- [Paggue](https://paggue.io/)
- [API Restful](https://www.devmedia.com.br/rest-tutorial/28912)
- [Laravel](https://laravel.com/)
- [Laravel Permission](https://spatie.be/docs/laravel-permission/v5/introduction)
- [Bref](https://bref.sh/)

Boa sorte!