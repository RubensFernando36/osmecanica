# 🔧 Sistema de Oficina Mecânica

## 📋 Descrição

Este projeto representa o modelo conceitual e lógico de um sistema de **gestão de ordens de serviço (OS)** para uma oficina mecânica. Ele permite o controle de clientes, veículos, equipes de mecânicos, serviços realizados, peças utilizadas e valores cobrados com base em uma tabela de referência de mão de obra.

---

## 🎯 Objetivo do Sistema

- Cadastrar clientes e seus veículos.
- Registrar ordens de serviço (OS) com data de emissão, status, valor total e previsão de conclusão.
- Designar equipes de mecânicos para cada OS.
- Incluir serviços realizados e peças utilizadas em cada OS.
- Calcular o valor da OS com base nos serviços e peças associadas.

---

## 🧱 Entidades Principais

- **Cliente:** Dados pessoais e contato.
- **Veículo:** Associado a um cliente.
- **Ordem de Serviço (OS):** Registro central da manutenção.
- **Equipe:** Conjunto de mecânicos.
- **Mecânico:** Com especialidade e histórico.
- **Serviço:** Ligado a uma tabela de referência de mão de obra.
- **Peça:** Componentes utilizados com valor unitário.
- **Item_Serviço / Item_Peça:** Itens aplicados em cada OS.
- **Tabela de Referência de Mão de Obra:** Base de preços para serviços.

---

## 🧩 Modelo Conceitual

> Diagrama ER disponível na pasta `diagrama/` ou abaixo:
<img width="951" height="1126" alt="Desafio2" src="https://github.com/user-attachments/assets/5c99717f-f5c6-4c5e-b816-32595bed2107" />



---

## ⚠️ Considerações

- Os valores calculados da OS são a soma dos serviços (`Item_Serviço`) e peças (`Item_Peça`).
- Apenas o ID da OS é mantido nas tabelas associativas para evitar redundância.
- O campo `Autorizada` define se o cliente liberou a execução do serviço (0 = Não, 1 = Sim).

---
