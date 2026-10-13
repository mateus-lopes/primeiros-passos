# 1.2 · O computador é bem literal

!!! abstract "Hoje você vai…"
    Conhecer o Brigadeirobô 🤖, entender por que o computador precisa de instruções **bem precisas** e caçar seus primeiros **bugs**. ⏱️ ~1h

---

## Explicação

Imagine que você comprou um robô de cozinha, o **Brigadeirobô**. Ele é ótimo, mas tem um jeitinho especial: ele faz **exatamente** o que está escrito. Nem mais, nem menos. Ele não tem bom senso e não "entende o que você quis dizer".

Você entrega para ele a receita de brigadeiro da lição passada. Olha o que acontece:

| Você escreveu | O Brigadeirobô fez |
|---|---|
| "Coloque o leite condensado numa panela" | Colocou a **lata fechada** dentro da panela. Ninguém mandou abrir! 🥫 |
| "Mexa sem parar até a massa desgrudar" | Mexeu… com o quê? Ele não tem colher na mão. Ficou parado. |
| "Espere a massa esfriar" | Esperou. Mas quanto tempo é "esfriar"? Ficou esperando até hoje. ⏳ |

Parece bobo, mas **o computador é exatamente assim**. Ele não sabe que a lata precisa ser aberta. Tudo o que para nós é "óbvio" precisa estar escrito.

Por isso, quem programa aprende a escrever instruções:

- **Precisas:** nada de "um pouco", "mais ou menos", "até ficar bom".
- **Completas:** nenhum passo pode ficar subentendido.
- **Na ordem certa:** o computador segue de cima para baixo, um passo de cada vez.

---

## Bugs 🐞

Quando um programa tem um erro, a gente chama de **bug** (que em inglês quer dizer "inseto").

!!! example "Curiosidade"
    Em 1947, uns cientistas não entendiam por que o computador deles estava dando problema. Foram procurar e acharam… uma **mariposa de verdade** presa dentro da máquina! Eles colaram o inseto no caderno de anotações, e o nome pegou. 🦋

Os bugs mais comuns são os mesmos de uma receita mal escrita:

| Tipo de bug | Exemplo na receita |
|---|---|
| **Instrução vaga** | "Coloque um pouco de açúcar" (quanto?) |
| **Passo faltando** | Esqueceu de dizer para abrir a lata |
| **Ordem trocada** | "Passe no granulado" antes de "faça as bolinhas" |

!!! tip "Bug não é vergonha"
    Todo programador escreve bugs, **todo dia**. A diferença de quem tem experiência é só que ela já está acostumada a procurar e consertar. Encontrar um bug é parte do trabalho, não um fracasso.

---

## Exemplo pronto: consertando para o robô

Instrução vaga:

> ❌ "Mexa até ficar no ponto."

Instrução que o Brigadeirobô entende:

> ✅ "Pegue a colher de pau. Mexa a massa sem parar. Quando der para ver o fundo da panela ao passar a colher, pare de mexer."

Ficou mais comprida, né? Tudo bem! Para o computador, **claro é melhor que curto**.

---

## ✏️ Mexe aí

Reescreva estas instruções (de cabeça ou no papel) para que o Brigadeirobô consiga seguir sem dúvidas:

1. "Unte as mãos."
2. "Coloque em forminhas."

??? question "Quer ver um jeito de escrever?"
    1. "Pegue a manteiga. Passe uma pontinha de manteiga na palma das duas mãos."
    2. "Pegue uma forminha de papel. Coloque um brigadeiro dentro dela. Repita até acabarem os brigadeiros."

    Repare que, na segunda, apareceu um **repita**. Guarde isso: é o assunto da próxima lição! 😉

---

## 🎯 Desafio 1.2

Esta é a receita de **vitamina pós-treino** que alguém escreveu para o Brigadeirobô. Ela está **cheia de bugs**:

> **Vitamina de banana com aveia**
>
> 1. Ligue o liquidificador.
> 2. Coloque a banana no liquidificador.
> 3. Coloque um pouco de leite.
> 4. Coloque a aveia.
> 5. Sirva no copo.
> 6. Tampe o liquidificador.

Crie a pasta `desafio-1.2` com um arquivo `vitamina.txt` dentro e escreva:

1. **Os bugs que você encontrou** (tem pelo menos 5, mas se achar 3 já está ótimo!). Para cada um, diga o tipo: instrução vaga, passo faltando ou ordem trocada.
2. **A receita corrigida**, do jeito que o Brigadeirobô consegue seguir.

Depois, faça o ritual de entrega. 📦

!!! tip "Bônus (opcional)"
    Volte no seu `unha.txt` do desafio 1.1 e leia como se você fosse o Brigadeirobô. Tem algum bug? Se tiver, conserte e entregue de novo!

---

## ✅ Checklist

- [ ] Entendi que o computador faz exatamente o que está escrito
- [ ] Sei que instruções precisam ser precisas, completas e na ordem certa
- [ ] Sei o que é um **bug**
- [ ] Conheço três tipos de bug: instrução vaga, passo faltando e ordem trocada
