# Comunicação entre sistemas - REST e níveis de maturidade

- Muitos desenvolvedores já sabem trabalhar com REST
- Representational state of transfer. (Estado representacional de transferência)
- Surgiu em 2000 por Roy Fielding em uma dissertação de doutorado
- Simplicidade
- Stateless
- Cacheável

## REST: Níveis de maturidade (Richardson Maturity Model)

### Nível 0: The Swamp of POX
- Não possui padrão para comunição.

### Nível 1: Utilização de resources
- Há um padrão, metodos e verbos porem, nao utilizado corretamente
    | VERBO  | URI         | OPERACOES |
    | ------ | ----------- | --------- |
    | GET    | /products/1 | buscar    |
    | POST   | /products   | inserir   |
    | PUT    | /products/1 | alterar   |
    | DELETE | /products/1 | remover   |

### Nível 2: Verbos HTTP utilizados corretamente
    | GET    | buscar  |
    | ------ | ------- |
    | POST   | inserir |
    | PUT    | alterar |
    | DELETE | remover |

### Nível 3: HATEOAS: Hypermedia as the Engine of Application State
- Quando utilizamos corretamente as Resquests e Responses.
Nesse nivel, configuramos o header para dizer o que a API pode receber e retornar.

No response é enviado alem do solicitado, links que podem ser acessados a partir daquele ponto...

![](./assets/hateoas.png)