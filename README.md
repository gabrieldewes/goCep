# goCep
Projeto em Golang para buscar dados do CEP e armazenar em cache 

# Compilar

Além de ter o Go instalado no sistema operacional é necessário executar:

	export GOPATH=/path/goCep
	go get github.com/go-martini/martini
	go get github.com/andelf/go-curl
	/** 
	*  Verifique se você tem libcurl (e seus dev headers, static/dynamic libs) instalados!
	*  $ sudo apt install libcurl-gnutls-dev 
	*  $ pkg-config --libs libcurl
	**/
	go get github.com/ryanuber/go-filecache
	go build

# Executar

O binário chamado goCep será criado. Basta executá-lo e ele ficará ouvindo na porta 3000 por novas requisições.
Ou,
	go run server.go

# Testando
Para rodar os tests, você pode executar:

	go test

# Uso

Basta acessar a URL como no exemplo abaixo

	http://localhost:3000/cep/89201405

O retorno será um JSON com o conteúdo 
