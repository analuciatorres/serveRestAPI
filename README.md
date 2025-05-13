# Dominando Postaman
Teste de API Rest do manual ao CI/CD
serveRestAPI


## Sobre o que é este projeto
Este repositório foi criado para o curso Dominando Postman para teste de API Rest

## Tecnologias utilizadas
- Postman
- node version v18.18.0
- newman 6.2.1
- newman-reporter-html

## Documentação
Doc da api ServeRest: [Consulte Swagger](https://serverest.dev/)

## Como Instalar o ambiente
- Primeiro instele o node no seu computador [baixe aqui](https://serverest.dev/#/)
- Segundo realize a instalação do newman de forma global
  
  ``
  npm install -g newman
 ``

  Em caso de dúvidas consulte a [Documentação newman](https://www.npmjs.com/package/newman)

- Terceiro realize a instalação da dependência dos relatórios (opicional)

```
  npm install -g newman-reporter-htmlextra
```

  Em caso de dúvidas consulte a [Documentação newman-reporter-htmlextra](https://www.npmjs.com/package/newman-reporter-htmlextra)
  
## Como rodar os testes

### Pelo Postman web ou  desktop
- Importe a colection e o environment
- Execute os teste de forma manual ou automatizada

### Pelo Newman
- Abra o console de sua preferência
- Execute a seguinte linha de comando para rodar os testes
```
newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli
 ```

 - Execute a seguinte linha de comando para rodar os testes gerando relatório com o newman-reporter-htmlextra 
  
  ```
  newman run ServeRest.postman_collection.json -e serveRest_env.postman_environment.json -r cli,htmlextra
  ```

### Report
Se você optou por rodar os testes com report-htmextra, você gerou um arquivo com o resultado dos serus testes e para verificar as validações você pode abrir a pasta **newman** que foi criada no local em que os arquivos de colection e environment se encontram

## Entre em contato
Em caso de dúvidas, sugestões e colaborações por favor entre em contato pelo email torres.analucia@gmail.com ou pelo [Linkedin](https://www.linkedin.com/in/analuciatorresdasilva/)

