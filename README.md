# Atendimento Inteligente – Delivery

## Sobre o projeto

O **Atendimento Inteligente – Delivery** é um projeto desenvolvido no n8n que simula um sistema de atendimento ao cliente de um aplicativo de delivery.

O objetivo é utilizar Inteligência Artificial para interpretar mensagens dos clientes, identificar o tipo de solicitação e encaminhá-la para a equipe responsável, contribuindo para um atendimento mais organizado e eficiente.

Este projeto foi desenvolvido como iniciativa de aprendizado e prática em automação de processos e Inteligência Artificial.

## Funcionalidades

- Recebimento de mensagens por Webhook e Chat Trigger.
- Classificação automática das solicitações utilizando IA.
- Identificação da categoria e prioridade do atendimento.
- Encaminhamento para a equipe responsável.
- Registro dos atendimentos em uma Data Table.
- Envio de notificações por e-mail para a equipe.

## Categorias de atendimento

| Categoria | Equipe responsável | Prioridade |
|---|---|---|
| Atraso | Logística | Média |
| Pagamento | Financeiro | Alta |
| Pedido não recebido | Resolução de pedidos | Alta |
| Outros | Atendimento geral | Baixa |

Os atendimentos são registrados com status inicial **aberto**.

## Tecnologias utilizadas

- **n8n:** automação e integração dos processos.
- **Claude Haiku 5.5:** interpretação e classificação das mensagens.
- **Data Tables:** armazenamento dos registros de atendimento.
- **Gmail:** envio de notificações por e-mail.

## Como funciona o fluxo

1. O sistema recebe a mensagem enviada pelo cliente.
2. A Inteligência Artificial interpreta o conteúdo e identifica a categoria da solicitação.
3. O fluxo define a prioridade e a equipe responsável.
4. O atendimento é registrado na tabela de tickets.
5. Uma notificação por e-mail é enviada para a equipe.

## Testes realizados

Foram realizados testes com diferentes situações de atendimento:

- Atraso na entrega.
- Problemas relacionados a pagamento.
- Pedido não recebido.
- Outras solicitações e sugestões.

Os testes foram realizados no ambiente n8n utilizado durante o desenvolvimento.

## Como importar o projeto

1. Baixe o arquivo `Atendimento_Inteligente_Delivery_GitHub_FINAL.json`.
2. Acesse sua conta n8n.
3. Importe o arquivo JSON como um workflow.
4. Crie ou selecione uma Data Table chamada `tickets_atendimento`.
5. Confira o mapeamento dos campos da tabela.
6. Configure suas próprias credenciais do Claude e do Gmail.
7. Substitua o endereço de e-mail indicado pelo seu próprio endereço.
8. Configure a autenticação do Webhook.
9. Realize os testes antes de utilizar o fluxo.

**Importante:** algumas configurações e credenciais precisam ser definidas na conta de quem importar o projeto.

## Segurança

O arquivo disponibilizado não deve conter credenciais, chaves de API, dados pessoais de clientes ou informações privadas de contas.

Utilize suas próprias credenciais e dados fictícios durante os testes.

## Aprendizados

Durante o desenvolvimento, foram praticados conceitos de:

- Automação de processos com n8n.
- Integração de modelos de Inteligência Artificial.
- Classificação de mensagens em linguagem natural.
- Organização e encaminhamento de solicitações.
- Armazenamento de dados.
- Testes e validação de fluxos automatizados.

---

**Projeto desenvolvido para fins de aprendizado e construção de portfólio.**
