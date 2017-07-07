# Trabalho_sd
Trabalho de Sistemas Distribuidos, Ulbra - Canoas - 2017/01 - Prof. Tales


O trabalho foi desenvolvido utilizando node.js e base de dados MySQL (com phpmyadmin) e WAMP;

 - Rode o WAMP;



1º) Para criar o banco de dados, abra o phpMyAdmin e importe o arquivo 'trabalho_sd_estrutura.sql';


2º) Pelo phpMyAdmin, importar os arquivos e 'airports.csv' e 'carriers.csv' nas respectivas tabelas 'carriers' e 'airports';


3º) Coloque o arquivo referente ao ano que irá trabalhar na mesma pasta que o arquivo 'script_leitura_arquivo.php' e no terminal, rode o comando 'php script_leitura_arquivo.php';


4º) Abra o MySQL pelo terminal e rode a instrução a baixo, cuidando para refereciar exatamente o local onde se encontra o arquivo 'editado.csv'

SQL> LOAD DATA INFILE 'editado.csv' replace INTO TABLE ontime FIELDS TERMINATED BY ';' LINES TERMINATED BY '\n';



5º) Abra o arquivo config.json, localizado na pasta server, e altere conforme as informações de sua maquina;
	(IMPORTANTE: Não altere o ip local do memcached. Nos dados referente ao servidor, coloque IP de rede de sua maquina);


6º) No arquivo 'client.js', altere o valor de IP das constantes HOST_HTTP para o IP de rede da sua maquina;


7º) No arquivo 'client.js', altere o valor de IP das constantes HOST_TCP para o IP de rede do servidor que deseja acessar;
	(IMPORANTE: É recomendado manter os valores das portas);


8º) No arquivo 'script.js' altere na primeira linha, o ip e a porta conforme os valores de HOST_TCP e HOST_PORT do arquivo 'client.js'


9º) No navegador, digite o caminho até sua pasta client e acesse abra a pagina client.html
	(IMPORTANTE: Ao invés de digitar localhost, coloque o IP de rede da sua maquina).
