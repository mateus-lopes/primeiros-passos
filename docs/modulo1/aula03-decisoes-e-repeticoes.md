# 1.3 · Decisões e repetições

!!! abstract "Hoje você vai…"
    Aprender a escrever instruções que **escolhem** o que fazer e que **repetem** coisas, montando a sua ficha de treino como um algoritmo. ⏱️ ~1h

---

## Explicação

Até agora, os nossos algoritmos seguiam sempre a mesma linha reta: passo 1, passo 2, passo 3… Isso é a **sequência**.

Mas a vida real não é tão certinha. Às vezes a gente precisa **decidir** o que fazer, e às vezes precisa **repetir** a mesma coisa várias vezes. Os programas também!

### 🔀 Decisão: SE… SENÃO…

Pense no vôlei. Depois de cada jogada, alguém precisa decidir de quem é o ponto:

```text
SE a bola caiu dentro da quadra adversária:
    o ponto é nosso
SENÃO:
    o ponto é delas
```

O **SE** faz uma pergunta que só pode ter duas respostas: **sim ou não**. Essa pergunta se chama **condição**.

- Se a resposta for **sim**, faz o que está embaixo do **SE**.
- Se for **não**, faz o que está embaixo do **SENÃO**.

O **SENÃO** é opcional. Às vezes a gente só quer fazer algo **se** uma coisa for verdade, e pronto:

```text
SE a unha estiver com esmalte antigo:
    remover com acetona
```

Se não tiver esmalte antigo, simplesmente pula essa parte e segue a vida. 💅

### 🔁 Repetição: REPITA…

Agora pense no treino. Em vez de escrever:

```text
fazer 12 agachamentos
descansar 1 minuto
fazer 12 agachamentos
descansar 1 minuto
fazer 12 agachamentos
descansar 1 minuto
```

A gente escreve:

```text
REPITA 3 VEZES:
    fazer 12 agachamentos
    descansar 1 minuto
```

Bem melhor, né? E se o treino mudar para 4 séries, é só trocar um número.

Às vezes, a gente não sabe quantas vezes vai repetir, mas sabe **quando parar**. Lembra do brigadeiro?

```text
REPITA ATÉ a massa desgrudar do fundo da panela:
    mexer a massa
```

### O recuo (aquele espacinho à esquerda)

Reparou que algumas linhas começam mais para a direita? Esse espaço se chama **recuo** (ou **indentação**). Ele mostra **o que pertence a quê**:

```text
REPITA 3 VEZES:
    fazer 12 agachamentos      ← faz parte do REPITA
    descansar 1 minuto         ← faz parte do REPITA
alongar                        ← NÃO faz parte: só acontece no final, uma vez
```

Esse espaço muda tudo! No código de verdade é igualzinho, então vale se acostumar desde já.

---

## Exemplo pronto: um set de vôlei 🏐

Juntando tudo o que você aprendeu (sequência, decisão e repetição):

```text
entrar em quadra
REPITA ATÉ o set acabar:
    jogar o ponto
    SE a bola caiu dentro da quadra adversária:
        marcar 1 ponto para nós
        comemorar 🎉
    SENÃO:
        marcar 1 ponto para elas
cumprimentar o time adversário
```

Leia com calma, de cima para baixo, como se você fosse o Brigadeirobô. Repare:

- `entrar em quadra` acontece **uma vez**, no começo.
- Tudo que está recuado embaixo do `REPITA` acontece **a cada ponto**.
- `comemorar` só acontece **se** o ponto for nosso.
- `cumprimentar` acontece **uma vez**, no final.

??? example "Curiosidade: como isso fica em JavaScript?"
    Não precisa entender nada daqui, é só para você espiar o futuro. 👀 Veja como se parece com o que você acabou de escrever:

    ```javascript
    for (let serie = 1; serie <= 3; serie++) {
      fazerAgachamentos(12);
      descansar(1);
    }

    if (bolaCaiuNaQuadraAdversaria) {
      pontosNossos = pontosNossos + 1;
    } else {
      pontosDelas = pontosDelas + 1;
    }
    ```

    O `for` é o **REPITA**, o `if` é o **SE** e o `else` é o **SENÃO**. No Módulo 5, você vai escrever isso de verdade!

---

## ✏️ Mexe aí

Pegue o treino de agachamento lá de cima e, de cabeça ou no papel:

1. Mude para **4 séries de 15**.
2. Adicione uma decisão: **se** estiver muito cansada, descansar 2 minutos; **senão**, descansar 1 minuto.

??? question "Quer conferir?"
    ```text
    REPITA 4 VEZES:
        fazer 15 agachamentos
        SE estiver muito cansada:
            descansar 2 minutos
        SENÃO:
            descansar 1 minuto
    ```
    Repare que o **SE** está **dentro** do **REPITA** (tem recuo), e o que está dentro do **SE** tem **mais** recuo ainda. Ou seja: a decisão acontece **a cada série**.

---

## 🎯 Desafio 1.3

Crie a pasta `desafio-1.3` com um arquivo `treino.txt` dentro.

Escreva a **sua ficha de treino** como um algoritmo, com:

- Pelo menos **3 exercícios**
- Pelo menos um **REPITA**
- Pelo menos um **SE** (com ou sem **SENÃO**)
- **Recuo** certinho, mostrando o que pertence a quê

Depois, faça o ritual de entrega. 📦

!!! tip "Bônus (opcional)"
    Reescreva o seu algoritmo de unhas do desafio 1.1 usando **REPITA** (para cada unha…) e **SE** (se o esmalte borrar…). Vai ficar bem mais curto!

---

## ✅ Checklist

- [ ] Sei usar **SE** e **SENÃO** para tomar decisões
- [ ] Sei o que é uma **condição** (uma pergunta de sim ou não)
- [ ] Sei usar **REPITA** um número de vezes e **REPITA ATÉ** algo acontecer
- [ ] Entendi que o **recuo** mostra o que pertence a quê

---

## 🎉 Fim do Módulo 1!

Você acabou de aprender as **três ideias que existem em todo programa do mundo**:

- 📋 **Sequência**
- 🔀 **Decisão**
- 🔁 **Repetição**

Sério: do aplicativo do banco ao Instagram, é tudo isso, só que escrito numa língua que o computador entende. E aprender essa língua é o próximo passo.

No **Módulo 2**, você vai criar a sua **primeira página de internet**. 🌐
