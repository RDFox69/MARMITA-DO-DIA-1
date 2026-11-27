
Abra `http://127.0.0.1:5000`. Para desenvolver a interface com atualização automática, deixe o Flask em execução e, em outro terminal, rode `npm run dev`; o Vite encaminha as chamadas `/api` ao servidor Python. A base SQLite fica em `instance/marmita.sqlite3` e persiste entre reinícios do servidor.


- **Visão geral:** pedidos do dia por etapa, faturamento, pagamentos concluídos e valores pendentes.
- **Novo pedido:** nome e telefone, pratos e quantidades, personalizações, adicionais, observações, retirada ou entrega, endereço, meio e situação do pagamento. O total muda conforme as escolhas.
- **Fila da cozinha:** cinco etapas com cartões que destacam cliente, itens, personalizações, endereço, entrega e pagamento. Um botão avança o pedido; a equipe vê os pedidos ativos, todos ou somente os de hoje.
- **Contas e permissões:** clientes criam conta, enviam pedidos e acompanham status e previsão. A equipe vê todos os pedidos; seu acesso precisa de aprovação administrativa.
- **Clientes:** lista e busca por contatos já registrados; ao iniciar um novo pedido, recupera telefone e endereço.
- **Fechamento de caixa:** faturamento separado do que foi recebido, totais pagos por Pix, dinheiro ou cartão, pendências e contagem de pedidos.
- **Persistência no servidor:** clientes, pedidos, pagamentos e status ficam no SQLite do servidor e são compartilhados entre dispositivos; a interface atualiza a fila automaticamente a cada 15 segundos.

BACKLOG

- [Product Backlog e critérios de aceitação](docs/product-backlog.md)
- [Sprint 1 — Pedidos e cozinha](docs/sprint-1.md)
- [Sprint 2 — Entregas e financeiro](docs/sprint-2.md)
- [Quadro Kanban atual, limites de WIP e diagrama](docs/kanban.md)

Feito e Modificado por Kauê Motta 
Alterações feitas com IA
