# ROBSON FERREIRA


# Olá Robson



## Estou em transição de carreira para a aréa de desenvolvimento web.
## Já Possuo algum conhecimento em HTML, CSS, JAVA SCRIPT e PYTHON.



A minha contribuição é mostra esse erro que dar ao tenta clona um desktop.


Ao tenta clona utilizando o git clone + "URL" ocorreu o seguinte erro.

" error: RPC failed; curl 56 schannel: failed to read data from server: SEC_E_DECRYPT_FAILURE (0x80090330) - Os dados especificados no puderam ser decodificados.
error: 1545 bytes of body are still expected
fetch-pack: unexpected disconnect while reading sideband packet
fatal: early EOF
fatal: fetch-pack: invalid index-pack output "

Esse erro se dar porque as versões atuais do protocolo HTTP, HTTP/2 e HTTP/3 o git não linda bem com o HTTP/2 e o HTTP/3.

Para baixa o arquivo git no desktop basta definir temporariamente que o Git use a versão HTTP/1.1 com o seguinte comando.

git -c http.version=HTTP/1.1 ou seja ficar dessa forma.

Ex: git -c http.version=HTTP/1.1 clone "URL"

Descreva as alternativas que você considerou
Para que fique mais completa a solução adicione o seguinte comando --depth=1 ficando da seguinte forma.
Ex; git -c http.version=HTTP/1.1 clone --depth=1 "URL"

Esse comando --depth serve para baixa a última versão do arquivo que deseja baixa.

Contexto adicional
Adicione qualquer outro contexto ou captura de tela sobre a solicitação de recurso aqui.


