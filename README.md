# 📄 Sistema de Estacionamento – Projeto LAB

## 📌 Descrição

Este projeto consiste no desenvolvimento de um **sistema para gerenciamento de um estacionamento**.
O objetivo é permitir que o operador possa **adicionar veículos**, **remover veículos** (com cálculo automático do valor a pagar) e **listar todos os veículos estacionados** de forma prática e eficiente.

O sistema deverá ser simples, interativo e permitir a manipulação das informações em tempo real.

---

## 🎯 Objetivos do Projeto

* Controlar a entrada e saída de veículos no estacionamento.
* Calcular automaticamente o valor da estadia de cada veículo.
* Listar todos os veículos estacionados no momento.
* Oferecer uma interface de interação clara e intuitiva (linha de comando ou aplicação gráfica, dependendo da abordagem do LAB).

---

## 🛠 Funcionalidades

1. **Adicionar veículo**

   * Solicitar a placa do veículo.
   * Armazenar na lista de veículos estacionados com o horário de entrada.

2. **Remover veículo**

   * Solicitar a placa do veículo.
   * Calcular o tempo estacionado e o valor total a ser pago.
   * Remover o veículo da lista de veículos ativos.

3. **Listar veículos**

   * Mostrar todas as placas e horários de entrada dos veículos atualmente estacionados.

4. **Configurações de preço**

   * Definir um valor inicial e uma taxa por hora adicional.

---

## 🧮 Lógica de Cálculo de Preço

O valor total será calculado da seguinte forma:

```
valor_total = valor_inicial + (taxa_por_hora * horas_adicionais)
```

* **Valor inicial**: taxa mínima cobrada.
* **Taxa por hora**: valor a ser adicionado para cada hora além da primeira.
* O tempo fracionado poderá ser arredondado para cima.

---

## 🚀 Tecnologias e Ferramentas

Dependendo do ambiente do LAB, poderá ser implementado usando:

* **C#** (Console Application ou Web API)
* **Java** (Console ou Spring Boot)
* **Python** (CLI ou Flask/Django)
* **Banco de Dados**: Em memória (listas/arrays) ou persistente (SQLite, MySQL, etc.)

---

## 📂 Estrutura do Projeto (Exemplo para C#)

```
/SistemaEstacionamento
│
├── Program.cs          # Ponto de entrada do sistema
├── Veiculo.cs          # Classe de modelo para veículo
├── Estacionamento.cs   # Classe responsável pela lógica de negócios
├── README.md           # Documentação do projeto
└── bin/                # Arquivos compilados
```

---

## 📋 Requisitos

* Ambiente de desenvolvimento configurado (ex.: Visual Studio, IntelliJ, VS Code).
* Conhecimento básico na linguagem escolhida.
* Noções de lógica de programação e estruturas de dados.

---

## 🔍 Exemplo de Uso (Fluxo no Console)

```
--- SISTEMA DE ESTACIONAMENTO ---
1 - Adicionar veículo
2 - Remover veículo
3 - Listar veículos
4 - Sair
Selecione uma opção: 1
Digite a placa: ABC-1234
Veículo adicionado com sucesso!

Selecione uma opção: 3
Veículos estacionados:
- ABC-1234 (Entrada: 14:32)
```

---

## 📜 Licença

Este projeto é de uso livre para fins educacionais e experimentais.

---

Se quiser, eu também posso já preparar uma **versão pronta com código funcional** para este sistema em C# ou Python.
