# Testes unitários em Jest

O objetivo desta atividade é construir e testar códigos escritos em JavaScript

Dado o seguinte código : 
  
```javascript
function sum(a, b) {
  return a + b;
}

function sub(a, b) {
  return a - b;
}

function buildObject(length) {
  let obj;

  for (let i = 1; i <= length; i++) {
    // faz a copia do objeto e cria uma key com o valor do i atual  e.g. {'1' : 1, '2': 2}
    obj = { ...obj, [i]: i };
  }

  return obj;
}

function sumPositiveNumber(a, b) {
  if (a <= 0 || b <= 0) {
    throw new Error("Not allowed zero or negative numbers");
  }

  return sum(a, b);
}

module.exports = { sum, sub, buildObject, sumPositiveNumber };
```

O código acima possui quatro funções em declaras em JavaScript.
A seguir avalia o código de testes para executar essas funções e tentar validar sua corretude : 
```javascript
const { sum, sub, buildObject, sumPositiveNumber } = require("../src");

describe("Expect to be", () => {
  it("Sum 2 + 3 and sub 3 always shold be equal 2", () => {
    const result = sub(sum(2, 3), 3);

    expect(result).toBe(2);
  });
});

describe("Expect to equal", () => {
  it("Should correctly build object", () => {
    const obj = buildObject(3);

    expect(obj).toEqual({ "1": 1, "2": 2, "3": 3 });
  });
});

describe("Expect to throw exception", () => {
  it("Shouldn't sum unless both numbers are positive", () => {
    const result = () => sumPositiveNumber(-3, 3);

    expect(result).toThrow("Not allowed zero or negative numbers");
  });
});
```

O código acima requere as funções previamente declaras e executa as mesmas testando seus valores usando notações específicas e determinadas para definir os valores esperados pela execução do codigo, como o `expect toThrow` ou `expect toEqual`.
Acesse a documentação do [Jest](https://jestjs.io/) e veja as demais notações usadas para validação de resultados dos testes.