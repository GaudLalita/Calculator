# Calculator
its a sample calculator that perform simple calculations such as addition, substraction ,multiplication and division
here is the source code for this calculator
<html>
    <head>
        <title>calculator</title>
        <style>
*{
margin:0;
padding:0;
font-family:roboto,arial;
box-sizing:border-box;
}

.container{
width:100%;
height:100%;
background-color:rgb(227, 227, 223);
display:flex;
align-items:center;
justify-content:center;


}
.calculator{
    background-color:darkslategray;
   
    padding:10px;
    border-radius:8px;
    

}
.calculator form input{
    border:0;
    outline:0;
    width:60px;
    height:60px;
    border-radius:8px;
    box-shadow:-8px -8px 15px rgba(255, 255, 255, 0.1), 5px 5px 15px rgba(0,0,0,0.2);
    color:aliceblue;
    background:transparent;
    font-size:20px;
    cursor:pointer;
    margin:10px;
}
 form .display{
    display:flex;
    justify-content:flex-end;
    margin:20px 0;   
 }

 form .display input{
    text-align:right;
    flex:1;
    font-size:45px;
    box-shadow:none; 
 }

form input.equal{
    width:145px;
}

 form input.cal{
    color:blanchedalmond;
 }
  form input.bracks{
    color:rgba(0, 255, 255, 0.735);
  }

        </style>
    </head>
    <body>
<div class="container">
    <div class="calculator">
        <form>
            <div class="display">
                <input  class="enter" type="text" name="screen">
            </div>
            <div>
                <input type="button" value="AC" onclick="screen.value='' " class="cal">
                <input type="button" value="DEL" onclick="screen.value=screen.value.slice(0,-1)" class="cal">
                <input type="button" value="." onclick="screen.value+='.' " class="cal">
                <input type="button" value="/" onclick="screen.value+='/' " class="cal">
            </div>
            <div>
                <input type="button" value="(" onclick="screen.value +='('" class="bracks">
                <input type="button" value=")" onclick="screen.value +=')'" class="bracks">
                <input type="button" value="{" onclick="screen.value +='{'" class="bracks">
                <input type="button" value="}" onclick="screen.value +='}'" class="bracks">
            </div>
            <div>
                <input type="button" value="7" onclick="screen.value +='7'" >
                <input type="button" value="8" onclick="screen.value +='8'" >
                <input type="button" value="9" onclick="screen.value +='9'" >
                <input type="button" value="*" onclick="screen.value +='*'" class="cal">
            </div>
            <div>
                <input type="button" value="4" onclick="screen.value +='4'" >
                <input type="button" value="5" onclick="screen.value +='5'" >
                <input type="button" value="6" onclick="screen.value +='6'" >
                <input type="button" value="+" onclick="screen.value +='+'" class="cal">
            </div>
            <div>
                <input type="button" value="1" onclick="screen.value +='1'" >
                <input type="button" value="2" onclick="screen.value +='2'" >
                <input type="button" value="3" onclick="screen.value +='3'" >
                <input type="button" value="-" onclick="screen.value +='-'" class="cal">
            </div>

            
            
            <div>
                <input type="button" value="00" onclick="screen.value+='00'" >
                <input type="button" value="0" onclick="screen.value+='0'" >
                <input type="button" value="=" onclick="screen.value=eval(screen.value)" class="equal cal">
            </div>
        </form>
    </div>
</div>


    </body>
</html>
