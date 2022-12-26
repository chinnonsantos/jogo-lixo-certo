# Jogo Lixo Certo - APS 4º Semestre (2013) de Ciência da Computação da UNIP

**Jogo 2D feito em Java 8 utilizando a biblioteca Swing para interface gráfica**, para trabalho acadêmico APS (Atividade Prática Supervisionada) do 4º Semestre da graduação em Ciência da Computação (CC) - UNIP (Universidade Paulista) - 17/11/2013 🎮

> **“DESENVOLVIMENTO DE UM JOGO COM UTILIZAÇÃO DE INTERFACE GRÁFICA”**

## Sobre o jogo

O Jogo é bem simples, com intuito somente de testar conhecimentos adquiridos no semestre estudado, foram dedicadas poucas horas de programação, porém o resultado e satisfatório devido a quantidade mínima de recursos e tecnologia necessárias para desenvolvimento.

Ah!, sobre o personagem, foi uma homenagem ao um amigo de turma que se chama **Rodrigo Marinho**, que sempre copia todos os meus códigos de trabalho, dessa vez já vou facilitar para ele deixando o personagem com seu nome. Hahaha

## Alunos

Chinnon Santos – RA: B5526C-7.
Leonardo Felipe da Silva - RA: B5680D-5.
Lucas Aleixo Mendonça - RA: B25444-0.
Magdiel Alves de Oliveira - RA: B4707G-0.

## Código Fonte & Material Acadêmico

Foi disponibilizado nesse repositório o código fonte original do jogo criado em 11/2013, sem as configurações necessárias para que seja possível o re-build do projeto.

Naquela época o objetivo não era compartilhar o código fonte na internet (eu também não tinha conhecimento de GIT), mas devido ao sucesso que o vídeo do jogo teve no YouTube com outros alunos de CC da UNIP, resolvi compartilhar o `.JAR` por link e hoje (quase 10 anos depois), estou disponibilizando o código fonte completo (.class, imgs e áudios) no GitHub, incluindo o material acadêmico em PDF.

O código fonte pode ser encontrado no diretório [`source/*`](/source/) do repositório.

O material acadêmico pode ser encontrado no diretório [`docs/APS-4-SEMESTRE.pdf`](/docs/APS-4-SEMESTRE.pdf) do repositório.

> Originalmente esse projeto foi construído usando a IDE Eclipse, hoje não utilizo mais essa IDE, e assim que possível irei refatorar o projeto para ser possível executar o build pela IDE IntelliJ.

---

## Regras do jogo (conceitos gerais)

- Acerta o número máximo de lixo exatamente na boca da lixeira correta de
acordo com o lixo que aparecer na tela no **prazo de 1 (um) minuto**.
- O acerto do lixo corretamente na boca da lixeira e o tipo do lixo ser
correspondente ao tipo da lixeira, **soma 10 (dez) pontos** à sua pontuação total.
- O acerto do lixo corretamente na boca da lixeira, mas e o tipo do lixo _NÃO_ ser
correspondente ao tipo da lixeira, **subtrai 5 (cinco) pontos** à sua pontuação
total.
- O não acerto do lixo corretamente na boca da lixeira, **subtrai 10 (dez) pontos** à sua pontuação total.
- O resultado da pontuação total no termino de 1 minuto for positiva (maior que zero), você recebe os parabéns e cumpre o objetivo do jogo.
- O resultado da pontuação total no termino de 1 minuto for negativa (menor ou
igual a zero), você recebe uma mensagem de fracasso.
- A qualquer momento do jogo é possível voltar ao menu inicial e encerrar a
partida atual.
- A quantidade de lixos exibidas são ilimitadas.
- O aparecimento de tipos de lixo e definida de forma aleatória pelo sistema do
jogo, podendo ocorrer repetições seguidas do mesmo tipo de lixo, elevando o
nível de dificuldade.
- Após o termino dos 60 segundos não é possível mais jogar lixos nas lixeiras
sendo que o mesmo não é mais exibido.
- Você pode jogar quantas vezes quiser, não há limites de jogada, também
poderá abandonar a partida quantas vezes quiser, não há limitações para
abandono de jogo.

## Plano de desenvolvimento do jogo

O plano de jogo foi elaborado em 4 fases, tendo como base a gerência de
desenvolvimentos de grandes jogos do mercado atual.

### 1º Fase – Roteiro

Cada vez mais se assemelham a roteiros de filmes. Este é um item
fundamental para o processo de criação e será o elemento crucial para
convencer os investidores da potencialidade do nosso jogo. É nesse item que o
jogo deve mostrar seu diferencial em relação aos outros. Chamam-se aos
roteiros de jogos de roteiros interativos, pois diferentemente que os roteiros de
filmes, devem ter espaço para interferência do usuário no desencadeamento da
história.

### 2º Fase - Game Design

Entende-se por game design a conceituação artística do jogo. Hoje em dia,
dada a complexidade das histórias e dos cenários elaborados é importante que
esta parte do documento seja escrita por um artista. Dentro deste item deverão
ser expostos quais as principais características dos cenários, esboços de
personagens, descrição das texturas fundamentais, mapas e descrições dos
combates. (também denominado de level design).

### 3º Fase - Game Play

Nesta parte do documento deve descrever-se como será a jogabilidade.
PRINCIPAL ETAPA DE UM JOGO, Por jogabilidade entendem-se as regras do
jogo e o balanceamento das regras (game balancing). Nesta descrição deve
ficar claro que o jogo é divertido e irá proporcionar desafios interessantes. Esta
parte do documento é muito importante para guiar os programadores
principalmente na etapa de scripting. Uma mal elaboração dessa etapa pode
influência seriamente em um mal desenvolvimento (bugs) e atrasos em todo o
projeto.

### 4º Fase - Interface Gráfica

Pode-se dividir a interface em in game e out game. A primeira consiste na
instrumentação disponível durante o jogo e é responsável pela entrada de
dados do jogador para a aplicação. A interface out game é a forma de
apresentar a introdução do jogo, sua configuração, instruções, carregar o jogo,
entre outras operações de suporte. Costuma-se dizer que a melhor interface é
aquela que passa despercebida para o jogador, permitindo que o mesmo possa
focar-se no desenrolar da história e das ações. Resumindo, o in game é a parte
do jogo que se é jogável, a parte onde você possui um tempo para atingir o
objetivo que é fazer pontuação acertando corretamente o tipo de lixo em sua
lixeira, já o out game é a nossa abertura do Marinho correndo e a tela onde
você escolhe jogar ou sair do jogo.
