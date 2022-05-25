# Desafio Back-end

## Se liga aqui

- Crie um repositório no seu GitHub **sem citar nada relacionado a Paggue**.
- Faça seus commits no seu repositório.
- Envie o link do seu repositório para o email **dev@paggue.io**.
- Dê uma olhada nos [links](#links).
- Fique à vontade para perguntar qualquer dúvida no email **dev@paggue.io**.

### Como é que eu envio o email?

#### **Desafio Back-end**

> Seu Nome
>
>Whatsapp
>
>Link do repositório

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
- Cuidado com a segurança
- Testes unitários e testes integração

## Como eu vou me destacar?

- Uso do Docker
- Uso de Design Patterns
- Documentação
- Proposta de melhoria na arquitetura
- **PHP/Laravel**
- Conhecimento da AWS (S3, EC2, ELB, Lambda...)

## E Qual é o meu desafio?

Em nossa rotina vemos muitas empresas realizando suas vendas em máquinas de cartão ou de maneira online e nesse processo
temos sistemas que gerenciam essas vendas, recebimentos, saldos e pagamentos.

Em nosso sistema temos empresas e usuários que administram essas empresas.

- Para a empresas é preciso do seguinte, CNPJ, Razão social, Nome fantasia, telefone e email, cada empresa deve ser
  única (CNPJ)

- Para os administradores, precisamos do Nome Completo, CPF, e-mail e Senha. CPF/CNPJ e e-mails devem ser únicos no
  sistema. Sendo assim, seu sistema deve permitir apenas um cadastro com o mesmo CPF ou endereço de e-mail.

- Apenas administradores podem solicitar saques(pagamento) para uma determinada empresa.

- Valide se a empresa tem saldo antes de criar um pagamento.

- O saque só pode ser realizado para uma conta verificada.

- Após o Pagamento criado o mesmo deve ser processado em uma sub-rotina [Job](https://laravel.com/docs/9.x/queues)

- O pagamento deve ser uma transação (ou seja, revertido em qualquer caso de inconsistência) e o dinheiro deve voltar
  para o saldo da empresa.

- Após o pagamento processado deve ser enviado ao administrador uma notificação (email, sms) enviada por um serviço de
  terceiro.

    - Os serviços de terceiros podem está eventualmente indisponível


> Importante ressaltar que esse teste é qualitativo e não quantitativo, vamos levar em consideração a qualidade do código e não o número de etapas concluídas.

> Não iremos avaliar
> - Frontend (só avaliaremos a (API Restful)
> - Processo de Autenticação
> - Cadastro de administrador e empresa

## Links
- [Paggue](https://paggue.io/)
- [API Restful](https://www.devmedia.com.br/rest-tutorial/28912)
- [Laravel](https://laravel.com/)


Boa sorte!