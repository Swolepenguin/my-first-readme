# my-first-readme
repo explaining readme
```javascript
const handleWin = (letter) => {
  gameIsLive = false;
  if (letter === "x") {
    statusDiv.innerHTML = `${letterToSymbol(letter)} has won!`;
  } else {
    statusDiv.innerHTML = `<span>${letterToSymbol(letter)} has won!</span>`;
  }
};
```

```CSS 
.grid {
    background-color: salmon;
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(3, 1fr);
    gap: 15px;
    margin-top: 50px;
}
```

```HTML 
<div class="grid">
    <div class="box" id="box-1"></div>
    <div class="box" id="box-2"></div>
    <div class="box" id="box-3"></div>
    <div class="box" id="box-4"></div>
    <div class="box" id="box-5"></div>
    <div class="box" id="box-6"></div>
    <div class="box" id="box-7"></div>
    <div class="box" id="box-8"></div>
    <div class="box" id="box-9"></div>
</div>
```
// this is the tic-tac-toe readme continuation

```Git opening process 
Go to Github `fork` the repo
then `clone` the repo
open up your command line or git bash and `Git clone` the copied link

```
//heres my javaScript
```javaScript 
const gameStatus = document.querySelector('gamestatus')

const player1 = 'x'
const player2 = 'o'
let gameState = ['','','','','','','','','']
let xO = ['X','O','X','O','X','O','X','O','X']
let currentPlayer = 'x'
let b1 = document.getElementById('b1')
let b2 = document.getElementById('b2')
let b3 = document.getElementById('b3')
let b4 = document.getElementById('b4')
let b5 = document.getElementById('b5')
let b6 = document.getElementById('b6')
let b7 = document.getElementById('b7')
let b8 = document.getElementById('b8')
let b9 = document.getElementById('b9')

function changeCurrentPlayer(){
    if (currentPlayer===player1){
        currentPlayer=player2
    }
    else  {
        currentPlayer=player1
    }
};

b1.addEventListener('click',function(){
    b1.textContent= currentPlayer 
    changeCurrentPlayer()
    checkingForWinner()
})

b2.addEventListener('click',function(){
    b2.textContent= currentPlayer 
    changeCurrentPlayer()
    checkingForWinner()
})
b3.addEventListener('click',function(){
    b3.textContent= currentPlayer 
    changeCurrentPlayer()
    checkingForWinner()
})
b4.addEventListener('click',function(){
    b4.textContent= currentPlayer 
    changeCurrentPlayer()
    checkingForWinner()
})
b5.addEventListener('click',function(){
    b5.textContent= currentPlayer 
    changeCurrentPlayer()
    checkingForWinner()
})
b6.addEventListener('click',function(){
    b6.textContent= currentPlayer 
    changeCurrentPlayer()
    checkingForWinner()
})
b7.addEventListener('click',function(){
    b7.textContent= currentPlayer 
    changeCurrentPlayer()
    checkingForWinner()
})
b8.addEventListener('click',function(){
    b8.textContent= currentPlayer 
    changeCurrentPlayer()
    checkingForWinner()
})

b9.addEventListener('click',function(){
    b9.textContent= currentPlayer 
    changeCurrentPlayer()
    checkingForWinner()
})








    
function rowOneForWinner(gamestate,player1){
    if(b1.textContent===player1 && b2.textContent===player1 && b3.textContent===player1)
    {console.log('winner is player1')}
    else if (b1.textContent===player2 && b2.textContent===player2 && b3.textContent===player2)
    {console.log( 'winner is player2')} 
};

function rowTwoForWinner(gamestate,player1){
    if(b4.textContent===player1 && b5.textContent===player1 && b6.textContent===player1)
    {console.log('winner is player1')}
    else if(b4.textContent===player2 && b5.textContent===player2 && b6.textContent===player2)
    {console.log( 'winner is player2')} 
};
function rowThreeForWinner(gamestate,player1){
    if(b7.textContent===player1 && b8.textContent===player1 && b9.textContent===player1)
    {console.log('winner is player1')}
    else if(b7.textContent===player2 && b8.textContent===player2 && b9.textContent===player2)
    {console.log( 'winner is player2')} 
};
function columnOneForWinner(gamestate,player1){
    if(b1.textContent===player1 && b4.textContent===player1 && b7.textContent===player1)
    {console.log('winner is player1')}
    else if(b1.textContent===player2 && b4.textContent===player2 && b7.textContent===player2)
    {console.log( 'winner is player2')} 
};
function columnTwoForWinner(gamestate,player1){
    if(b2.textContent===player1 && b5.textContent==player1 && b8.textContent===player1)
    {console.log('winner is player1')}
    else if(b2.textContent===player2 && b5.textContent===player2 && b8.textContent===player2)
    {console.log( 'winner is player2')} 
};
function columnThreeForWinner(gamestate,player1){
    if(b3.textContent===player1 && b6.textContent===player1 && b9.textContent===player1)
    {console.log('winner is player1')}
    else if(b3.textContent===player2 && b6.textContent===player2 && b9.textContent===player2)
    {console.log( 'winner is player2')} 
};
function diagonalOneForWinner(gamestate,player1){
    if(b1.textContent===player1 && b5.textContent===player1 && b9.textContent===player1)
    {console.log('winner is player1')}
    else if(b1.textContent===player2 && b5.textContent===player2 && b9.textContent===player2)
    {console.log( 'winner is player2')} 
};
function diagonalTwoForWinner(gamestate,player1){
    if(b3.textContent===player1 && b5.textContent===player1 && b7.textContent===player1)
    {console.log('winner is player1')}
    else if(b3.textContent===player2 && b5.textContent===player2 && b7.textContent===player2)
    {console.log( 'winner is player2')} 
};

function checkingForWinner(){
    rowOneForWinner()
    rowTwoForWinner()
    rowThreeForWinner()
    columnOneForWinner()
    columnTwoForWinner()
    columnThreeForWinner()
    diagonalOneForWinner()
    diagonalTwoForWinner()
};
console.log(checkingForWinner)
```
//heres my html
```<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Hello Front-End</title>
  <link rel="stylesheet" type="text/css" href="css/style.css">
</head>
<body>
  <h1>Tic Tac Toe</h1>
  <div class="grid">
    <div class="row">
      <div class="box" id="b1"></div>
      <div class="box" id="b2"></div>
      <div class="box" id="b3"></div>
    </div>
    <div class="row">
      <div class="box" id="b4"></div>
      <div class="box" id="b5"></div>
      <div class="box" id="b6"></div>
    </div>
    <div class="row">
      <div class="box" id="b7"></div>
      <div class="box" id="b8"></div>
      <div class="box" id="b9"></div>
    </div>
  </div>

  <script type="text/javascript" src="js/app.js"></script>
</body>
</html>
```
this is my css
```h1 {
  color: purple;
}
.grid{
  display: table;
  border-spacing: 5px;
}
.row{
  display:table-row;
  
}
.box{
  width: 50px;
    height: 50px;
    background: rgb(100, 168, 134);
    display: table-cell;
}
```