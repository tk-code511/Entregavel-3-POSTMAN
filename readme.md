# API de Operações Matemáticas

Projeto desenvolvido em JavaScript utilizando Node.js e Express.

## Como executar

Primeiro, instale as dependências:

```bash
npm install
```

Depois, execute o servidor:

```bash
node app.js
```

O servidor será iniciado em:

```text
http://localhost:3001
```

## Rotas

### Soma

**POST**

```text
http://localhost:3001/soma
```

JSON enviado no Postman:

```json
{
    "a": 10,
    "b": 5
}
```

Resposta:

```text
O resultado da soma de 10 e 5 é 15
```

### Subtração

**POST**

```text
http://localhost:3001/subtracao
```

JSON:

```json
{
    "a": 10,
    "b": 5
}
```
Resposta:

```text
O resultado da subtração de 10 e 5 é 5
```


### Multiplicação

**POST**

```text
http://localhost:3001/multiplicacao
```

JSON:

```json
{
    "a": 10,
    "b": 5
}
```

Resposta:

```text
O resultado da multiplicação de 10 e 5 é 50
```


### Divisão

**POST**

```text
http://localhost:3001/divisao
```

JSON:

```json
{
    "a": 10,
    "b": 5
}
```

Resposta:

```text
O resultado da divisão de 10 e 5 é 2
```


## Testando no Postman

No Postman, selecionar o método **POST** e utilizar:

```text
http://localhost:3001/soma
```

Depois, em **Body → raw → JSON**, colocar:

```json
{
    "a": 10,
    "b": 5
}
```

Para testar as outras operações, basta trocar a parte final da URL:

```text
/soma
/subtracao
/multiplicacao
/divisao
```

mantendo o mesmo formato do JSON.
