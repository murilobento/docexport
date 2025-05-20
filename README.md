# NOVA SISTEMA DOCEXPORT

## Configurações iniciais
- Cadastro da empresa:
- Dados básicos: CNPJ, inscrição estadual, razão social, nome fantasia, endereço completo, e-mail, 2 contatos telefônicos, logotipo;
- Dados fiscais e contábeis, CNAE, NIRE, Regime, Incentivador Cultural sim ou não, Regime de apuração fiscal, órgão de registro, regime especial de tributação);
- PIS/COFINS, método apuração, código do método de apuração, CST saídas, CST entradas, alíquota PIS, alíquota COFINS; 
- Dados do contador (nome, CRC e CNPJ ou CPF);
- Dados bancários principais.


## Autenticação
- Autenticação completa com login, esqueceu sua senha (redefinir por e-mail);
- Perfil de acesso (usuário comum ou admin) para controlar quais rotas ou páginas cada nível pode acessar no sistema. 

## Tecnologias
- Preferência para desenvolver em PHP usando o framework Laravel;
- Use o Bootstrap como base para a estilização dos componentes. Que tenha layout amigável, responsivo, para acesso com celular também, com tema escuro e claro;
- Banco de dados a sua escolha, optando por otimização e segurança;
- Implementação de protocolos de segurança para o sistema.

## Módulo Estoque
- Cadastrar produtos (Unidade de medida, tipo de estoque, natureza, controla estoque?, estoque máximo e mínimo, estoque atual, precificação (preço de fornecedor, preço de custo, preço de reposição, custo médio, margem %, podendo alterar valores manualmente e/ou de acordo com valor de compra), dados fiscais (origem, NCM, CEST, Segmento CEST, e regras fiscais ICMS e PIS/COFINS que foram cadastrados no Comercial).
- Cadastrar classificação fiscal e NCM (buscar da internet de acordo com a numeração do produto);
- Controlar o estoque;
- Cadastrar local de estoque;
- Cadastrar tipo de estoque (ativo imobilizado, mercadoria para revenda, material para brinde, matéria prima, material de uso e consumo)
- Requisição de compra;
- Realizar compras de produtos/serviços importando o XML ou manualmente (que gere um contas a pagar no financeiro); 
- Controle de patrimônio da empresa por tipo (ativo imobilizado, veículo);
- Correção de estoque (acerto de estoque, contagem de estoque e inventário);
- Consulta de movimentação de estoque.
- Relatórios ().

## Módulo Comercial
- Cadastro de clientes e fornecedores;
- Cadastro operação fiscal (venda de mercadoria, devolução de mercadoria, remessa de bonificação doação ou brinde, devolução de compra, entrada de bonificação doação ou brinde, compra de material de uso e consumo, compra de ativo imobilizado, exportação de mercadorias recebidas com fim especial, venda de mercadoria adquirida ou recebida de terceiros, compra para comercialização de terceiros, devolução mercadoria exportação recebida com fim especial), devolução de venda de mercadoria adquirida ou recebida de terceiros, venda de bem ativo imobilizado);
- Cadastro de regras fiscais ICMS (tributado 18%, substituição tributária, isento, outros, não tributada, combustível, isento 41, diferimento);
- Cadastro de regras fiscais PIS e COFINS (tributado, isento, operação de aquisição com isenção, PIS/COFINS 49, operação sem incidência de contribuição);
- Gerar vendas (que gere contas a receber) e invoice (proforma);
- Gerar orçamentos (não interfere no contas a pagar, nem em estoque);
- Gerar nota fiscal a partir de uma venda, ou emitir manualmente (podendo também cancelar ou inutilizar a mesma);
- Relatórios ().

## Módulo Financeiro
- Cadastro de bancos e agências;
- Cadastro de centro de custo (pessoa física, pessoa jurídica);
- Cadastro de condição de pagamento (escolhe o forma: a prazo ou a vista e a quantidade parcelas, podendo ser entrada + quantidade de parcelas, ou apenas as quantidades de parcelas. O período das parcelas também pode ser escolhido pelo usuário);
- Cadastro de formas de pagamento (PIX, dinheiro, crédito, débito, cheque, boleto);
- Cadastro de plano de contas. (Estabelece uma estrutura hierárquica para classificar todas as contas contábeis da empresa divididos em: ativos, passivos, receitas, despesas e patrimônio líquido);
- Cadastro de funcionários (para controlar folha salarial);
- Controlar as despesas;
- Controlar os pagamentos aos fornecedores ();
- Contas a pagar e receber (o lançamento pode ser a partir de uma NF ou cupom já emitidos com importação por XML, ou manualmente);
- Baixar uma conta (a pagar, a receber ou pagamento a fornecedor) paga/quitada;
- Relatórios ().
