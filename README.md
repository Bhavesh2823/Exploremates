@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');
/* *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}*/

body{
    font-family: 'Poppins', sans-serif;
}

header{
    width: 80%;
    height: 95vh;
    /*border: 2px solid black;*/
    margin: auto; /*only left side and right side margin will be adjust here - Bhavesh*/
}

header nav{
    width: 95%;
    height: 7%;
    /*border: 1px ridge green;*/
    margin: auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

header nav ul{
    list-style: none; /*will remove the styling on list items*/
    display: flex;
}

header nav ul li{
    padding: 5px 13px;
}

header nav ul li a{
    text-decoration: none;
    color: black;
    margin: 2px 8px 2px 4px;
    font-size: 15px;
    font-weight: 500;
    transition: .3s linear;
}

header nav ul li a:hover{
    color: gray;
    font-size: 14px;
}

header nav ul li:nth-last-child(1){
    background-color: black;
    border-radius: 15px;
    padding: 5px 20px;
}

header nav ul li:nth-last-child(1) a{
    color: white;
}

header nav .bi-three-dots{
    display: none;
}

header .content{
    width: 100%;
    height: 93%;
    /*border: 1px solid red;*/
    position: relative;
}

header .content::before{
    content: "";
    position: absolute;
    width: 100%;
    height: 80%;
    /*border: 1px solid blue;*/
    background: url('bg1.jpg') no-repeat center center/cover;
    border-radius: 12px;
    z-index: -1;
}

header .content .cont_box{
    width: 500px;
    height: auto;
    color: white;
    padding: 30px;
}

header .content .cont_box h1{
    line-height: 40px;
    font-weight: 800;
}

header .content .cont_box p{
    font-size: 14px;
    font-weight: 400;
    color: rgb(241,241,241);
}

header .content .cont_box button{
    margin-top: 20px;
    padding: 10px 20px;
    border-radius: 20px;
    border: 3px solid black;
    background: black;
    color: white;
    outline: none;
    cursor: pointer;
    transition: .3s linear;
}

header .content .cont_box button:hover{
    background: rgb(68, 67, 67);
    border: 3px solid rgb(98, 97, 97);
}

header .content .trip_box{
    position: relative;
    width: 95%;
    height: 200px;
    margin: auto;
    /*border: 1px solid black;*/
}

header .content .trip_box .search_box{
    position: absolute;
    top: 0;
    left: 0;
    width: 60%;
    height: 60px;
    display: flex;
    align-items: center;
    justify-content: center;
    background: white;
    border-radius: 5px;
    box-shadow: 10px 15px  10px rgb(30, 29, 29);
    z-index: 1;
    padding: 10px 20px;
}

header .content .trip_box .search_box .card{
    width: 200px;
    height: 100%;
}

header .content .trip_box .search_box .card h4{
    font-size: 15px;
    margin: 0;
    font-weight: 700;
}

header .content .trip_box .search_box .card .bi{
    position: absolute;
    font-size: 13px;
    margin: 2px 0px 0px 5px;
    transition: .3s linear;
}

header .content .trip_box .search_box .card input{
    margin-top: 3px;
    padding: 5px 0px;
    border: none;
    outline: none;
    font-size: 13px;
}

header .content .trip_box .search_box input[type="button"]{
    background: black;
    color: white;
    border: none;
    outline: none;
    padding: 10px 20px;
    border-radius: 20px;
    transition: .3s linear;
    cursor: pointer;
}

header .content .trip_box .search_box input[type="button"]:hover{
    background: rgb(68, 67, 67);
    border: 3px solid rgb(98, 97, 97);
}

header .trip_box .travel_box{
    position: relative;
    width: 100%;
    height: auto;
    margin: auto;
    /*background: black;*/
    top: 40px;
    border-radius: 10px;
    padding-bottom: 20px;
    box-shadow: 0px 20px 25px -10px rgb(165,165,165);
}

header .trip_box .travel_box::before{
    content: '';
    position: absolute;
    width: 100%;
    height: 100%;
    border-radius: 10px;
    background: rgb(241,241,241, .10);
    backdrop-filter: blur(5px);
    z-index: -1;    
}

header .trip_box .travel_box h4{
    margin: 0;
    padding: 60px 0px 15px 1.7%;
}

header .trip_box .travel_box .cards{
    width: 96%;
    height: auto;
    margin: 0px auto;
    /*border: 1px solid black;*/
    display: flex;
    align-items: center;
    justify-content: space-between;
}


header .trip_box .travel_box .cards .card{
    width: 220px;
    height: 180px;
    /*border: 1px solid black;*/
}

header .trip_box .travel_box .cards .card h3{
    margin: 0px 0px 10px 0px;
    display: flex;
    align-items: center;
    font-size: 16px;
    font-weight: 600;
}

/*header .trip_box .travel_box .cards .card h3 img{
    width: 20px;
    height: 20px;
    margin-left: 5px;

}*/

header .trip_box .travel_box .cards .card img{
    width: 100%;
    height: 50%;
}

header .trip_box .travel_box .cards .card .btn_city{
    display: flex;
    align-items: center;
    justify-content: space-between;
    /*border: 1px solid black;*/
}

header .trip_box .travel_box .cards .card .btn_city a{
    text-decoration: none;
    background:black;
    color: white;
    border-radius: 20px;
    padding: 6px 20px;
    font-size: 11px;
    transition: .3s linear;
}

header .trip_box .travel_box .cards .card .btn_city a:hover{
    background: rgb(68, 67, 67);
    /*border: 3px solid rgb(98, 97, 97);*/
}

header .trip_box .travel_box .cards .card .btn_city h5{
    font-size: 11px;
    font-weight: 500;
    margin: 0;
    margin-top: 5px;
    line-height: 15px;
}

