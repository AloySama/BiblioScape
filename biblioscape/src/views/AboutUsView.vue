<template>
    <div class="ourStory">
        <h1 class="ourProject">Notre projet</h1>
        <p>Lorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum
        <br>Lorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum<br>
        Lorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum<br>
        Lorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum<br>
        Lorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum<br>
        Lorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum<br>
        Lorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum<br></p>
        <p><br>Lorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum
        <br>Lorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum<br>
        Lorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum<br>
        Lorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum<br>
        Lorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum<br>
        Lorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum<br>
        Lorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum dolor sitLorem ipsum<br></p>
    </div>
    <div class="ourTeam">
        <h1>Notre équipe</h1>
    </div>
    <div class="main">
        <div class="profile-card">
            <div class="img">
                <img src="../assets/profilPictures/elisa.png">
            </div>
            <div class="caption">
                <h3>Elisa Souchois</h3>
                <p>Développeuse</p>
            </div>
        </div>
        <div class="profile-card">
            <div class="img">
                <img src="../assets/profilPictures/alois.png">
            </div>
            <div class="caption">
                <h3>Aloïs Brengard</h3>
                <p>Développeur</p>
            </div>
        </div>
        <div class="profile-card">
            <div class="img">
                <img src="../assets/profilPictures/julien.png">
            </div>
            <div class="caption">
                <h3>Julien Prudhomme</h3>
                <p>Développeur</p>
            </div>
        </div>
        <div class="profile-card">
            <div class="img">
                <img src="https://1.bp.blogspot.com/-8c7QTLoyajs/YLjr2V6KYRI/AAAAAAAACO8/ViVPQpLWVM0jGh3RZhh-Ha1-1r3Oj62wQCNcBGAsYHQ/s16000/team-1-3.jpg">
            </div>
            <div class="caption">
                <h3>Damien Doe</h3>
                <p>Développeur</p>
            </div>
        </div>
        <div class="profile-card">
            <div class="img">
                <img src="https://1.bp.blogspot.com/-8c7QTLoyajs/YLjr2V6KYRI/AAAAAAAACO8/ViVPQpLWVM0jGh3RZhh-Ha1-1r3Oj62wQCNcBGAsYHQ/s16000/team-1-3.jpg">
            </div>
            <div class="caption">
                <h3>Noah Doe</h3>
                <p>Designer</p>
            </div>
        </div>
        <div class="profile-card">
            <div class="img">
                <img src="https://1.bp.blogspot.com/-8c7QTLoyajs/YLjr2V6KYRI/AAAAAAAACO8/ViVPQpLWVM0jGh3RZhh-Ha1-1r3Oj62wQCNcBGAsYHQ/s16000/team-1-3.jpg">
            </div>
            <div class="caption">
                <h3>Yohan Doe</h3>
                <p>Designer</p>
            </div>
        </div>
    </div>
</template>


<style scoped>
   * {
     margin: 0;
     padding: 0;
     box-sizing: border-box;
   }
   .ourTeam{
    margin-top: 6%;
   }
   .ourProject{
    margin-top: 2%;
    margin-bottom: 2%;
   }
   .main{
     width: 100%;
     height: 350px;
     display: flex;
     justify-content: center;
     align-items: center;
     /* background-color: #0c5db9; */
   }
   .profile-card{
     position: relative;
     font-family: sans-serif;
     width: 220px;
     height: 220px;
     background: #fff;
     padding: 30px;
     border-radius: 50%;
     box-shadow: 0 0 22px #3336;
     transition: .6s;
     margin: 15px;
     justify-content: space-between;
   }
   .profile-card:hover{
     border-radius: 10px;
     height: 260px;
   }
   .profile-card .img{
     position: relative;
     width: 100%;
     height: 100%;
     transition: .6s;
     z-index: 99;
   }
   .profile-card:hover .img{
     transform: translateY(-60px);
   }
   .img img{
     width: 100%;
     border-radius: 50%;
     box-shadow: 0 0 22px #3336;
     transition: .6s;
   }
   .profile-card:hover img{
     border-radius: 10px;
   }
   .caption{
     text-align: center;
     transform: translateY(-80px);
     opacity: 0;
     transition: .6s;
   }
   .profile-card:hover .caption{
     opacity: 1;
   }
   .caption h3{
     font-size: 21px;
     font-family: sans-serif;
   }
   .caption p{
     font-size: 15px;
     color: #0c52a1;
     font-family: sans-serif;
     margin: 2px 0 9px 0;
   }
   .caption .social-links a{
     color: #333;
     margin-right: 15px;
     font-size: 21px;
     transition: .6s;
   }
   .social-links a:hover{
     color: #0c52a1;
   }
</style>