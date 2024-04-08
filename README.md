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

<h2>Conhecendo a base de dados</h2>
&nbsp;

-- visualizando alguns dados das tabelas - 1 --</br>
SELECT * FROM categorias;

<img class="aligncenter size-full wp-image-22850" src="https://www.makerzine.com.br/wp-content/uploads/2024/04/query1.png" alt="" width="400" height="258" />

&nbsp;

-- visualizando alguns dados das tabelas - 2 --</br>
SELECT * FROM produtos;

<img class="aligncenter size-full wp-image-22851" src="https://www.makerzine.com.br/wp-content/uploads/2024/04/query2.png" alt="" width="995" height="471" />

&nbsp;

-- contando o total de produtos --</br>
SELECT COUNT(*) AS Total_de_produtos FROM produtos;

<img class="aligncenter size-full wp-image-22852" src="https://www.makerzine.com.br/wp-content/uploads/2024/04/query3.png" alt="" width="195" height="87" />

&nbsp;

-- contando o total de vendas --</br>
SELECT COUNT(*) AS Total_de_Vendas FROM vendas;

<img class="aligncenter size-full wp-image-22853" src="https://www.makerzine.com.br/wp-content/uploads/2024/04/query4.png" alt="" width="184" height="94" />

&nbsp;

-- contando os registros de todas as tabelas --</br>

SELECT COUNT(*) AS Qtd, 'Categorias' AS Tabela FROM categorias</br>
UNION ALL</br>
SELECT COUNT(*) AS Qtd, 'Clientes' AS Tabela FROM clientes</br>
UNION ALL</br>
SELECT COUNT(*) AS Qtd, 'Fornecedores' AS Tabela FROM fornecedores</br>
UNION ALL</br>
SELECT COUNT(*) AS Qtd, 'ItensVenda' AS Tabela FROM itens_venda</br>
UNION ALL</br>
SELECT COUNT(*) AS Qtd, 'Marcas' AS Tabela FROM marcas</br>
UNION ALL</br>
SELECT COUNT(*) AS Qtd, 'Produtos' AS Tabela FROM produtos</br>
UNION ALL</br>
SELECT COUNT(*) AS Qtd, 'Vendas' AS Tabela FROM vendas;</br>

&nbsp;

<img class="aligncenter size-full wp-image-22855" src="https://www.makerzine.com.br/wp-content/uploads/2024/04/query5.png" alt="" width="487" height="325" />

&nbsp;
