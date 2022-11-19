# Notas Desenvolvimento Web Front-end (PUC Minas)
<!--ts-->
- [Os padrões da web](#os-padrões-da-web)
    - [Documentação do W3C](#documentação-do-w3c)
- [Arquitetura Web](#arquitetura-web)
    - [Modelo Cliente-Servidor](#modelo-cliente-servidor)
    - [Internet](#internet)
    - [Protocolo HTTP](#protocolo-http)
    - [URI](#uri)
    - [URL](#url)
    - [URN](#urn)
<!--te-->

***
## WWW - World Wide Web
>Sistema de informação interligado por hipertexto.

- [What is Web 2.0 - O'Reily Media, 2005](https://www.oreilly.com/pub/a/web2/archive/what-is-web-20.html)

# Os padrões da web

Entre os padrões mantidos pelo [W3C](https://www.w3.org/standards/), podemos citar:

- Design e Aplicações Web (HTML, CSS, SVG, Ajax, Acessibilidade);
- Arquitetura da Web (Protocolo HTTP, URI);
- Web Semântica (Linked Data - RDF, OWL, SPARQL);
- Web Services (SOAP, WSDL);
- Tecnologia XML (XML, XML Schema, XSLT);
- Navegadores e ferramentas de autoria.

## Documentação do W3C

O W3C estabelece um processo rigoroso para a manutenção dos padrões mantidos pela organização. Um padrão passa pelos seguintes estágios antes de ser liberado formalmente para o mercado:

- Working Draft (WD);
- Candidate Release (CR);
- Proposed Recomendation (PR);
- Recomendation (REC).

# Arquitetura Web

## Modelo Cliente-Servidor

- Cliente requisita por meio `URI`;
- Servido corresponde por meio do protocolo `HTTP`.

## Internet

É uma rede mundial de computadores baseada no protocolo TCP/IP, em que todo computador conectado é denominado host (hospedeiro) e possui um identificador endereço `IP` (Internet Protocol) no padrão A.B.C.D (ex: 200.20.15.22). `DNS` troca os números para um nome legível pelo usuário (ex: www.google.com).

A `URL` (Uniform Resource Locator), é um texto codificado que traz todos os detalhes sobre o recurso solicitado pelo ambiente cliente. A URL, é um tipo de `URI` (Uniform Resorce Identifier), padrão utilizado na Internet para referenciar recursos dos mais diversos tipos como páginas, imagens, vídeos, até pessoas, produtos e outras entidades. A URI, seja uma URL ou uma URN, funciona tal qual o CPF para pessoas.

## Protocolo HTTP

`HTTP` é a forma como clientes e servidores se comunicam na rede. As requisições e as respostas obedecem aos padrões estabelecidos pelo protocolo HTTP.

A requisição `HTTP` é um pacote de dados enviado através da Internet pelo Cliente Web para o Servidor Web e identifica o recurso solicitado e como ele deve ser entregue. A resposta `HTTP` é formada por pacotes de dados enviados pelo `Servidor Web` para o `Cliente Web` com o recurso solicitado.
>[HTTP - Mozilla.org](https://developer.mozilla.org/pt-BR/docs/Web/HTTP)
## URI

`URI` (Uniform Resource Identifier) é um padrão para o endereçamento de recursos disponíveis na rede que engloba os conceitos de `URL` (Uniform Resource Locator) e `URN` (Uniform Resource Name).

## URL

O URL (Uniform Resource Locator) é um padrão de URI que serve para referenciar um recurso e sua localização, normalmente na Internet. O URL é composto pelas seguintes partes:

- Esquema – identifica a forma de interação entre um cliente e um servidor, como por exemplo, http, https, ftp, entre outros;
- User:pass – informações de usuário;
- Host – nome ou número IP onde se encontra a aplicação servidor;
- Porta – identifica a porta TCP/IP associada ao servidor. A porta padrão do HTTP (80) pode ser omitida;
- Caminho – indica o local exato onde o recurso se encontra;
- Query – dados não hierárquicos, detalhando a consulta normalmente sob a forma de pares nome e valor;
- Fragmento – identifica uma seção no recurso.

## URN

O `URN` (Uniform Resource Name) é um tipo de `URI` que identifica um recurso específico (NSS) pelo nome em um namespace (NID), sem expressar a sua localização. No exemplo “urn:isbn:978-1-491-91866-1”, utilizamos a `URN` para identificar um livro a partir do seu código de ISBN, sem dizer onde esse livro está localizado.


>[Identificando recursos da web - Mozilla.org](https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Basics_of_HTTP/Identifying_resources_on_the_Web)