# Comandos Docker (PT-BR) 
# Documentação

[Docker Flag Documentation](https://docs.docker.com/engine/reference/commandline/docker/) 

[Docker Reference Documentation](https://docs.docker.com/reference/) 

## Onde usar

É preciso utilizar em terminal Powershell quando estamos no Windows, mesmo no VSCode.

# Comandos

### Escolher sistema

Escrever no arquivo _Dockerfile_ o sistema e a versão que queremos instalar

_FROM debian:buster_


### Criar uma imagem

_docker build -t ingate-debian_

--tag, -t **&#10132;** Nomeia ou adiciona uma _flag_ no formato 'name:tag' 

### Rodar _container_

_docker run --rm -it --name meu-container -p 8080:8000 -v ${PWD}:/app ingate-debian_

##### Flags escritas no exemplo acima

--rm **&#10132;** deleta tudo ao desligar aplicação ou computador, ou quando finalizar _container_

-it **&#10132;** flag para poder interagir com o _docker_. (computador &#8594; _docker_)

--name **&#10132;** nomeia o _container_. O _default_ é um nome maluco qualquer gerado pelo _docker_

-p 8080:8000 **&#10132;** -p é a flag para criar porta. 8080 é a porta de acesso do meu computador que quero que ele utilize. 8000 é a porta que eu quero que dentro do _container_ ele disponibilize. É possível indicar portas diferentes destas do exemplo

-v **&#10132;** Monta um novo volume (da mesma forma que é montado um volume ao plugar um pendrive). Ele é totalmente sincronizado com nossa máquina. Se rodar em cmd, ${PWD} fica %cd%, que é $(pwd) do Mac. :/app cria um diretório /app dentro da raiz onde estamos com o container montado. **cd** significa _current director_.

ingate-debian **&#10132;** nome da imagem criada

### Listar todos os _containers_

_docker ps_