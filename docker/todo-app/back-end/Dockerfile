#Imagem utilizada / nome da aplicação
FROM node:14-alpine AS todobackend
WORKDIR /
#Expoe em qual porta a aplicação irá rodar (3001 do host, não muda nada apenas descrição)
EXPOSE 3001
#Para evitar executar o comando npm install, Add e descompacta todo o node modules
ADD /node_modules.tar.gz .
# copia o restante do diretório back end
COPY . .
#Executável que o container irá usar/comando(último comando executado)
ENTRYPOINT [ "npm start" ]