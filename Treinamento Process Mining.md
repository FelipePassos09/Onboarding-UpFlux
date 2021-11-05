Treinamento Process Mining

<h1>Aula 1 - Processos, Importância e Process Mining</h1>
	<p>Os processos precisam ser fluidos, desse modo temos maior agilidade em sua execução e maior eficácia.</p>

<h2>Processos Falham</h2>
	<ul>
	<li>Processos falham e isso é normal, na área da saúde isso é uma coisa inaceitável pois gera insatisfação imediata, riscos e prejuísos para o cliente.</li>
	<li>Mapeamento de Fluxo de Valor - problemas
		<ul>
		<li>Subjetividade</li>
		<li>Geralmente Mapeia-se apenas o caminho feliz</li>
		<li>Nem todas as pessoas realmente conhecem o processo</li>
		<li>Nem todos querem que os problemas apareçam</li>
		<li>Tempo elevado na observação do processo</li>
		</ul>
		</li>
<h2>o que é Mineração de Processos</h2>
<p> Na literatura é a ideia de descobrir, monitorar e melhorar processos exrtraindo conhecimento a partir de logs de eventos(dados de processos) disponíveis nos sistemas de informações</p>
<p>O process mining uniu-se com a ciencia de dados para agregar suas práticas à descoberta e monitoação de processos, desse modo podemos aplicar IA, machine-learning, analise preditiva e outras tecnologias inerentes à ciencia de dados aos estudos e algoritmos utilizados pelo process mining</p>

<h2>Definição do Log de Eventos</h2>
<p>O log de eventos reune todos os dados necessários para a analise dos processos a serem analisados, nesse quesito precisamos de alguns dados essenciais, que são:CASE_ID,ACTIVITY e TIMESTAMP. Outros dados podem ser agregados a estes para um maior enriquecimento da analise, porém os três citados anteriormente são essenciais ao processo.</p>
<p>Com os dados já estruturados iniciamos o processo de analise, porém outra necessidade é que precisam ser levados em consideração um grande volume de transações, é recomendado um mínimo de 1000 casos para uma maior profundidade de analise e correta obtenção dos indicadores relacionados.</p>

<h2>Criando um Log de eventos</h2>
<h3>Criando o log de eventos</h3>
<p>CSV FILE<br />
<table style="border:1px">
<tr>
<td>CASE</td><td>ACTIVITY</td><td>DATE</td>
</tr>
<tr>
<td>hospital_a</td><td>apresentar influenciador</td><td>01/01/2021</td>
</tr>
<tr>
<td>hospital_a</td><td>apresentar decisor</td><td>15/01/2021</td>
</tr>
<tr>
<td>hospital_a</td><td>negociação de preço</td><td>30/01/2021</td>
</tr>
<tr>
<td>hospital_a</td><td>contrato juridico</td><td>28/02/2021</td>
</tr>
<tr>
<td>hospital_a</td><td>fechamento</td><td>30/03/2021</td>
</tr>
<tr>
<td>hospital_b</td><td>apresentar influenciador</td><td>01/01/2021</td>
</tr>
<tr>
<td>hospital_b</td><td>apresentar decisor</td><td>15/01/2021</td>
</tr>
<tr>
<td>hospital_b</td><td>demonstração de valor</td><td>15/02/2021</td>
</tr>
<tr>
<td>hospital_b</td><td>negociação de preço</td><td>28/02/2021</td>
</tr>
<tr>
<td>hospital_b</td><td>contrato jurídico</td><td>28/04/2021</td>
</tr>
</table>
<h3>Sistema</h3>
<p>O sistema conta com templates de carregamento e um padrão para casos genéricos. Cada template destina-se a diferenciar etapas do processo específico tomando como base um </p>
<p>Após o carregamento precisamos definir o mapeamento da tabela com um "de x para" entre as colunas e os campos da plataforma de modo que possam ser lidos corretamente.</p>
<p>Após o carregamento ser realizado podemos proceder à descoberta de processos, clicando sobre o processo criado e, em seguida, em mapa de processo dentro da opção de Descoberta.</p>
<p>Dentro da descoberta temos várias possibilidades de analise de casos com aplicação de filtros, views alterantivas, mudança de paradigmas de analise e descoberta aprofundada.</p>

