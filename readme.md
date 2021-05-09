# Projeto "HELLO" 

Esse projeto tem como finalidade exemplificar um "Hello World" em Go. 

## Introdução a Go

- Surgiu em meados de 2009
- Uma linguagem considerada "Futurista"
- Possui 25 palavras chave
- Google estava precisando de uma linguagem de compilação mais rápida que a C
- Fácil de ser aprendida
- Modularizado, ou seja, trabalha com módulos

## Instale o Go

### Windows

Basta que siga o executável, para isso clique [aqui.](https://golang.org/)

### Linux

Para instalar em seu linux, siga os passos a seguir:

1 - Baixe o arquivo ".tar.gz". Basta clicar [aqui.](https://golang.org/dl/go1.16.4.linux-amd64.tar.gz)

2 - Extraia em `/usr/local/go`, para isso siga o comando a seguir:

```sh
sudo rm -rf /usr/local/go && sudo tar -C /usr/local -xzf go1.16.4.linux-amd64.tar.gz 
```

**Obs:** Caso esteja em root, não será preciso digitar "sudo", para inserir sua senha de usuário.

3 - Agora crie uma variável de ambiente, para isso basta digitar o seguinte comando a seguir:

```sh
gedit .bashrc # entrar no arquivo .bashrc pelo editor de texto 
```

Cole no final do arquivo a seguinte linha

```sh
export PATH=$PATH:/usr/local/go/bin
```

4 - Recarregue o terminal. basta usar `source .bashrc`
5 - Digite o comando: `go version`

Se você fez direitinho, perfeito! Você tem o Go instalado e pronto para ser usado :)

### MacOS

Se você tem um Macbook basta clicar [aqui.](https://golang.org) e baixar o ".dmg", criar uma "PATH" para `/usr/local/bin/`, reiniciar o Terminal e pronto, o Go está instalado :)

## Estrutura do Go

### Sua pasta

O go tem um diretório todinho para ele na pasta do seu usuário, veja:

- **Windows:** C:/Users/seu-usuario/go
- **Linux & MacOS:** /home/seu-usuario/go

**Obs:** Caso não tenha, use esse comando no seu terminal `mkdir go`

### Estrutura da pasta "go"

```sh
pasta-do-usuario/
└── go
    ├── bin
    ├── pkg
    └── src
```

- **bin**: Onde vai ficar o executável dos seus projetos

- **pkg**: Onde fica os pacotes compartilhados do Go (Pois ele é modularizado)

- **src**: Onde vai ficar seus códigos/projetos em Go

  

## Executando esse projeto

Conteúdo do arquivo:

```go
// Ajuda na hora de criar um executável
package main
// Importa o módulo fmt
import "fmt"
// função principal
func main() {
    // print na tela
    fmt.Println("Hello World!")
}
```

Para executar este projeto, basta seguir estas etapas (Lembrando que você tem que ter o Go já instaldo):

- Clone o repositório, para a pasta "src" que está na pasta go dentro do seu usuário.

```sh
cd $HOME/go/src # caso windows subistitua "$HOME" por c:/Users/seu-user/go/src

# clone dentro da pasta "src" 
git clone https://github.com/JoaoValentimDev/hello-world-go
```

- Extraia o "hello-world-go-main.zip" com um gerenciador de pacotes compactados, como winrar por exemplo.
- Entre na pasta do projeto.

```sh
cd hello-world-go-main
```

- Execute o seguinte comando:

```sh
go run hello.go
```

- Caso queira criar um executável use o comando a seguir:

```sh
go build hello.go
```

- Para executar basta digitar o nome do executável:

```sh
./hello
```

Parabéns, você executou um "Hello World!" em Go!
