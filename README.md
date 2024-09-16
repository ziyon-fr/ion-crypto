ZIYON Token Smart Contract
Este repositório contém o contrato inteligente para o token ZIYON (símbolo: ION), implementado no padrão BEP-20. O contrato é escrito em Solidity e utiliza bibliotecas e práticas recomendadas, como SafeMath, para garantir operações seguras e evitar transbordamento de valores. Ele foi projetado para ser flexível e seguro, com funcionalidades que incluem controle de transações e gestão de permissões.

Características principais
Padrão BEP-20: O token segue as especificações do BEP-20, proporcionando compatibilidade com a Binance Smart Chain e outras plataformas que utilizam esse padrão.
Total Supply: O fornecimento total de tokens é fixado em 100 milhões, com 8 casas decimais.
Controle de Permissões: Funções de controle como onlyOwner permitem que apenas o proprietário do contrato execute operações críticas, como transferir a propriedade ou ajustar limites de transação.
Máxima Quantidade de Transação: O contrato impõe um limite de transação para evitar manipulações de mercado, definido em 100.000 tokens por transação.
Segurança: O contrato utiliza a biblioteca SafeMath para todas as operações aritméticas, garantindo a proteção contra overflow e underflow.
Eventos de Transferência e Aprovação: Suporte completo a eventos BEP-20, incluindo Transfer e Approval.
Funcionalidades Implementadas
totalSupply: Retorna a quantidade total de tokens em circulação.
decimals: Retorna o número de casas decimais usadas pelo token.
symbol: Retorna o símbolo do token.
name: Retorna o nome do token.
getOwner: Retorna o endereço do proprietário do token.
balanceOf: Retorna o saldo de tokens de um determinado endereço.
transfer: Transfere tokens de um endereço para outro.
approve e allowance: Gerencia as permissões de um terceiro para gastar tokens em nome de outro endereço.
transferFrom: Permite transferências de tokens usando a permissão de terceiros.
Configurações de Deploy
O contrato já vem configurado com as seguintes propriedades predefinidas:

Nome do token: ZIYON
Símbolo do token: ION
Casas decimais: 8
Suprimento total: 100.000.000 ION
Quantidade máxima por transação: 100.000 ION
Como Usar
Clone o repositório e implante o contrato usando qualquer ferramenta de desenvolvimento Solidity como Remix, Truffle ou Hardhat.
