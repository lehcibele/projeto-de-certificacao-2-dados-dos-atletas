# 🏋️‍♀️ Projeto de Certificação 2 – Dados dos Atletas

## 📘 Sobre o projeto

Este projeto foi desenvolvido como parte da **Fase 8 - Projetos Avançados** da trilha de **Lógica de Programação** do **DEVstart**.  
O objetivo é criar uma aplicação em **JavaScript** capaz de:

- Receber as informações de um atleta;
- Calcular automaticamente sua **categoria**, **IMC (Índice de Massa Corporal)** e **média válida das notas**;
- Exibir todos os dados processados de forma organizada.

## 🧠 Conceitos aplicados

Durante o desenvolvimento, foram aplicados conceitos fundamentais de **Programação Orientada a Objetos (POO)**, como:

- **Classes e Objetos**
- **Encapsulamento**
- **Métodos e atributos**
- **Cálculos e manipulação de arrays**

## ⚙️ Estrutura da classe `Atleta`

A classe `Atleta` centraliza todos os atributos e métodos relacionados aos atletas.

### **Atributos**
- `nome` → Nome do atleta  
- `idade` → Idade do atleta  
- `peso` → Peso em kg  
- `altura` → Altura em metros  
- `notas` → Array contendo as notas atribuídas ao atleta

### **Métodos**
| Método | Descrição |
|--------|------------|
| `calculaCategoria()` | Retorna a categoria do atleta de acordo com sua idade |
| `calculaIMC()` | Calcula o IMC usando a fórmula `peso / (altura * altura)` |
| `calculaMediaValida()` | Calcula a média das notas válidas (seguindo o método do Projeto 1) |
| `obtemNomeAtleta()` | Retorna o nome do atleta |
| `obtemIdadeAtleta()` | Retorna a idade |
| `obtemPesoAtleta()` | Retorna o peso |
| `obtemNotasAtleta()` | Retorna as notas |
| `obtemCategoria()` | Retorna a categoria |
| `obtemIMC()` | Retorna o IMC calculado |
| `obtemMediaValida()` | Retorna a média válida |

## 🧮 Regras de cálculo

### **1. Categoria**
| Faixa etária | Categoria |
|---------------|------------|
| 9 a 11 anos | Infantil |
| 12 a 13 anos | Juvenil |
| 14 a 15 anos | Intermediário |
| 16 a 30 anos | Adulto |
| Outras idades | Sem categoria |

### **2. IMC**
> **Fórmula:**  
> `IMC = peso / (altura * altura)`

### **3. Média válida**

A média válida é calculada a partir das notas do atleta, desconsiderando a **maior** e a **menor** nota, e calculando a média das restantes.

## 💻 Exemplo de uso

```javascript
// Declara o atleta
const atleta = new Atleta(
  "Cesar Abascal",
  30, 
  80, 
  1.70,
  [10, 9.34, 8.42, 10, 7.88]
);

console.log(`Nome: ${atleta.obtemNomeAtleta()}`);
console.log(`Idade: ${atleta.obtemIdadeAtleta()}`);
console.log(`Peso: ${atleta.obtemPesoAtleta()}`);
console.log(`Altura: ${atleta.altura}`);
console.log(`Notas: ${atleta.obtemNotasAtleta()}`);
console.log(`Categoria: ${atleta.obtemCategoria()}`);
console.log(`IMC: ${atleta.obtemIMC()}`);
console.log(`Média válida: ${atleta.obtemMediaValida()}`);
```

## 🧾 Saída esperada

```
Nome: Cesar Abascal
Idade: 30
Peso: 80
Altura: 1.7
Notas: 10,9.34,8.42,10,7.88
Categoria: Adulto
IMC: 27.68166089965398
Média válida: 9.25333333
```

## 🚀 Como executar o projeto

1. Clone o repositório:
```
git clone https://github.com/lehcibele/projeto-de-certificacao-2-dados-dos-atletas.git
```

2. Acesse a pasta do projeto:
```
cd dados-atletas
```

3. Abra o arquivo dados-atletas.js em um editor de código (como VS Code).

4. Execute o código no console do navegador ou no Node.js:
```
node dados-atletas.js
```

## 🏆 Autor

**Letícia Cibele**

💡 Desenvolvido como parte do **DEVstart - Trilha 1: Lógica de Programação**

📅 Projeto de Certificação 1

🔗 [GitHub](https://github.com/lehcibele)