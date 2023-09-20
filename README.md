1.Abri o Terminal;

2.Escolher uma pasta;

3.Crie um Arquivo para o Servidor;

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

7. digitar no terminal:
node index.js

8. Testar no nevagador:
localhost:8011/