<h1>Aula 2</h1>
<h2>Processos Ineficientes Geram Experiencias Ruins</h2>
<p>Um processo ineficiente tende a gerar problemas e afetar a satisfação dos clientes devido á suas consequencias, como demora, retrabalho, falta de organização, descumprimento de prazos, produtos / serviços de má qaulidade, entre outros<br /> Tal problema afeta negativamente a empresa pois gera prejuízos, gastos desnecessários e perda de clientes e reputação.</p>
<p>Avaliemos o caso de uma pizzaria:<br />Um grupo de amigos resolve fazer um pedido online, porém após uma hora ainda noa foi feita a entrega do pedido. Ao entrarem em contato com a pizzaria são informados que repitam o pedido novamente pois o primeiro foi perdido de alguma maneira. Aborrecidos eles refazem o pedido e aguradam a entrega para poderem comer. Quando finalmente é feita a entrega, a pizza já está fria. Espantados com o mau serviço eles fazem uma avaliação negativa da pizzaria e uma crítica em seu site para alertar outros possíveis clientes.</p>
<p>A pizzaria em questão foi inaugurada há cerca de uma no e o neg[ocio costuma ir bem com os clientes elogiando a qualidade e sabor das pizzas. entretanto houve um aumento nas avaliações negativas de clientes e também uma diminuição dos lucros, com prejuízos em algumas entregas. Ao perguntar aos clientes regulares, o dono da pizzaria é informado que em alguns dias a pizza chega perfeitamente, porém em outros demora muito a entrega.</p>
<li style="font-size: 14px; padding: 25px; list-style: none">Nesses casos uma pesquisa de NPS pode ser útil para entender parte das dores e descobrir possiveis problemas no negócio.</li>
<h3>Processo da Pizzaria - Order-to-Cash</h3>
<p>O processo Order to Cash (O2C) é aplicável quando há o recebimento e processamento de pedidos de clientes.</p>
<img src="src\media\business-solutions-order-to-cash-lifecycle.png">

<h2>Pegadas Digitais</h2>
<p>Toda interação, seja ela digitalizado ou não, deixa marcas, no cenário da pizzaria essas pegadas estão nos sistemas de busca, pedidos, gerenciamento e entregas. Nesse caso podem ser transforados em Logs de Eventos.<br />Além dos logs contidos nos sistemas de pedidos e entregas, internamente há o registro das atividades realizadas, as pessoas quem realizaram as atividades e os horários onde as mesmas foram recebidas e entregues, nesse caso realizado de modo manual em uma planilha. <br />Além desses dados há a notação de dados de satisfação dos clientes, gastos, lucros e toda a sorte de dados adicionais relevantes ao negócio. Todo esse conjunto de dados pode ser tido como um facilitador da analise de processos pois nos permite visualizar de modo geral toda a jornada do processo, desde o inicio até sua conclusão e os desdobramentos de cada atividade em virtude de suas caracterísiticas e demais dados inerentes.</p>
<p style="display:flex; position: relative;">
<img src="src\media\fluxo pizzaria..png" style="display:flex; position: relative">
<a style="text-decoration:none; color: black;">Ao realizarmos o carergamento desses logs para a plataforma podemos observar todos os cenários pelos quais o processo seguiu, suas variantes e desdobramentos. Através do processo de descoberta podeos, inclusive, observar que o comportamento mais comum da plataforma é a solicitação via telefone, seguida do pedido no balcão e, por fim, via website. Vemos também que dependendo de cada origem há um comportamento distinto para o inicio da preparacão e consequente sequencia onde, em um dado momento podemos observar um loop-back no processo por telefone com um retorno de chamada. <br />Também vemos que, em todos os casos analisados, após o ínicio do preparo da pizza eles seguiram o mesmo fluxo (salvo onde houve desistência).<br />NEsse caso todos seguiram para o processo de assar e assim pro diante. Mas podemos notar que durante os processos algumas unidades se perderam, chegando ao final do processo um número inferior de pedidos. <br /><br />Isso se dá pois limitamos nossa visualização a um cenário ideal, ao abrirmos o range de conexões observamos uma pulverização caótica de rotinas, com caminhos confusos, salto de etapas, loops e diversos outros comportamentos estranhos ao proecsso conforme definido.</a></p>
<p>Devido a essas possibilidades a ferramneta de descoberta pode agregar tanta qualidade e otimização aos processos, através dela conseguimos identificar as variações e falhas no decorrer do processo.<br />Dentro da ferramenta temos várias possibilidades de análise, são elas:
	<h3>Atividades</h3>
	<p>São as várias atividades listadas do processo, por ela estabelecemos nosso range de observação do fluxo.</p>
	<h3>Conexões</h3>
	<p>São o número de variações do processo conforme identificado dentro dos dados carregados, nela definimos qual a profundidade que iremos observar o processo e qual o nível de precisão será exibido, desse modo podemos observar mais ou menos variações.</p>
	<h3>Perspectiva</h3>
	<p>é a maneira como iremos observar o processo, quais valores iremos apresentar como filtro principais e qual a relação que iremos abordar, se tempo, frequencia, custo, etc.</p>
	<p>Temos em perspectiva duas opções:
		<ul>
			<li>Primária:
				<ul>
					<li>É definida por qual fator iremos observar das atividades e qual a sua recorrência em virtude da opção selecionada.</li>
				</ul>
			</li>
			<br />
			<li>Secundária:
				<ul>
					<li>É fator que podemos agregar às variantes e rotinas identificadas, como a relação entre tempo e frequencia, ocorrência e frequencias, entre outros.</li>
				</ul>
			</li>
		</ul>
	</p>
</p>
<h3>Filtros</h3>
<h4>Atributos</h4>
<p>Temos, também, a possibilidade de desmembrar as nossas analises através ad ferramenta de filtros, obtendo assim novos valores e medições.<br /> <br /> Basta clicarmos no ícone de filtro e selecionar o atributo que iremos levar em consideração para recolhermos nossa métrica, lá podemos selecionar qualquer um dos campos carregados em nosso log de eventos. Desse modo teremos uma segmentação da nossa análise apenas para a condição especificada, desse modo facilitando o entendimento dos dados apresentados e do fluxo como seguiu. Além disso, em casos onde diagnosticamos uma pulverização muito grande de comportamentos, é bastante eficaz para o tratamento individual de cada atributo e seu entendimento mais simplificado.</p>
<h4>Tempo</h4>
<p>No modo tempo podemos segmentar nossos dados em virtude do timestamp do case, assim podemos observar períodos específicos de comportamentos, e ter indicadores levando em consideração sazonalidade, periodicidade e situações adversas temporarias.</p>
<h4>Extremidade</h4>
<p>:/</p>
<h4>Relações</h4>
<p>Como o nome indica, esse filtro permite segmentar as atividades pelas suas relações, criando visualizações de fugas ou aderencia ao processo.</p>
<h4>Ponto de Interesse</h4>
<p>Esse filtro permite segmentar nossa visualização por um dado específico dentro de um range de tempo, desse modo podemos visualizar a tendencia e relacionamentos desse ponto dentro da faixa definida e obter insights direcionados.</p>
<h4>Performance</h4>
<p>Aqui podemos definir a segmentação por resultados gerados, ou seja, a performance do processo. Nesse caso filtramos o conteúdo estabelecendo nossos interesses mínimos e máximos para visualizar os resultados dentro dessa faixa, seja para vermos tudo que atendeu às expectatiavs como para observar melhor aqueles que consideramos tendo fugido dos objetivos esperados.</p>

<h3>Funções dos Filtros</h3>
<p>Através dos filtros podemos gerar visualizações mais assertivas e "limpas" dos processos analisados, de modo que conseguimos estabelecer um melhor entendimento do processo analisado e criar conceitos mais eficazes para sua adequação.<br/>Em conjunto a isso temos a possibilidade de combinar os filtros em busca de detalhes antes perdidos entre o log de eventos como, quanto de prejuízo tivemos em decorrência da fuga de alguma etapa do processo ou como uma etapa do processo pode ser removida para agregar maior eficiência e assertividade na execução do fluxo. Isso tudo requer um estudo aprofundado que é favorecido com o uso de segmentações melhor aplicadas.</p>

<h1>Aula 3</h1>
<h2>Extraindo valor dos dados</h2>
<p></p>