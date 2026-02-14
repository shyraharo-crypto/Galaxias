# Galaxia<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Galaxia</title>
<style>
body{margin:0;background:black;overflow:hidden;}
.star{
position:absolute;
width:3px;
height:3px;
background:white;
border-radius:50%;
animation:caer linear infinite;
}
@keyframes caer{
from{transform:translateY(-10vh);}
to{transform:translateY(110vh);}
}
</style>
</head>
<body>
<script>
for(let i=0;i<150;i++){
let s=document.createElement("div");
s.className="star";
s.style.left=Math.random()*100+"vw";
s.style.animationDuration=(Math.random()*4+2)+"s";
document.body.appendChild(s);
}
</script>
</body>
</html>
