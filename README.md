# IZI MEI


                   
## Teste para desenvolvedor

**Leia atentamente as instruções abaixo e responda as questões da melhor forma possível.**

O teste será composto de três perguntas técnicas e uma avaliação prática.

Responda as perguntas com suas palavras, com o seu entendimento sobre o tema.

Publique o teste prático com as respostas em um arquivo readme em um repositório git-hub e envie o link para dev@meifacil.com.


**Perguntas:**

- Explique com suas palavras o que é domain driven design e sua importância na estratégia de desenvolvimento de software.

- Explique com suas palavras o que é e como funciona uma arquitetura baseada em microservices. explique ganhos com este modelo, desafios em sua implementação e desvantagens.

- Explique qual a diferença entre processamento sincrono e assincrono e qual o melhor cenário para utilizar um ou outro.

> STATELESS(assincrono) não mantem o estado apenas processa a função invocada, STATEFULL(sincrono) mantem o estado de cada cliente e usará do mesmo para as próximas respostas.
> STATELESS(assincrono) é massa pra spa e pra mobile apps, STATEFULL(sincrono) atende bem a sistemas web monoliticos


#### Teste prático:

Regra de negócio:

Criar um microservices que, através de um http post efetue um pagamento junto com o débito em uma conta corrente e o credito em outra conta. O valor líquido a ser creditado deve ser calculado em cima das seguintes taxas.
Saldo inicial pode ser fixo.

        
| **Parcelas**  | **Taxa**  |
|---|---|
| [**_1_**] |  [**_3,79%_**]  |
| [**_2_**] |  [**_5,78%_**]  |
| [**_3_**] |  [**_7,77%_**]  |
        
       

<code>Entidades: pagamento, contacorrente, lançamentos (você pode incrementar com outras entidades se achar necessário)</code>

<code>Parâmetros de entrada:
Valor
Parcelas
Conta origem
Conta destino</code>

<code>Parâmetros de saída: 
http status code
Valor líquido
Saldo conta origem
Saldo conta destino</code>

<code>Informações adicionais:
O método “post” devera receber os parametros no body da requisição em formato json</code>

<code>Serão avaliados critérios de arquitetura como separação de responsabilidade, clean code, segurança e testes</code>

**Tecnologias que você pode utilizar .net core 2.X, c#, node.js, nestjs, express**
