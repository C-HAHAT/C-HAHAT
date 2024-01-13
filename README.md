<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Change mode</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA==" crossorigin="anonymous" referrerpolicy="no-referrer" />
</head>
<body>
    <button id="btn">Change mode click me!</button>
</body>
<script src="javasript.js">
  let newbtn = document.querySelector("#btn");

document.querySelector("body").style.textAlign = "center";
document.querySelector("body").style.marginTop = "20%" ;
document.querySelector("button").style.fontSize = "40px" ;
let currMode  = "light";

newbtn.addEventListener("click",() => {
    if(currMode === "light"){
        currMode = "dark";
        document.querySelector("body").style.backgroundColor = "black";
        document.querySelector("button").style.backgroundColor = "red";
    }else{
        currMode = "light";
        document.querySelector("body").style.backgroundColor = "white";
        document.querySelector("button").style.backgroundColor = "white";
    }

    console.log(currMode);
})
</script>
</html>
