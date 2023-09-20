1.Abri o Terminal;
Digite:
sudo apt install python3-pip
Aguarde a instalação
pip3 install --user nodeenv
Aguarde a instalação
Teste a instalação do nodeenv digitando:
nodeenv –version


2.;
Abra um terminal, selecione a pasta onde ficará a pasta que irá conter o NodeJs.
digite:
nodeenv nodejs-env
onde: nodeenv é o comando
e nodejs-env é o nome da pasta (diretório) que irá ser instalado o NodeJs
Após a instalação para ativar esta versão do NodeJs, digite:
source ./nodejs-env/bin/activate
O indicador de prompt irá mudar, sinalizando que você está com o ambiente ativo.
Para testar digite:
node --version
Será informado a versão do NodeJs que está habilitada neste terminal 
Para desativar digite:
deactivate_node
O prompt irá sinalizar que o ambiente não está mais ativo


3.Abra um terminal, ative o NodeJs de sua preferência, digite:
source ./caminho_do_nodejs_env/bin/activate


4.Abrir o arquivo utilizando:
sudo nano index.js"ou"nome do arquivo;

5.Colar o código:
var http = require('http');

http.createServer(function (req, res) {
  res.writeHead(200, {'Content-Type': 'text/html; charset=utf-8'});

 var dataAtual = new Date();
 var dataFormatada = dataAtual.toLocaleDateString('pt-BR');

  res.end('<h1 style="font-size: 24px;">Marcos Antônio<h1>\n<P>Data atual: ' + dataFormatada + '</p>');
}).listen(8011);

6.Sair e Salvar, apertando "X"

7. digitar no terminal para iniciar o servidor:
node index.js

8. Testar no nevagador:
localhost:8011/
