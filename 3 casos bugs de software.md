# Três casos de Bugs em Software que causaram grandes prejuízos
## - 1. Bug do Foguete Ariane 5 (1996)
Em 1996, a Agência Espacial Europeia lançou o foguete Ariane 5, que explodiu só 37 segundos depois do lançamento. O motivo foi um erro de software: um valor de velocidade foi convertido de um tipo de dado de 64 bits para 16 bits, e foi o que causou um estouro de número. Esse erro não foi detectado nos testes porque o software tinha sido reutilizado do Ariane 4, que tinha características diferentes. O prejuízo estimado foi de cerca de 370 milhões de dólares.

## - 2. Bug do Therac-25 (Anos 1980)
O Therac-25 era uma máquina de radioterapia usada em hospitais nos anos 1980. Mas devido a falhas no software de controle, a máquina administrou doses letais de radiação em vários pacientes do hospital, e issso resultou em pelo menos seis mortes. O problema estava relacionado a condições de corrida (race conditions) no código, que não foram previstas pelos desenvolvedores. Esse caso destacou a importância de testes rigorosos em sistemas críticos à vida.

## - 3. Bug do Mars Climate Orbiter (1999)
Em 1999, a NASA perdeu a sonda Mars Climate Orbiter por causa de um erro de conversão de unidades. Enquanto uma parte do sistema usava unidades imperiais (libras-força), outra parte usava o sistema métrico (newtons). Essa falha de comunicação causou a entradw incorreta da sonda na atmosfera de Marte, causando a sua destruição. O prejuízo foi de aproximadamente 125 milhões de dólares. Esse caso marcou a importância da padronização e validação de dados em sistemas mais complexos.
