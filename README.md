# 7DaysOfCodeAlura

<p>Desafio de lógica de programação com javascript proposto pela Alura para fixar os conhecimentos aprendidos nos cursos.
Além disso, também está servindo para aprender a utilizar Git e GitHub. Paralelamente, a depender do desafio, também está sendo empregado o uso de HTML e CSS para aprendizado. Alguns dos caminhos tomados aqui podem não ser os melhores e foram escolhidos para fins de aprendizado.</p>

## Dia 1
<p align="justify">Verificar a lógica de comparadores de um curto pedaço de código. Onde == verifica se dois elementos são semelhantes e retorna true (1 = '1', o número retorna como igual a um texto 1) e === verifica se são identicos, nesse exemplo anterior retornia falso, pois um deles é um texto e o outro não.
Para isso precisou apenas acertar os parâmetros do if, as variáveis já estavam dadas, e se utilizou o console.log para verificar se estava correto.</p>

## Dia 2
<p align="justify">Fazer com que uma página seja levemente dinâmica utilizando javascript para armazenar e reutilizar dados inseridos na página e ao preencher os dados (nome, idade) e apertar para enviar, aparece uma mensagem com esses dados. Também teve um desafio opcional que consistia em mais uma mensagem com pergunta sim ou não com mais uma resposta dinamica baseado no que o usuário inseriu na página.
Aqui criei várias const para utilizar os elementos do HTML com document.getElementbyId(), após isso é verificado se botão foi aperta com .onclick que iniciava a função que com .innerText escrevia o texto de acordo com o que foi inserido na página fazia o texto da pergunta opcional aparecer novamente com o .classList.remove (que remove um estilo no CSS que deixava o texto escondido). O desafio opcional foi feito de forma semelhante, porém com um botão para cada resposta (sim e não) e uma resposta personalizada para cada uma das escolhas.</p>
<p align="center">
<img width="420px" height="465.5px" src="https://user-images.githubusercontent.com/63385341/176802494-b9528d63-5e06-4ae4-93b3-df4a2b062963.gif">
</p>

## Dia 3
<p align="justify">Propor diferentes caminhos para o usuário com base em suas escolhas. O tema é programação, há duas opções inciais front-end e back-end e para cada uma delas há uma interação diferente: ao escolher front-end é mostrado as opções de React e Vue, já para o back-end, Java e C#. E no fim, após algumas outras perguntas o usuário pode preencher um campo dizendo quais tecnologias ele quer conhecer, ao preencher e adicionar a palavra escrita ela aparece embaixo. É possível escrever e adicionar infinitos termos (era uma das propostas do desafio), elas se somam conforme são adicionadas e mantém a formatação.
Para atingir o proposto (e de uma forma diferente da solução do dia anterior para fins de aprendizado) foi criada uma função em cada botão do html, sendo a mesma função para todos, porém com parâmetros diferentes. Se utilizando do for foi possível fazer essa verificação e transformar em números que servem de parâmetro para outra função cujo objetivo era fazer surgir os textos e opções novas baseados na escolha anterior do usuário. O funcionamento é semelhante a função anterior, mas contando apenas com if e else: o parâmetro é comparado com os índices de uma lista e com base nesses números o texto correto surge na tela (tem seu estilo display:none removido). Foi adicionado uma redundância aqui para que em caso de apertar os dois botões de uma mesma opção, o texto do apertado anteriormente desaperece, dando lugar ao correto. Por fim, utilizando .value para obter o que foi escrito no último campo de resposta e com .innerText para escrever em um paragráfo vazio, a lista com as tecnologias que se deseja conhecer é construída, somando a nova palavra com o que já foi escrito anteriormente.</p>
<p align="center">
<img width="420px" height ="465.5px" src="https://user-images.githubusercontent.com/63385341/176984767-9e92decf-5cd7-49ac-9307-a81dce40e8b7.gif">
</p>

## Dia 4
<p align="justify">O desafio do quarto dia consiste em criar um jogo de adivinhação contra a máquina. O usuário tem duas chances de adivinhar um número aleatório. Como há poucos textos nesse desafio, não foi necessário um html dedicado, sendo assim, em qualquer uma das páginas do desafio há um botão para iniciar o desafio. Surge um prompt com um texto indicando para inserir um número de 1 a 10. O valor digitado e enviado no prompt é comparado com uma variável que coleta o número gerado aleatóriamente por uma função e caso seja igual surge um alert com parabenizações. Em caso de erro, se inicia uma nova função com um novo prompt para a última tentativa, o código dessa segunda parte é bastante semelhante com o da primeira. Nos acertos e no último erro aparece o valor correto dentro da mensagem.</p>

## Dia 5
<p align="justify">O quinto dia consiste em um desafio de criar listas com categoria. Semelhante a uma lista de mercado. O usuário tem que escrever quais itens (alimentos) ele quer por em sua lista e em qual categoria esse alimento se encaixa. Esse desafio também incluiu HTML, a página perguntando se o usuário quer ou náo preencher a lista, ao clicar no botão de sim ele inicia o processo, mostrando o próximo conteúdo. Então se deve preencher o campo com o alimento desejado e apertar: aqui foi utilizado um addEventListener input para verificar quando uma tecla é solta, se for o Enter surge as possíveis categorias com um texto com a palavra escrita. O input é esvaziado para um visual melhor e, assim, valor dele é armazenado em uma variável para náo se perder para as futuras funções. Ao clicar em uma das categorias e aparece o botão de finalizar o processo, o usuário pode então acrescentar quantas vezes quiser e apertar o botão quando terminar. O valor armazenado na variável anteriormente é empurrado para uma lista previamente criada (e vazia no código), sendo essa associada, através de parametros na função do clique do botão, as categorias existentes. Aqui foram utilizadas várias listas e funções com parametros para deixar o código mais enxuto. Por fim, ao clicar no botão de finalizar, todo o conteúdo desaparece e surge a lista com todos os itens já categorizados, isso foi possível utilizando .innerHTML em 'p' que coloca o que está dentro das listas que foram preenchidas nas funções anteriores.</p>
<p align="cente">
<img width="420px" height="465.5px" src="https://user-images.githubusercontent.com/63385341/177432325-082d1b14-043f-4513-b6c8-3cd30dc50b1d.gif">
</p>