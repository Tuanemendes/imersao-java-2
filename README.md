
<div align="center">
    <img src="https://www.alura.com.br/assets/img/imersao-java/imersao-logo.1676983691.svg"width="250" height="80" alt="Imersão Alura"/>
</div>


<h1>👩‍💻 Java-stickers</h1>

<div align="center">

![Badge em Desenvolvimento ](http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge )
![GitHub Org's stars](https://img.shields.io/github/stars/tuanemendes?style=social)

</div>
<h2>Índice</h2>

* [Descrição do Projeto](#descrição-do-projeto)
* [Tecnologias utilizadas](#tecnologias-utilizadas)
* [Funcionalidades e Demonstração da Aplicação](#funcionalidades-e-demonstração-da-aplicação)
* [Tecnologias Utilizadas](#tecnologias-utilizadas)
* [Aula 01](#aula-1)
* [Aula 02](#aula-2)
* [Aula 03](#aula-3)
* [Aula 04](#aula-4)
* [Aula 05](#aula-5)
* [Desenvolvido Por](#desenvolvido-por)
* [Pessoas Contribuidoras](#pessoas-contribuidoras)


<h2>💻 Descrição do Projeto</h2>

<p>
O projeto tem como ojetivo de desenvolver uma aplicação  do zero em Java visando teoria por meio da prática amplição de portifólios e da carreira de dev. 
</p>

<h2>💻Tecnologias Utilizadas</h2>

|     |   |
| :--------: | :--------: |    
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original-wordmark.svg" width="40" height="40" /> | Java 17 |   
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" width="40" height="40"  /> | [VsCode](https://code.visualstudio.com/?wt.mc_id=vscom_downloads) |
| <img src="https://user-images.githubusercontent.com/54903202/229671656-e5e752f3-6aa8-4432-9b36-174f86669ff7.png" width="40" height="40" /> | [Coding Pack para Java](https://code.visualstudio.com/docs/languages/java#_install-visual-studio-code-for-java) |
| <img src="https://user-images.githubusercontent.com/54903202/229672038-342beb0f-f6bc-442d-9f2b-4e2ed2d99085.png"/> | [Proton VPN](https://protonvpn.com/) |
| <img src="https://user-images.githubusercontent.com/54903202/229672346-6f051572-5109-4185-92d9-2cf235804e65.png"/> | [IMDb-API](https://imdb-api.com/api)(*obs: VPN ligada) |
| <img src="https://user-images.githubusercontent.com/54903202/229672797-003c08c7-d735-49a1-acc3-7852f802e5d3.png" width="40" height="40"/> | [NASA-API](https://api.nasa.gov/) |
| <img src="https://img.icons8.com/color/40/null/spring-logo.png"/> | [Spring Initializr](https://start.spring.io/) |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-plain-wordmark.svg" width="40" height="40" /> | [MongoDB](https://www.mongodb.com/cloud/atlas/lp/try4?utm_content=rlsavisitor&utm_source=google&utm_campaign=search_gs_pl_evergreen_atlas_core_retarget-brand_gic-null_amers-all_ps-all_desktop_eng_lead&utm_term=mongodb&utm_medium=cpc_paid_search&utm_ad=e&utm_ad_campaign_id=14412646314&adgroup=131761122172&cq_cmp=14412646314&gclid=Cj0KCQjwz6ShBhCMARIsAH9A0qV-auOAO9-3MF2jGsKldDiosvvrVpqEfJQHYB5xz-peXjLt4-oY8WQaAmlBEALw_wcB) |
| <img src="https://user-images.githubusercontent.com/7853266/44114706-9c72dd08-9fd1-11e8-8d9d-6d9d651c75ad.png" width="40" height="40" /> | [Postman](https://www.postman.com/downloads/) |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" width="40" height="40" /> | [Docker](https://www.docker.com/) |        
| <img src="https://user-images.githubusercontent.com/54903202/229669708-f3093d2e-88fa-4503-a133-8266d5906811.png"/> | [Fly.io](https://fly.io/) |


<h2>💻Funcionalidades e Demonstração da Aplicação</h2>
<p>
    A inversão são de 5 dias de códificação em java criação de classes, conceitos de herença, polimorfismo, a utilização  do framework spring com a criação de uma API para ser consumida pelo próprio gerador de stickers,   implementação de desafios.  
</p>

<h2>👩‍🏫👨‍🏫Aula 1</h2> 
<p>
 
Na primeira aula ideia iniciamente é  consumir microserviços de uma  API dos top 250 filmes, no qual será utilizada a IMDb-API. Foi realizado cadatro no site da IMDb-API para conseguir buscar o dados dos Top250Movies, o site não funcionava dizendo estar fora do ar como o status 403, para resolução do problema, foi passado pelo time da alura um link pra buscar os dados e um segunda que encontrei foi utilizar uma VPN  que no qual foi possível acessar a o link do site IMDb-API.
Na classe main foi criado a  conexão com o  http para buscar o top 250 filmes. 
Foi criado uma JsonParser para fazer o processo de separação dos dados. 
Criado um for para trazer a lista com manipulação do dados titulo , poster, classificação.

</p>
<h3>🛠Desafios Dia 01</h3>

* Consumir o endpoint de filmes mais populares da API do IMDB. Procure também, na documentação da API do IMDB, o endpoint que retorna as melhores séries e o que retorna as séries mais populares.<br>
* Usar sua criatividade para deixar a saída dos dados mais bonitinha: usar emojis com código UTF-8, mostrar a nota do filme como estrelinhas, decorar o terminal com cores, negrito e itálico usando códigos ANSI, e mais!<br> 
* Colocar a chave da API do IMDB em algum lugar fora do código como um arquivo de configuração (p. ex, um arquivo .properties) ou uma variável de ambiente.<br>

<p>
Para aprimoarar os stickers foi implementado uma saudação ja enviar a messagem de bom dia, boa tarde, boa noite de acordo com a hora que for gerada.  
</p>


```java
            LocalTime horaAtual = LocalTime.now();
            String textoSaudacao;
            
            if(horaAtual.isBefore(LocalTime.of(12, 0))){
                textoSaudacao = "Bom dia!";
            }else if(horaAtual.isBefore(LocalTime.of(18,0))){
                textoSaudacao = "Boa tarde!";
            }else{
                textoSaudacao = "Boa Noite!";
            }

```



<div align="center">
    <img  src="https://user-images.githubusercontent.com/54903202/229676349-a20e3f5c-f553-4ae6-bf38-f03391869d2e.png" width="250" height="380" alt="Figura IMDBtop250">
</div>



<div align="center">
    <img  src="https://user-images.githubusercontent.com/54903202/229263265-7e4ace23-5d1d-4c04-b7fd-cf4b2cafb84e.png" width="650" height="100" alt="Terminal Estrelas">
</div>

<h2>👩‍🏫 👨‍🏫Aula 2</h2>
<p>
     Aula de Manipulação de imagem para gerar stickers pra whatsapp, com a utilização de bibliotecas Java para modificar tamanho da imagem , buscando  as imagens  da API  dos filmes passadno textos dentro dessas imagens
</p>

<h3>🛠Desafios Dia 02</h3>

* Redimencionar as imagens para ter um maior resolução.<br>
* Criar diretório de saída das imagens, se ainda não existir.<br>
* Centralizar o texto na figurinha.<br>
* Colocar outra fonte como a Comic Sans ou a Impact, a fonte usada em memes.<br>
* Colocar contorno (outline) no texto da imagem.<br>
* Colocar uma imagem de você que está fazendo esse curso sorrindo, fazendo joinha e fazer com que o texto da figurinha seja personalizado de acordo com as classificações do IMDB.

<div align="center">
    <img  src="https://user-images.githubusercontent.com/54903202/229262614-e9b22466-1b2d-4f17-952a-f2cdfef23ad4.png" width="250" height="380" alt="Figura IMDB">
</div>

<h2>👩‍🏫 👨‍🏫Aula 3</h2> 
<p>
 Aula de refatoração do código com foco em orientação obejtos para deixar mais seguro, manutenivel e organizado para  gerar  facilidade para outros                  desenvolvedores conseguir entender o código, foi separado as seguintes classes:
</p>

 <div align="center">
    <img  src="https://user-images.githubusercontent.com/54903202/229262211-24ebcb77-70cd-4037-bb74-9a987aafde37.png"  alt="Classes Java">
</div>
   
<p>
   Com essa refatoração sendo possível utilização de outras API pra gerar outros stickers como foi utilizado a API da NASA. 
</p>

<div align="center">
    <img  src="https://user-images.githubusercontent.com/54903202/229262393-d900483f-efe2-41e4-90c7-048a42acbcee.png" width="250" height="380" alt="Figura NASA">
</div>

<h3>🛠Desafios Dia 03</h3>


* Transformar a classe que representa os conteúdos em um Record, disponível a partir do Java 16.<br> 
* Criar as suas próprias exceções e usá-las na classe que implementa o cliente HTTP.<br> 
* Usar recursos do Java 8 e posterior, como Streams e Lambdas, para mapear uma lista em uma outra.<br> 
* Criar uma Enum que une, como configurações, a URL da API e o extrator utilizado. 

<p>
No desafio de transformar a class para record, foi necessário criar outro construtor para ter somente dois atribudos pois na record que foi criado tinha três atributos. 
</p>


``` java 
  public record Content(String title,String urlImage,double classification) {
    
    public Content(String title, String urlImage) {
        this(title, urlImage, 0.0); // classificação como padrão 0.0
    }
}

```

<p>
Realização do teste da exception criada.
</p>

<div align="center">
    <img  src="https://user-images.githubusercontent.com/54903202/229329515-7d66a41d-74ee-4181-a582-30fb86470fa5.png" width="650" height="100" alt="Terminal Exception">
</div>

<p>
 No desafio na criação do enum foi implementado uma lógica se caso for NASA_APOD ele consiga pegar as chaves do arquivo de configuração e a data que esta sendo passada para buscar mais  imagens e não somente do dia. 
</p>

 ```java
         if(api.equals(API.NASA_APOD)){
            //API Nasa
            String apiKeyNasa = properties.getProperty("NASA_API_KEY");
            String dateNasa = properties.getProperty("DATA_NASA");
            url = api.getUrl() + apiKeyNasa + dateNasa;

        }else{
            String apiKeyImdb = properties.getProperty("IMDB_API_KEY");
             url = api.getUrl() + apiKeyImdb;
        }

 ```
 
<h2>👩‍🏫 👨‍🏫Aula 4</h2>

<p>
Criação de uma API em spring que seria um projeto que tem como base ser pré configurado, que ao iniciar um projeto não é necesssario configurações como tomcat, gerenciamento de projeto com o maven, é tudo gerenciado por meio de dependências  com suas anotações. O projeto tem com objetivo criar uma API local incialmente para ser consumida a partir do primeiro projeto que foi criado para gerar os stickers, sua busca será por linguagens preferidas, sendo utilizando banco de dados mongoDB, para utilização do banco sendo necessário incluir as denpendencias do mongo no aquivo pom.xml do projeto spring  e  realizado as configurações  para buscar o banco de dados em nuvem.
</p>

<div align="center">
    <img  src="https://user-images.githubusercontent.com/54903202/229370710-e52f1043-f24f-41e2-97bf-eb016d6077a2.png" width="250" height="380" alt="Figura Linguagem">
</div>

<p>
Outra ferramenta muito importante para o desenvolvimento é o postman que é  software para realizar  busca de dados, inserir, deletar por meio dos endopoints da aplicação, ele possui uma gama de funcionalidades para realizar testes em uma API.  
</p>

<div align="center">
    <img  src="https://user-images.githubusercontent.com/54903202/229371928-6686d757-3896-44cf-97dd-d2738eff118b.png" width="700" height="350" alt="Terminal Exception">
</div>

<h3>🛠Desafios Dia 04</h3>

* Finalizar o CRUD (Create, Read, Update e Delete) para que se possa atualizar e excluir uma linguagem cadastrada;
* Devolver a listagem ordenada pelo ranking;
* Retornar o status 201 quando um recurso (linguagem, no nosso caso) for cadastrado através do POST; 

<p>
O desafio de ordenação é algo realmente muito simples , apenas criando uma linha de código na classe LanguageRepository foi possvel criar um método  findByOrderByRanking para ordernada a lista da linguagens.  
</p>

<div align="center">
    <img  src="https://user-images.githubusercontent.com/54903202/229381422-7decab87-5214-4d1f-aa87-bf5b2fa55a51.png" width="700" height="350" alt="Terminal Exception">
</div>
<p>
Desafio do status code para 201 created teve a alteração do metodo post para  ter uma  ResponseEntity 
</p>

<div align="center">
    <img  src="https://user-images.githubusercontent.com/54903202/229382002-ccb05a9b-2ee7-441d-a749-580e9645ca64.png" width="700" height="350" alt="Terminal Exception">
</div>

<h2>👩‍🏫 👨‍🏫Aula 5</h2>
Publicação da API no cloud 

<p>
Criação de um arquivo docker file  publicar a imagem no docker hub 
</p>

```docker
FROM openjdk:17-jdk-alpine
VOLUME /tmp
ARG JAVA_OPTS
ENV JAVA_OPTS=$JAVA_OPTS
COPY target/languages-api-0.0.1-SNAPSHOT.jar languagesapi.jar
EXPOSE 8080
ENTRYPOINT exec java $JAVA_OPTS -jar languagesapi.jar
# For Spring-Boot project, use the entrypoint below to reduce Tomcat startup time.
#ENTRYPOINT exec java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar languagesapi.jar

```

<p>
Criação da conta no Fly.oi para fazer o deploy do projeto para rodar em cloud.
</p>

<div align="center">
    <img  src="https://user-images.githubusercontent.com/54903202/229656160-92ef3507-a7e7-4e2e-8179-341c575a9c1a.png" width="700" height="350" alt="fly.io">
</div>

<p>
Realizado set para a senha do banco de dados
</p>

<div align="center">
    <img  src="https://user-images.githubusercontent.com/54903202/229674646-eacc729d-7677-46ab-b74c-26898a97f35d.png" width="700" height="80" alt="Set-senha">
</div>


Deploy finalizado com sucesso! <br>
link para acesso 👇 <br>
➡️ ➡️ ➡️ [languages-api](https://language-api-alura.fly.dev/languages) ⬅️ ⬅️ ⬅️ 

<h2>👩‍Desenvolvido Por</h2>

 [Tuane](https://www.linkedin.com/in/tuane-mendes/) 💙      

<h2>Pessoas Contribuidoras</h2>

 [Time Alura](https://www.alura.com.br/) 💙 <br>
 
 [Alexandre Aquiles](https://www.linkedin.com/in/alexandreaquiles/) <br>
 [Jacqueline Oliveira](https://www.linkedin.com/in/jacqueline-r-oliveira/) <br>
 [Paulo Silveira](https://www.linkedin.com/in/paulosilveira/)
 


