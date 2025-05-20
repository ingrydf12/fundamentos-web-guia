![\[Image\]()](https://github.com/ingrydf12/fundamentos-web-guia/blob/master/docs/introducao.PNG?raw=true)


# Tags e estrutura

[Referências](https://www.hostinger.com.br/tutoriais/o-que-e-html-conceitos-basicos)

Uma tag diz para o navegador onde um elemento começa e termina, enquanto um **atributo** descreve as características de um elemento.

As tags são marcadas por 3 elementos principais:
- Tag de abertura – usada para dizer onde um elemento começa a ter efeito. A tag é cercada de colchetes angulares para abertura e fechamento. Por exemplo, use a tag de abertura ```<p>``` para criar um parágrafo.
- Conteúdo – essa é a parte que os usuários verão.
- Tag de fechamento – igual à tag de abertura, mas com uma barra antes do nome do elemento. Por exemplo, ```</p>``` para encerrar um parágrafo.

**Exemplo completo:**

```html
<p>Este é um parágrafo de exemplo.</p>
```

Mas a parte ainda bônus do HTML são os **atributos das tags**, que possuem **um nome e um valor**.

Os atributos são características adicionais dadas para aquele elemento e que sempre são especificados na tag de abertura. Um elemento pode ter vários atributos.

### Características dos atributos:
- Sempre no formato nome="valor"
- Podem modificar o comportamento ou aparência do elemento


### Atributos Comuns:

**Atributos Globais (funcionam em quase todas as tags):**

- id: Identificador único
- class: Classificação para CSS/JavaScript
- style: Estilos CSS inline (ou seja, direto no HTML)
- title: Texto de tooltip (bom para acessibilidade)
- lang: Define o idioma do conteúdo

**Atributos Específicos:**

- ```<a>```: href, target, rel
- ```<img>```: src, alt, width, height
- ```<input>```: type, name, value, placeholder

#### Notas:

href -> referencia links externos ou links para própria página, ex.: âncoras para seções específicas.
src -> referencia localmente no projeto ou em endereços de imagens.

Você pode visualizar mais e ver detalhes sobre as tags e respectivos atributos aqui:
[Guia de tags - Hostinger](https://www.hostinger.com.br/tutoriais/codigos-html-prontos-guia-pdf)

# O que são class e id nas propriedades das tags HTML?

Classes são atributos globais no HTML que permitem agrupar elementos com características ou funções semelhantes, facilitando a estilização e também, manipulações em Javascript. Podem ser repetidas várias vezes em um mesmo documento HTML e é uma boa prática usar nomes que descrevam o propósito semântico do elemento, em vez de sua representação.

Já os IDs, como seu próprio nome diz, é um identificador exclusivo e pela própria documentação do MDN Docs:
-  Seu objetivo é identificar o elemento ao navegar por âncoras (usando um identificador de fragmento), quando utilizar scripts ou estilizando (com CSS).

## E qual a diferença? Qual devo usar em que contextos?

Não existe um certo ou errado nisso, mas você pode seguir as boas práticas de programação. 

- Classes podem ser repetidas, mas IDs são únicos.

Normalmente utilizamos classes para elementos que podem repetir seu estilo ou que não precisam de algum tipo de interação. Caso queira particularizar o uso de determinada tag, usa-se ID, como exemplo é uma interação ou microanimação para aquela tag.

- Você pode usar a mesma classe para vários elementos;
- Você pode usar várias classes para um mesmo elemento.