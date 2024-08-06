Aprendizados (Aula 1):

GO:
- go version (basics ;P)
- go mod init github.com/Raphael-GC/ama (cria o arquivo go.mod)
- 

Docker:
- compose.yml (arquivo principal onde configuramos quais serviços utilizaremos e em quais portas eles serão utilizados)
- Ao passar portas podemos usar variáveis de ambiente qual a seguinte sintaxe: ${NOME}:5432 ; Do lado direito é a porta dentro do container e do lado esquerdo (variável de ambiente) é o externo ao container.
- Ao passar variáveis de ambiente é importante que as mesmas estão configuradas no PATH do Host, ou uma outra maneira seria ter um arquivo ".env", que contenha os valores dessas variáveis, no mesmo diretório onde estar o arquivo "compose.yml"
- Como ao desligar o docker perdemos as informações, e as infos do banco de dados precisam ser persistidas, uma das maneiras de contornar isso é usando Volumes. Onde FileSystem interno se comunica com o lado externo e repassa essa informação, clonando tudo para o host, seja ele uma maquina local ou um S3 por exemplo.
- 

PostgreSQL:
-