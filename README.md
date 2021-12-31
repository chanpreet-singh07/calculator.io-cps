let screen= document.getElementById(`screen`);
buttons = document.querySelectorAll(`button`);
let screenValue = '';
for(item of buttons){
    item.addEventListener(`click`, (e)=>{
        buttonText = e.target.innerText;


        console.log(`Button text is `, buttonText );
        if(buttonText=='X'){
            buttonText = '*';
            screenValue += buttonText; 
            screen.value = screenValue;
        }
        else if (buttonText =="C"){
            screenValue = ""; 
            screen.value = screenValue;
        }
        else if (buttonText =='='){
            screen.value = eval(screenValue);
        }
         else{
            screenValue += buttonText;
            screen.value = screenValue;
         } 


    })
}

.body{
    background-color: rgb(219, 206, 206);
    font-family: Impact, 'Arial Narrow Bold', sans-serif;
    font-size: 10px;
}
.container{
    text-align: center;
    margin-top:23px;
}
table{
    margin: auto;
}
.input{
    font-size: 34px;
    border: 5px solid rgb(0, 0, 0);
    border-radius: 18px;
}
.button{
    font-size: 37px;
    background-color: rgb(0, 107, 110);
    width: 104px;
    height: 66px;
    color: aliceblue;
    border-radius: 15px;
}
.text{
    color: rgb(0, 138, 143);
    font-size: 50px;
}
.calculator{
    background-color: white;
    display: inline-block;
    padding: 23px;
    border-radius: 50px;

}
button:hover {
    background-color: rgb(255, 194, 194);
}


<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <link rel="stylesheet" href="s21 ultra .css" />
    <title>calculator</title>
    <body>
      <div class="container">
        <h1 class="text">CALCULATOR</h1>

<div class="calculator">
        <input type="text" name="screen" id="screen" class="input" />

        <table >
          <tr>
            <td><button class="button">(</button></td>
            <td><button class="button">)</button></td>
            <td><button class="button">C</button></td>
            <td><button class="button">%</button></td>
          </tr>
          <tr>
            <td><button class="button">7</button></td>
            <td><button class="button">8</button></td>
            <td><button class="button">9</button></td>
            <td><button class="button">X</button></td>
          </tr>
          <tr>
            <td><button class="button">4</button></td>
            <td><button class="button">5</button></td>
            <td><button class="button">6</button></td>
            <td><button class="button">-</button></td>
          </tr>
          <tr>
            <td><button class="button">1</button></td>
            <td><button class="button">2</button></td>
            <td><button class="button">3</button></td>
            <td><button class="button">+</button></td>
          </tr>
          <tr>
            <td><button class="button">0</button></td>
            <td><button class="button">.</button></td>
            <td><button class="button">/</button></td>
            <td><button class="button">=</button></td>
          </tr>
        </table>
      </div>
      </div>
    </body>
    <script src="index.js"></script>
    <!-- <script src="index.js"></script> -->
  </head>
  <body class="body"></body>
</html>
