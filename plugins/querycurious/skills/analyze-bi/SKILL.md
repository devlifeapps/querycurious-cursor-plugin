---
name: analyze-bi
description: Answer business questions about the user's company using QueryCurious. Use when the user asks about sales, orders, customers, products, stores, or BI metrics from the Lifeapps data warehouse.
---

# Analyze BI with QueryCurious

## When to use

- The user asks for numbers, rankings, or lists from their company's BI data.
- The user mentions vendas, pedidos, clientes, produtos, lojas, or faturamento.

## Instructions

1. Read `querycurious://docs/entities` before choosing an entity set.
2. Read `querycurious://docs/entity/{name}` before selecting or filtering fields.
3. Use only attribute names listed in that schema. Do not invent attributes.
4. When `functional_description` is null, do not invent a meaning for the field.
5. Call `list_entity_sets`, `describe_entity_set`, `query_entity_set`, `aggregate_entity_set`, or `sample_entity_set`.
6. Treat every result as already limited to the company of the signed-in user.
7. If the tool returns `Missing tenant context` or `Ambiguous tenant context`, stop and tell the user to ask a Lifeapps administrator to link their SSO user to a single company.
