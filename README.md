<h1>Análise de dados com SQL</h1>
<h2>Metadados das tabelas utilizadas</h2>
<strong>Tabela de vendas</strong>
<ul>
 	<li><strong>id_venda:</strong> Chave primária</li>
 	<li><strong>data_venda:</strong> Data da venda</li>
 	<li><strong>total_venda:</strong> Valor total da venda</li>
 	<li><strong>cliente_id:</strong> Chave estrangeira relacionando ao cliente</li>
</ul>
<strong>Tabela de produtos</strong>
<ul>
 	<li><strong>id_produto:</strong> Chave primária</li>
 	<li><strong>nome_produto:</strong> Nome do produto</li>
 	<li><strong>preco:</strong> Preço do produto</li>
 	<li><strong>categoria_id:</strong> Chave estrangeira relacionando a categoria</li>
 	<li><strong>marca_id:</strong> Chave estrangeira relacionando a marca</li>
 	<li><strong>fornecedor_id:</strong> Chave estrangeira relacionando ao fornecedor</li>
 	<li><strong>data_estoque:</strong> Data da última compra de estoque</li>
 	<li><strong>status:</strong> Status do pedido (Vendido, fora de linha, etc.)</li>
</ul>
<strong>Tabela de clientes</strong>
<ul>
 	<li><strong>id_cliente:</strong> Chave primária</li>
 	<li><strong>nome_cliente:</strong> Nome completo do cliente</li>
 	<li><strong>idade:</strong> Idade do cliente</li>
 	<li><strong>endereco:</strong> Endereço do cliente</li>
</ul>
<strong>Tabela de categorias</strong>
<ul>
 	<li><strong>id_categoria:</strong> Chave primária</li>
 	<li><strong>nome_categoria:</strong> Nome da categoria</li>
</ul>
<strong>Tabela de fornecedores</strong>
<ul>
 	<li><strong>id_fornecedor:</strong> Chave primária</li>
 	<li><strong>nome:</strong> Nome do fornecedor</li>
 	<li><strong>contato:</strong> Contato do fornecedor</li>
</ul>
<strong>Tabela de marcas</strong>
<ul>
 	<li><strong>id_marca:</strong> Chave primária</li>
 	<li><strong>nome:</strong> Nome da marca</li>
</ul>
<strong>Tabela de itens_venda</strong>
<ul>
 	<li><strong>venda_id:</strong> Chave estrangeira relacionando a venda</li>
 	<li><strong>produto_id:</strong> Chave estrangeira relacionado ao produto</li>
</ul>
&nbsp;
