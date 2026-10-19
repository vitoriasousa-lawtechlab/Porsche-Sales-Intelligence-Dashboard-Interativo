**Porsche Sales Intelligence — Dashboard Interativo**
Dashboard em HTML, CSS e JavaScript, desenvolvido para o desafio da DIO Criando Agentes de Tratamento de Dados. O projeto apresenta 100 registros de vendas de veículos Porsche em um painel responsivo e publicável no GitHub Pages.

**Acesse o dashboard**
https://github.com/vitoriasousa-lawtechlab/Porsche-Sales-Intelligence-Dashboard-Interativo/blob/main/index.html

**Perguntas de negócio**
- Onde estão concentradas as receitas? Gráfico das sete unidades federativas com maior receita, para identificar mercados prioritários.
- Quais modelos vendem mais? Gráfico dos sete modelos com mais transações, para analisar preferências de produto.
- Quais meios de pagamento movimentam mais receita? Gráfico por método de pagamento, para compreender o perfil comercial dos clientes.
**Análise complementar:** distribuição das situações de entrega, útil para acompanhar o fluxo operacional.
Indicadores e filtros
O painel exibe receita total, número de vendas, ticket médio e estados atendidos. Os filtros de modelo, estado, ano do veículo e método de pagamento recalculam todos os indicadores e gráficos imediatamente. O botão Limpar filtros retorna à visão geral.
**Preparação dos dados**
**Origem: **planilha sanitizada disponibilizada pela DIO. Foram selecionadas apenas colunas sanitizadas de data, modelo, ano, preço, quilometragem, pagamento, cidade, estado e situação de entrega, além do identificador da venda. Os campos de preço e ano foram convertidos para números; não existem fórmulas de Excel ou referências externas no painel. Foram mantidos 100 registros, com receita total de US$ 12,827,800.50 (soma do preço sanitizado).
Qualidade de dados: 24 datas aparecem como INVALID na fonte sanitizada. Essas datas foram convertidas para valor nulo, mas as transações continuam contabilizadas nos gráficos e KPIs, pois as perguntas de negócio não dependem da data. O filtro Ano do veículo utiliza o ano do modelo, não o ano da transação. Não foram incluídos dados pessoais de clientes ou vendedores no HTML.
Tecnologia e execução
- HTML5, CSS3 e JavaScript puro, sem dependências, bibliotecas ou chamadas de rede.
- index.html: arquivo único, inclui os dados sanitizados e toda a interface.
- base_tratada.csv: arquivo de auditoria do tratamento de dados utilizado.
- README.md: documentação do projeto.
Para reproduzir localmente, baixe o repositório e abra index.html diretamente no navegador. Para atualizar o painel, substitua o conjunto de dados incorporado à variável data no HTML pelos registros normalizados de uma nova base.
Prompt utilizado
Usando a base sanitizada de 100 vendas Porsche, construa um dashboard em arquivo único index.html com HTML, CSS e JavaScript. Não inclua dados pessoais. Apresente receita, número de vendas, ticket médio e estados atendidos. Responda três perguntas: quais estados geram mais receita, quais modelos têm mais vendas e quais meios de pagamento geram mais receita. Adicione uma análise de status de entrega e filtros por modelo, estado, ano do veículo e pagamento. Use um visual escuro, tipografia limpa e detalhes em dourado. Os gráficos e os KPIs devem reagir juntos aos filtros. Evite bibliotecas e dependências externas para funcionar no GitHub Pages.

Refinamentos incorporados à especificação final: inclusão de contagem de datas inválidas, manutenção desses registros nas análises não cronológicas, estados distintos e botão para redefinir os filtros. O projeto foi desenvolvido diretamente com o ChatGPT e geração de código HTML/JavaScript; não foi utilizado Canvas nem um agente separado com skill.
Publicação no GitHub Pages
1. Crie um repositório público, por exemplo porsche-sales-dashboard.
2. Envie index.html, base_tratada.csv e README.md para a raiz do repositório.
3. Vá a Settings → Pages → Build and deployment e selecione Deploy from a branch, branch main, pasta / (root).
4. Abra a URL fornecida pelo GitHub Pages e teste os filtros.
5. Substitua o link de exemplo acima pelo endereço publicado. Envie a URL do repositório como entrega na DIO.
Evidências sugeridas
Capture uma imagem da visão geral e outra com um filtro aplicado; adicione-as a images/ e referencie-as no README se desejar fortalecer o portfólio.
Nota: os valores de vendas não constituem projeções, e a base de dados é fornecida para fins de aprendizagem.
