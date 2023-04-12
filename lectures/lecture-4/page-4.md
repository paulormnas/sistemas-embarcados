---
layout: default
transition: slide-up
---

# Teste de Integração

<div>

Neste teste nós verificamos o comportamento do software quando conectado com o outros serviços, como WEB APIs, bancos de dados e outros dispositivos (no caso de software que envolvem conexões Bluetooth, NFC e etc).  

Aqui é importante definirmos Ambientes diferentes para rodar os testes:

- **Dev**: Ambiente local de desenvolvimento do software (desktop, notebook, smartphone, simuladores e todos os dispositivos necessários para o desenvolvimento do software). Aqui devemos rodar os testes de unidade e testes e2e que não necessitam de interação pelo usuário, ou que a interação possa ser simulada;
- **Staging**: Ambiente para testes que funciona de maneira muito semelhante ao ambiente de produção. Aqui serão realizados testes de integração, porém o banco de dados e os endereços de APIs deverão ser bancos e endereços de teste.
- **Prod**: Ambiente de produção é aquele em que o usuário vai atuar e inserir dados no sistemas. Nesse ambiente não devemos realizar testes e devemos usar os bancos de dados e endereços de APIs definitivos.

</div>