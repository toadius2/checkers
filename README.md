# checkers
checkers board task for driven delivery
<html>
<body>
    <script type = "text/javascript">
      
  //Game constructor 
    function Game(canvas) {
    this._boardRect = null;
    this._canvas = canvas;
    this._ctx = canvas.getContext("2d");
    this._boardModel = new BoardModel();
    this._boardRenderer = new BoardRenderer(this._ctx, this._boardModel);
    this.handleResize();
}
_p = Game.prototype;

//Resizing Board
var board = document.getElementById('BoardModel');
const renderBoard = () =>{
  for (var i = 0; i < 8; ++i){
    var row = document.createElement('div')
    row.className = 'row'
    row.style.flexDirection = i % 2 === 0 ? '' : 'row-reverse'; 
    for (var j = 0; j < 8; ++j){
      var square = document.createElement('div')
      square.className = 'square'
      square.style.backgroundColor = j % 2 === 0 ? 'white' : 'black'
      row.appendChild(square)
    }
    board.appendChild(row)
  }   
  }
 </script>
 </body>
 </html>
  
