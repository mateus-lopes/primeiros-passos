# 0.1 · Sessão 0: arrumando o computador

!!! abstract "Hoje você vai…"
    Instalar os programas da trilha, criar sua conta no GitHub e fazer a sua **primeira entrega**. ⏱️ ~2h, divididas em **2 partes** (uma por dia).

Esta lição é feita **junto com quem está te acompanhando**. Você mexe no computador, a outra pessoa só ajuda. Não precisa entender tudo hoje, só deixar pronto. 😉

---

## Parte 1 · Instalando as ferramentas (~1h)

### 1. VS Code: o seu caderno de código

O **VS Code** é o programa onde você vai escrever código. Pense nele como um bloco de notas turbinado: ele colore o código, avisa quando algo parece errado e organiza seus arquivos.

1. Acesse **[code.visualstudio.com](https://code.visualstudio.com/)** e clique no botão grande de download.
2. Instale:

=== "Windows"

    Abra o arquivo baixado e vá clicando em **Next** (Avançar). Numa das telas aparecem caixinhas de opções. Marque estas duas:

    - **Adicionar a ação "Abrir com Code" ao menu de contexto de arquivo**
    - **Adicionar a ação "Abrir com Code" ao menu de contexto de diretório**

    Elas deixam você abrir arquivos e pastas no VS Code com o botão direito do mouse. Bem prático!

=== "Mac"

    Abra o arquivo baixado e arraste o **Visual Studio Code** para a pasta **Aplicativos**.

3. Abra o VS Code. Se ele oferecer instalar o **pacote de idioma em português**, aceite e reinicie quando ele pedir.

!!! tip "Não apareceu a oferta de português?"
    Clique no ícone de quadradinhos na barra da esquerda (**Extensões**), pesquise por `Portuguese (Brazil) Language Pack` e instale o da **Microsoft**.

### 2. Desligando a IA do VS Code

O VS Code vem com um assistente de inteligência artificial que tenta escrever código por você. Nesta trilha, **a gente desliga isso**. Na lição 0.2 eu explico direitinho o porquê, mas o resumo é: quem tem que levantar o peso é você, senão o músculo não cresce. 💪

1. Abra as configurações:

    === "Windows"

        ++ctrl+comma++

    === "Mac"

        ++cmd+comma++

2. Na barra de busca que aparece no topo, digite: `disable ai features`
3. Marque a caixinha da opção **Chat: Disable AI Features**.

Pronto! Pode fechar a aba de configurações.

### 3. Git: o seu histórico de versões

O **Git** é um programa que guarda o histórico de tudo que você faz no código, tipo as fotos de "antes e depois" de um procedimento no salão. Com ele, você também consegue **entregar seus desafios**.

=== "Windows"

    1. Acesse **[git-scm.com](https://git-scm.com/)** e baixe a versão para Windows.
    2. Abra o instalador e vá clicando em **Next**. São muitas telas, mas as opções que já vêm marcadas estão ótimas.
    3. Só numa tela vale mudar: quando perguntar o **editor padrão** (*default editor*), escolha **Use Visual Studio Code as Git's default editor**.

=== "Mac"

    1. Abra o app **Terminal** (procure por "Terminal" no Spotlight, com ++cmd+space++).
    2. Digite `git --version` e aperte ++enter++.
    3. Se aparecer uma janela oferecendo instalar as **ferramentas de linha de comando**, clique em **Instalar** e espere terminar.

### 4. Conta no GitHub: o lugar onde seus projetos moram

O **GitHub** é um site onde você guarda seus projetos na internet. É lá que vão ficar os seus desafios e, mais pra frente, a sua página publicada.

1. Acesse **[github.com/signup](https://github.com/signup)** e crie sua conta.
2. Siga as instruções e confirme o e-mail.

!!! warning "Escolha o nome de usuário com carinho"
    Seu nome de usuário vai aparecer **no link da sua página** lá no Módulo 4, tipo `seunome.github.io`. Prefira algo simples e que você não vai ter vergonha de mandar para ninguém. 😅

🎉 **Fim da Parte 1!** Pode descansar. A Parte 2 fica para o próximo dia.

---

## Parte 2 · Sua primeira entrega (~1h)

### 5. Apresentando-se ao Git

O Git precisa saber quem você é, para "assinar" o seu trabalho. A gente faz isso pelo **terminal**, que é um jeito de conversar com o computador escrevendo em vez de clicar.

1. No VS Code, abra o terminal pelo menu **Terminal → Novo Terminal**. Vai aparecer uma área na parte de baixo da tela.
2. Digite os dois comandos abaixo, um de cada vez, apertando ++enter++ depois de cada um. Troque o que está entre aspas pelos **seus** dados (use o mesmo e-mail do GitHub):

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@exemplo.com"
```

Se nada aparecer depois de apertar ++enter++, **deu certo**. No terminal, silêncio costuma ser bom sinal. 😄

### 6. Criando a sua caixinha de desafios

Agora você vai criar um **repositório**, que é só um nome chique para "pasta de projeto que o Git acompanha". Ele vai se chamar `desafios`.

1. No GitHub, clique no **+** lá em cima, à direita, e depois em **New repository**.
2. Preencha assim:
    - **Repository name:** `desafios`
    - Marque **Private**, assim só você (e quem você convidar) vê.
    - Ligue a opção **Add README**.
3. Clique em **Create repository**.
4. Para que seus desafios possam ser corrigidos, convide quem está te acompanhando: vá em **Settings → Collaborators → Add people**.

### 7. Trazendo a caixinha para o seu computador

1. Crie uma pasta chamada `Programacao` dentro de **Documentos**. É lá que vão morar todos os seus projetos.
2. No GitHub, na página do repositório `desafios`, clique no botão verde **Code** e copie o link que aparece (começa com `https://`).
3. No VS Code, aperte ++ctrl+shift+p++ (no Mac, ++cmd+shift+p++), digite `clonar` e escolha **Git: Clonar**.
4. Cole o link e aperte ++enter++. Ele vai perguntar onde salvar: escolha a pasta `Programacao`.
5. Se aparecer uma janela pedindo para entrar no GitHub, entre com a sua conta e autorize.
6. Quando ele perguntar se quer abrir o repositório, clique em **Abrir**.

Agora a pasta `desafios` está aberta no VS Code, na barra da esquerda (o **Explorador**). 🎉

### 8. O primeiro desafio

1. No Explorador, clique com o botão direito numa área vazia e escolha **Nova Pasta**. Dê o nome `desafio-0.1`.
2. Clique com o botão direito na pasta `desafio-0.1` e escolha **Novo Arquivo**. Dê o nome `sobre-mim.txt`.
3. Escreva no arquivo **3 coisas que você ama**. Pode ser qualquer coisa!
4. Salve com ++ctrl+s++ (no Mac, ++cmd+s++).

Aproveite e crie mais um arquivo, agora **fora** de qualquer pasta, chamado `DUVIDAS.md`. Escreva só isto dentro dele e salve:

```markdown
# Dúvidas para perguntar
```

Ele vai ser o seu caderninho de dúvidas. Na próxima lição você vai entender como usar.

### 9. O ritual de entrega 📦

Entregar um desafio é parecido com fazer uma compra online:

| Passo | Na loja | No Git |
|---|---|---|
| 1 | Colocar os produtos no carrinho | `git add .` |
| 2 | Finalizar o pedido, com uma descrição | `git commit -m "descrição"` |
| 3 | Enviar o pedido | `git push` |

No terminal do VS Code, digite um comando de cada vez:

```bash
git add .
git commit -m "Desafio 0.1: sobre mim"
git push
```

!!! note "Atenção ao ponto"
    O `git add .` tem um **ponto** no final, separado por um espaço. Ele quer dizer "tudo o que mudou".

Se for a primeira vez, pode abrir uma janela do navegador pedindo para entrar no GitHub. É só entrar e autorizar.

Agora abra o seu repositório `desafios` no GitHub e atualize a página. Seus arquivos estão lá! **Essa foi a sua primeira entrega.** 🥳

---

## ✅ Checklist

- [ ] VS Code instalado, em português e com a IA desligada
- [ ] Git instalado e sabendo quem eu sou
- [ ] Conta no GitHub criada
- [ ] Repositório `desafios` criado e no meu computador
- [ ] Primeira entrega feita com `add`, `commit` e `push`

!!! tip "Não precisa decorar nada"
    Os comandos do ritual de entrega estão sempre aqui e na [lição 0.2](aula02-como-usar-a-trilha.md). Com o tempo, eles vão ficar automáticos, igual a uma sequência de treino que você já faz sem pensar.
