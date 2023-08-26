# just to practice computational logic exercises, many (all) times using javascript.

    <!-- #1 
    
    Crie um HTML com um parágrafo <p> vazio e um botão <button> com o texto "Alterar Texto".
    Use o JavaScript para selecionar o parágrafo e o botão usando document.querySelector.
    Adicione um ouvinte de evento ao botão para que, quando clicado, o texto do parágrafo seja alterado para "Novo texto!". -->


    #2
    
    <!-- Crie uma lista não ordenada <ul> com alguns itens de lista <li>. -->
     
                Mexer no HTML. Tags UL e LI. Fácil. 

    <!-- Adicione classes aos itens da lista. -->

                Mexer em CSS. Criar classe para cada um dos itens da lista. Uma classe em comum vai facilicar sua vida. 

    <!-- Crie dois botões, um para adicionar uma classe e outro para remover uma classe. -->

                Mexer no HTML e CSS. Tag BUTTON. Criar duas, um para adicionar e outro para remover. É bom criar de uma vez uma ID para cada um, já que lendo o pedido todo, você sabe que irá precisar utilizar estes botões de algum modo. 

    Use o JavaScript para selecionar os botões e adicionar ou remover uma classe de um item da lista quando os botões forem clicados.

                Pedindo várias coisas. Na verdade três. Uma é selecionar os botões e a classe criada (CRIANDO A VARIAVEL), então outra é criar a função que realizará a troca de classes e, enfim, a terceira, essa função irá acontecer quando os botões forem clicados. 

                Então, primeiro, selecionar os botões e classes: JS. Você criou classes, então vai nomear sua variável e juntar ela com o querySelector. Você criou IDs, então também vai juntar elas com .getElementByID. 

                Segundo e teceiro: crie a função que irá construir a mágica e o evento que permitirá ela acontecer. Isso poupará dedos e fará tudo dentro de um só lugar. 
                    
                    Primeiro: chame sua variável E adiciona o evento nela que irá fazer ela funcionar quando algo especifico acontecer. Termine essa linha chamando a função (uma função genérica, apenas para indicar para a máquina que terá de ler uma função) e abra seu escopo.

                    addButon.addEventListener('click', function() {

                    Segundo: chamar sua varável, de novo. desta vez, a variavel que engloba os itens da lista. Adicione a funcionalidade que .forEach, que fará que cada item dentro daquela variavel seja percorrido (cada uma das classes nomeadas 'item', lembra?) e ainda defina um acontecimento a isso através do (), alimentando com o arrow ao dizer que para cada ITEM ele vai fazer ALGUMA COISA.

                    itensList.forEach(item => {

                    Terceiro: está dizendo que para CADA ITEM, ele vai fazer alguma coisa. E essa coisa é: utilizando a funcionalidade .classList (para deixar claro que se trata de uma lista de classes), ele vai .add (adicionar) algo (), no caso, 'destaque'.

                    item.classList.add('destaque');