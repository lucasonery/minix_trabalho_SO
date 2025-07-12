# Projeto de Escalonamento - Minix 3

Este projeto implementa e compara três algoritmos de escalonamento no sistema operacional Minix 3, como parte de uma disciplina prática de Sistemas Operacionais.

## Organização do Repositório

O repositório está disponível em:  
[https://github.com/lucasonery/minix_trabalho_SO](https://github.com/lucasonery/minix_trabalho_SO)

### 🔄 Algoritmo Padrão (Round-Robin do Minix)
- **Localização**: branch `dev`
- **Responsável**: Lucas Nery
- **Descrição**: Essa versão contém o código original do Minix com as configurações padrão de escalonamento baseadas em prioridades com quantum fixo.

---

### 🕒 Algoritmo FCFS (First Come First Served)
- **Localização**: branch `vitorFCFV`  
- ⚠️ *Nome da branch está incorreto: aparece como `FCFV` em vez de `FCFS`*
- **Responsável**: Vitor Reis
- **Descrição**: Todos os processos recebem a mesma prioridade e um quantum extremamente alto, garantindo execução por ordem de chegada sem preempções desnecessárias.

---

### 🧠 Algoritmo SJN (Shortest Job Next)
- **Localização**: branch `vitor`
- **Responsável**: Vitor Reis
- **Descrição**: Processos são escalonados com base na estimativa de tempo de execução (burst). Essa estimativa é atualizada com base no histórico do processo, priorizando os que demandam menos tempo de CPU.

---

### 🎲 Algoritmo de Loteria (Lottery Scheduling)
- **Localização**: branch `vini_loteria`
- **Responsável**: Vinícius Corrêa
- **Descrição**: Cada processo recebe um número de "bilhetes". Um sorteio define qual processo será executado, com chances proporcionais ao número de bilhetes atribuídos.

---

## ⚠️ Limitações de Visualização

As alterações relacionadas aos **banners do sistema (1, 2 e 3)** e ao arquivo **`exec.c`** estão **disponíveis apenas** na branch `vitor`.  
Elas **não podem ser visualizadas** nas branches `vini_loteria` e `vitorFCFV`.

- **Banner 1 (boot)** e **Banner 3 (desligamento)**: modificados no arquivo `minix/kernel/main.c`
- **Banner 2 (mensagem pós-login)**: modificado em `/etc/motd`
- **Modificação no exec.c**: permite exibir no terminal qual binário está sendo executado (`/usr/src/minix/servers/pm/exec.c`)

---


## 👨‍💻 Autores

- **Lucas O. N. de Araújo** – lucas.nery@unifesp.br  
- **Vinícius A. Corrêa** – vinicius.correa@unifesp.br  
- **Vitor G. R. da Silva** – vitor.reis@unifesp.br  

UNIFESP - Universidade Federal de São Paulo  
Curso de Bacharelado em Ciência da Computação / Interdisciplinar em Ciência e Tecnologia
