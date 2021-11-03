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
CASE,ACTIVITY,DATE,
hospital_a,apresentar influenciador,01/01/2021,
hospital_a,apresentar decisor,15/01/2021,
hospital_a,negociação de preço,30/01/2021,
hospital_a,contrato juridico,28/02/2021,
hospital_a,fechamento,30/03/2021,
hospital_a,apresentar influenciador,01/01/2021,
hospital_a,apresentar decisor,15/01/2021,
hospital_a,demonstração de valor,15/02/2021,
hospital_a,negociação de preço,28/02/2021,
hospital_a,contrato jurídico,28/04/2021,

<h3>Sistema</h3>
<p>O sistema conta com templates de carregamento e um padrão para casos genéricos. Cada template destina-se a diferenciar etapas do processo específico tomando como base um </p>
<p>Após o carregamento precisamos definir o mapeamento da tabela com um "de x para" entre as colunas e os campos da plataforma de modo que possam ser lidos corretamente.</p>
<p>Após o carregamento realizado podemos proceder à descoberta de processo, clicando sobre o proecsso criado e, em seguida em mapa de processo dentro da opção de Descoberta.</p>