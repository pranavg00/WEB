<!DOCTYPE html>
<html lang="en" style="background-color: rgb(31, 31, 31); color: whitesmoke;">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>My Shoes</title>
</head>
  <style>
    *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body {
    min-height: 100vh;
    font-family: "poppins", sans-serif;
    align-items: center;
    justify-content: center;
    display: flex;
    perspective: 1000px;
}
.logo{
    position:fixed;
    top: 0;
    width: 100%;
}
.logo img{
    margin-left: auto;
    margin-right: auto;
    width: 10rem;
    display: block; 
}
.container {
    width: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: rgb(114, 112, 111);
    border-bottom-right-radius: 50%;
    border-top-right-radius: 50%;
}
.card {
    transform-style: preserve-3d;
    min-height: 85vh;
    width: 25rem;
    padding: 0rem 5rem;
    box-shadow: 0 20px 20px rgba(255, 255, 255, 0.2), 0px 0px 50px 20px rgba(255, 255, 255, 0.2);
    border-radius: 10px;
    background-color: rgb(93, 110, 124);
}
.shoe {
    min-height: 35vh;
    display: flex;
    align-items: center;
    justify-content: center;
}
.shoe img {
    width: 15rem; 
    z-index: 2;
    transition: all 0.75s ease-out;
}
.circle {
    width: 13rem;
    height: 13rem;
    background: linear-gradient(
        to right,
        rgba(82, 88, 98, 0.75),
        rgba(248, 248, 248, 0.75)
    );
    position: absolute;
    border-radius: 50%;
    z-index: 1;
}
.info h1{
    font-size: 2.3rem;
    transition: all 0.75s ease-out;
}
.info h3{
    font-weight: lighter;
    font-size: 1.2rem;
    color: rgb(137, 150, 160);
    padding: 1rem 0rem;
    transition: all 0.75s ease-out;
}
.purchase button{
    width: 15rem;
    height: 2.8rem;
    background-color: transparent;
    border: white 3px solid;
    border-radius: 50px;
    color: rgb(255, 255, 255);
    font-weight: 1000;
    transition: all 0.3s ease;
}
.purchase button:hover{
    background-color: rgb(255, 255, 255);
    color: rgb(0, 0, 0);
    border: rgb(0, 0, 0) 3px solid;
    letter-spacing: 2px;
}
.sizes {
    transition: all 0.75s ease-out;
}
.sizes button{
    width: 3.5rem;
    margin-bottom: 10px;
    height: 2rem;
    border-radius: 35px;
}
button.active {
    background-color: rgb(135, 162, 175); 
    color: whitesmoke; 
    margin-top: 10px;
}

/* 2ND SNEAKER */

.container-2 {
    width: 50%;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
    background-color: rgb(114, 112, 111);
    border-bottom-left-radius: 50%;
    border-top-left-radius: 50%;
}
.card-2 {
    transform-style: preserve-3d;
    min-height: 85vh;
    width: 25rem;
    padding: 0rem 5rem;
    box-shadow: 0 20px 20px rgba(255, 255, 255, 0.2), 0px 0px 50px 20px rgba(255, 255, 255, 0.2);
    border-radius: 10px;
    background-color: rgb(93, 110, 124);
}
.shoe-2 {
    min-height: 35vh;
    display: flex;
    align-items: center;
    justify-content: center;
}
.shoe-2 img {
    width: 15rem; 
    z-index: 2;
    transition: all 0.75s ease-out;
}
.circle-2 {
    width: 13rem;
    height: 13rem;
    background: linear-gradient(
        to right,
        rgba(82, 88, 98, 0.75),
        rgba(248, 248, 248, 0.75)
    );
    position: absolute;
    border-radius: 50%;
    z-index: 1;
}
.info-2 h1{
    font-size: 2.3rem;
    transition: all 0.75s ease-out;
}
.info-2 h3{
    font-weight: lighter;
    font-size: 1.2rem;
    color: rgb(137, 150, 160);
    padding: 1rem 0rem;
    transition: all 0.75s ease-out;
}
.purchase-2 button{
    width: 15rem;
    height: 2.8rem;
    background-color: transparent;
    border: white 3px solid;
    border-radius: 50px;
    color: rgb(255, 255, 255);
    font-weight: 1000;
    transition: all 0.3s ease;
}
.purchase-2 button:hover{
    background-color: rgb(255, 255, 255);
    color: rgb(0, 0, 0);
    border: rgb(0, 0, 0) 3px solid;
    letter-spacing: 2px;
}
.sizes-2 {
    transition: all 0.75s ease-out;
}
.sizes-2 button{
    width: 3.5rem;
    margin-bottom: 10px;
    height: 2rem;
    border-radius: 35px;
}
button.active-2 {
    background-color: rgb(135, 162, 175); 
    color: whitesmoke; 
    margin-top: 10px;
}

