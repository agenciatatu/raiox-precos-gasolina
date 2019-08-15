# Análise de dados para a matéria: https://www.agenciatatu.com.br/noticia/porto-de-pedras-tem-a-gasolina-mais-cara-de-alagoas/


O arquivo original enviado pela Sefaz/AL é o EconomizaAlagoas_PrecosCombustiveis_20dias.ods. Neste arquivo estão presentes todas as vendas de combustível, em todos os postos de Alagoas, no período entre 9 e 29 de Julho de 2019.

O primeiro passo foi filtrar os postos de modo a excluir da base tudo o que não fosse gasolina, isso originou o arquivo combustiveis-original.csv.

Ps. Inicialmente nossa intenção foi de selecionar os preços apenas da gasolina comum, no entanto percebemos que 27 postos comercializaram apenas gasolina aditivada no período, então entendemos ser mais justo fazer uma média de preços para todos os tipos de gasolina vendidos em cada posto.

Os dados originais não traziam os nomes dos postos ou o município onde eles se localizavam, então cruzamos os números de CNPJ com a base da Receita Federal, permitindo assim que fossem acessadas outras informações a respeito das empresas.

A partir daí foi possível verificar a média de preços em cada município e fazer um comparativo a partir da distância de cada município em relação a Maceió.

O código completo, em Python, está em um notebook, no arquivo "Dados Gasolina Municipio.ipynb".

O gráfico de dispersão foi feito com auxilio da ferramenta flourish.studio, já o mapa interativo foi possibilitado pela ferramenta mapbox.com. E o código também se encontra disponível neste Github.
