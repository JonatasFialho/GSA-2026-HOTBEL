em Tabela Analítica - Desempenho de Cidades, coloque um botao de ver detalhes, e quero que abra o modal e monstre todas as cidades Ranqueada e com venda dos 3 departamentos e status de ✅ se tiver venda dos departamentos e ⚠️ caso algum deles esteja zerado e valor em vermelho. 

e quero que a listagem dos nomes das cidades seja verificada todos as base de venda pra trazer o nome, e quero que no filtro quando selecionar algum mes, permaneça os nomes das cidades geral, e so o resultado da venda altere para o mes do filtro, para que caso alguma cidade nao tenha venda naquele mes ela apareça na hora do filtro constrando tudo zerado nela, O UNICO FILTRO QUE QUERO QUE ELE RESPEITE É O DO SUPERVISOR, VENDEDOR

ELE TEM QUE FAZER A MESMA LOGICA, ENCONTRAR NO GERAL E TRAZER QUANDO FILTRAR ELE.





Faça as seguintes implementações SEM ALTERAR NADA no restante do código existente:

1. Botão de Detalhes

Na seção "Tabela Analítica - Desempenho de Cidades":



Adicionar um botão chamado "Ver Detalhes"

Ao clicar, deve abrir um modal

2. Conteúdo do Modal

Dentro do modal, exibir:



Lista de todas as cidades ranqueadas

Para cada cidade, mostrar:

Nome da cidade

os departamentos e

Status visual:

✅ → se tiver venda de todos os departamentos

⚠️ → se algum dos departamentos estiver zerado

❌ → Se tiver tudo zerado

os Valores zerados devem aparecer em vermelho

3. Regra da Base de Cidades (CRÍTICO)

A construção da lista de cidades deve seguir exatamente esta lógica:



A lista de cidades NUNCA deve ser baseada em filtro de mês

A lista deve sempre considerar a base completa de dados

Comportamento correto:

Sem filtro → trazer todas as cidades da base

Com filtro de Supervisor → trazer todas as cidades que esse Supervisor atende (considerando toda a base, sem filtro de mês)

Com filtro de Vendedor → trazer todas as cidades que esse Vendedor atende (considerando toda a base, sem filtro de mês)

4. Comportamento dos Filtros

🔹 Filtro de SUPERVISOR:

Define quais cidades aparecem na lista

Deve buscar cidades na base completa (sem filtro de mês)

Mesmo que não tenha venda no período filtrado, a cidade deve aparecer com valor zerado

🔹 Filtro de VENDEDOR:

Mesma lógica do Supervisor:

Define as cidades da lista

Busca sempre na base completa (sem considerar mês)

Não pode remover cidades da lista por falta de venda no período

🔹 Filtro de MÊS:

Não altera a lista de cidades

Deve impactar somente os valores de venda

Se não houver venda no mês:

A cidade deve permanecer na lista

Com valores zerados

5. Regra de Exibição (OBRIGATÓRIO)

A lista de cidades nunca pode desaparecer ou reduzir por causa do filtro de mês

Toda cidade válida no contexto (Supervisor/Vendedor ou geral) deve sempre aparecer

Valores devem ser ajustados conforme os filtros aplicados

🧠 Regra Geral Consolidada

Lista de cidades = Base completa + (Supervisor ou Vendedor, se aplicado)

Valores = Baseados no filtro de mês

⚠️ RESTRIÇÃO FINAL

Não modificar nenhuma outra parte do código

Apenas adicionar essas funcionalidades solicitadas

Se quiser, posso agora transformar isso direto em código (Power BI / DAX ou front-end do seu projeto), já com a lógica pronta pra funcionar.