</style>
<body>
    <header style="align-content: center;">
        <div class="logo">
            <img src="jordann.png" alt="logo">
        </div>
    </header>
    <!-- 1 SNEAKER -->
    <div class="container">
        <div class="card">
            <div class="shoe">
            <div class="circle"></div>
            <img src="j2.png" alt="Jordan">
            </div>
            <div class="info">
                <h1 class="title">Jordan x Dior Air</h1>
                <h3 >This is because naturally, some sizes are in much higher demand than others.</h3>
                <div class="sizes">
                    <button>39</button>
                    <button>40</button>
                    <button class="active">42</button>
                    <button>44</button>
                </div><br>
                <div class="purchase">
                    <button>Purchase</button>
                </div>
            </div>
        </div>
    </div>
    <!-- 2 SNEAKER -->
    <div class="container-2">
        <div class="card-2">
            <div class="shoe-2">
            <div class="circle-2"></div>
            <img src="jordan 1.png" alt="jordan">
            </div>
            <div class="info-2">
                <h1 class="title-2">Jordan 1 Mid Pink</h1>
                <h3 >This is because naturally, some sizes are in much higher demand than others.</h3>
                <div class="sizes-2">
                    <button>39</button>
                    <button class="active-2">40</button>
                    <button>42</button>
                    <button>44</button>
                </div><br>
                <div class="purchase-2">
                    <button>Purchase</button>
                </div>
            </div>
        </div>
    </div>

    <script>
    //Movement Animation happen
const card = document.querySelector('.card');
const container = document.querySelector('.container');
//items
const title = document.querySelector('.title');
const shoe = document.querySelector('.shoe img');
const purchase = document.querySelector('.purchase button');
const description = document.querySelector('.info h3');
const sizes = document.querySelector('.sizes');

//Moving Animation Event
container.addEventListener("mousemove", (e) => {
    let xAxis = (window.innerWidth / 2 - e.pageX) / 10;
    let yAxis = (window.innerHeight / 2 - e.pageY) / 10;
    card.style.transform = `rotateY(${xAxis}deg) rotateX(${yAxis}deg)`;
});

//Animation IN
container.addEventListener("mouseenter", (e) => {
    card.style.transition = none;
});

//Animation OUT
container.addEventListener("mouseleave", (e) => {
    card.style.transition = "all 0.5s ease"
    card.style.transform = `rotateY(0deg) rotateX(0deg)`;
});

container.addEventListener("mouseenter", (e) => {
    //popout
    title.style.transform = "translateZ(150px)";
    shoe.style.transform = "translateZ(200px) rotateZ(-45deg)";
    description.style.transform = "translateZ(150px)";
    purchase.style.transform = "translateZ(75px)";
    sizes.style.transform = "translateZ(125px)";
    title.style.color = "black";
    card.style.background = "rgb(175, 133, 164)";
    description.style.color = "white";
});

container.addEventListener("mouseleave", (e) => {
    //popback
    title.style.transform = "translateZ(0px)";
    shoe.style.transform = "translateZ(0px) rotateZ(0deg)";
    description.style.transform = "translateZ(0px)";
    purchase.style.transform = "translateZ(0px)";
    sizes.style.transform = "translateZ(0px)";
    title.style.color = "";
    card.style.background = "";
    description.style.color = "";
});
//-----------------------------------------------------------------------------------------------//
//2ND SNEAKER

//Moving Animation
const secondcard = document.querySelector(".card-2");
const secondcontainer = document.querySelector(".container-2");

//items
const stitle = document.querySelector('.title-2');
const sshoe = document.querySelector('.shoe-2 img');
const spurchase = document.querySelector('.purchase-2 button');
const sdescription = document.querySelector('.info-2 h3');
const ssizes = document.querySelector('.sizes-2');

//Moving Animation Event
secondcontainer.addEventListener("mousemove", (e) => {
    let xAxis = (window.innerWidth / 2 - e.pageX) / 10;
    let yAxis = (window.innerHeight / 2 - e.pageY) / 10;
    secondcard.style.transform = `rotateY(${xAxis}deg) rotateX(${yAxis}deg)`;
});

//Animation IN
secondcontainer.addEventListener("mouseenter", (e) => {
    secondcard.style.transition = none;
    
});

//Animation OUT
secondcontainer.addEventListener("mouseleave", (e) => {
    secondcard.style.transition = "all 0.5s ease";
    secondcard.style.transform = `rotateY(0deg) rotateX(0deg)`;
});

secondcontainer.addEventListener("mouseenter", (e) => {
    //popout
    stitle.style.transform = "translateZ(150px)";
    sshoe.style.transform = "translateZ(200px) rotateZ(-45deg)";
    sdescription.style.transform = "translateZ(150px)";
    spurchase.style.transform = "translateZ(75px)";
    ssizes.style.transform = "translateZ(125px)";
    stitle.style.color = "black";
    secondcard.style.background = "rgb(175, 133, 164)";
    sdescription.style.color = "white";
});

secondcontainer.addEventListener("mouseleave", (e) => {
    //popback
    stitle.style.transform = "translateZ(0px)";
    sshoe.style.transform = "translateZ(0px) rotateZ(0deg)";
    sdescription.style.transform = "translateZ(0px)";
    spurchase.style.transform = "translateZ(0px)";
    ssizes.style.transform = "translateZ(0px)";
    stitle.style.color = "";
    secondcard.style.background = "";
    sdescription.style.color = "";
});
//-----------------------------------------------------------------------------------------------//




    </script>
</body>
</html>
