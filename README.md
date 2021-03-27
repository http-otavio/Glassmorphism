# Glassmorphism
Replicando conceitos do Glassmorphism/ efeito de vidro
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Efeito Vidro</title>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Poppins:300,400,500,600,700display=swap">
    <link rel="stylesheet" href="style.css">
    <style>
      *
{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;

}
body
{
display: flex;
justify-content: center;
align-items: center;
min-height: 100vh;
background-color: #161623;

}
body::before
{
content: '';
position: absolute;
top: 0;
left: 0;
width: 100%;
height: 100%;
background: linear-gradient(#f00, #f0f);
clip-path: circle(30% at right 70%);

}
body::after
{
content: '';
position: absolute;
top: 0;
left: 0;
width: 100%;
height: 100%;
background: linear-gradient(#2196f3, #e91e63);
clip-path: circle(20% at 10% 10%);
}
.container
{
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    max-width: 1200px;
    flex-wrap:wrap ;
    z-index: 1;

}
.container .cartão
{
    position: relative;
    width: 280px;
    height: 400px;
    margin: 30px;
    box-shadow: 20px 20px 50px rgba(0, 0, 0, 0.5);
    border-radius: 15px;
    background: rgba(255, 255, 255, 0.1);
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
    border-top: 1px solid rgba(255, 255, 255, 0.5);
    border-left: 1px solid rgba(255, 255, 255, 0.5);
    backdrop-filter: blur(5px);
}
 .container .cartão .content
{
    padding: 20px;
    text-align: center;
       transform: translateY(100px);
    opacity: 0;   
    transition: 0.5s;
}
   .container .cartão:hover .content
{
    transform: translateY(0px);
    opacity: 1; 
}   
 .container .cartão .content h2
 
{
   position: absolute;
   top: -106px;
   right: 10px;
   font-size: 8em;
   color: rgba(255, 255, 255, 0.05);
   pointer-events: none;
}

  .container .cartão .content h3
{
    font-size: 1.8em;
    color: #fff;
    z-index: 1;
}
.container .cartão .content p
{
  font-size: 1em;
  color: #fff;
  font-weight: 300;
}
.container .cartão .content a
{
    position: relative;
    display: inline-block;
    padding: 8px 20px;
    margin-top: 15px;
    background: #fff;
    color: #000;
    border-radius: 20px;
    text-decoration: none;
    font-weight: 500;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);


} 
    </style>
</head>
<body>
  <div class="container">
      <div class="cartão">
      <div class="content">
          <h2>01</h2>
          <h3>Cartão 1</h3>
          <p>Olá! Me chamo Otávio Messias e estou praticando CSS E HTML, irei replicar o efeito de vidro, conhecido como Glassmorphism, espero que dê certo!</p>
          <a href="https://www.youtube.com/watch?v=hv0rNxr1XXk">Mais Informações</a>
  </div>
  </div>
  
    <div class="cartão">
    <div class="content">
        <h2>02</h2>
        <h3>Cartão 2</h3>
        <p>Parece que estou conseguindo progresso no projeto, se tiver um 3º significa que eu consegui replicar o Glassmorphism da maneira que eu queria.</p>
        <a href="https://www.youtube.com/watch?v=hv0rNxr1XXk">Mais Informações</a>
</div>
</div>

    <div class="cartão">
    <div class="content">
        <h2>03</h2>
        <h3>Cartão 3</h3>
        <p>O projeto pode ser pequeno mas foi de grande ganho, é um efeito que me chamou bastante atenção, acredito que possa ser replicado de outras formas em difentes situações, espero que gostem!</p>
        <a href="https://www.youtube.com/watch?v=hv0rNxr1XXk">Mais Informações</a>
</div>
</div>
  </div>
</body>
</html>
