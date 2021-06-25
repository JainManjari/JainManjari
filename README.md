<style>
    @import url('https://fonts.googleapis.com/css2?family=EB+Garamond&display=swap');
    @import url('https://fonts.googleapis.com/css2?family=Newsreader&display=swap');

   

    .body
    {
        background: linear-gradient(to bottom,#F08331,#88D06D);
        height:inherit;
        min-height:500px;
        width:100%;
        padding:10px 5px 10px;
        color:snow;
    }


    @keyframes fadeInDown {
        from {
            opacity:0;
            transform: translatey(-10px);
        }
        to {
            opacity:1;
            transform: translatey(0);
        }
    }

    .header
    {
        text-align:center;
        display:block;
        /* margin-bottom:15px; */
        font-family: 'EB Garamond', serif;  
        animation-name:fadeInDown;
        animation-duration:1s;
        animation-delay:0.8s;
        animation-fill-mode:both;
       
    }

  




    .header a
    {
        color:darkslategrey;
        background:lightgreen;
        border:1.8px solid slategrey;
        padding:4px;
        border-radius:13px 0px 13px 0px;
        font-size:19px;
        transition:all ease-in 0.6s;
    }
    .header a:hover
    {
        text-decoration:none;
        color:black;
        border-color:darkslategrey;
    }

    .intro
    {
        display:flex;
        justify-content:center;
        min-height:300px;
        border:1px solid;
        margin:0px auto 10px;
        flex-wrap:wrap;
        width:85%;
        box-sizing:border-box;
    }

    .intro > div
    {
        display:flex;
        justify-content:center;
        align-items:center;
        border: 1.5px solid black;
        margin:5px;
    }

    @keyframes rotateInDownRight {
        0% {
        -webkit-transform-origin: right bottom;
        transform-origin: right bottom;
        -webkit-transform: rotate3d(0, 0, 1, 45deg);
        transform: rotate3d(0, 0, 1, 45deg);
        opacity: 0;
        }
        100% {
        -webkit-transform-origin: right bottom;
        transform-origin: right bottom;
        -webkit-transform: none;
        transform: none;
        opacity: 1;
        }
    } 

    .intro .content
    {
        width:65%;
        min-width:250px;
        font-family: 'Newsreader', serif;
        font-size:15px;
        color:white;
        /* animation-name:rotateInDownRight;
        animation-duration:2s;
        animation-delay:8s;
        animation-fill-mode:both; */
        
    }

    @keyframes rotateInDownLeft {
        0% {
       
        transform: rotate3d(0, 0, 1, -45deg);
        opacity: 0;
        }
        100% {
       
        transform: none;
        opacity: 1;
        }
    } 

    .intro .img-container
    {
        min-width:250px;
        min-height:100%;
        display:flex;
        justify-content:center;
        align-items:center;
        /* animation-name:rotateInDownLeft;
        animation-duration:2s;
        animation-delay:8s;
        animation-fill-mode:both; */
    }

    @media screen and (max-width:900px)
    {
        .intro .content
        {
            width:85%;
        }
    }
    .intro .img-container img
    {
        min-width:inherit;
        height:300px;
    }

    .horizontal
    {
        list-style: none;
        padding-left: 0px;
        margin: 0px;
    }

    .horizontal li
    {
        display: inline-block;
        margin:0px 8px 8px 0px;
    }



    .horizontal li a
    {
        cursor: pointer;
        color:#fd7777;
        text-decoration: none;
    }

    .center
    {
        text-align: center;
    }

    .social .social-icons{
        width: 55%;
        margin: auto;
      
    }

    .social .social-icons li{
        margin: 5px;
        animation-duration:2s;
        animation-delay:1.6s;
        animation-fill-mode:both;
    }

    @keyframes bounceInLeft {
        0%, 60%, 75%, 90%, 100% {
        -webkit-transition-timing-function: cubic-bezier(0.215, 0.610, 0.355, 1.000);
        transition-timing-function: cubic-bezier(0.215, 0.610, 0.355, 1.000);
        }
        0% {
        opacity: 0;
        -webkit-transform: translate3d(-3000px, 0, 0);
        transform: translate3d(-3000px, 0, 0);
        }
        60% {
        opacity: 1;
        -webkit-transform: translate3d(25px, 0, 0);
        transform: translate3d(25px, 0, 0);
        }
        75% {
        -webkit-transform: translate3d(-10px, 0, 0);
        transform: translate3d(-10px, 0, 0);
        }
        90% {
        -webkit-transform: translate3d(5px, 0, 0);
        transform: translate3d(5px, 0, 0);
        }
        100% {
        -webkit-transform: none;
        transform: none;
        }
  } 

    
    @keyframes bounceInRight {
        0%, 60%, 75%, 90%, 100% {
        transition-timing-function: cubic-bezier(0.215, 0.610, 0.355, 1.000);
        }
        0% {
        opacity: 0;
        transform: translate3d(3000px, 0, 0);
        }
        60% {
        opacity: 1;
        transform: translate3d(-25px, 0, 0);
        }
        75% {
        transform: translate3d(10px, 0, 0);
        }
        90% {
        transform: translate3d(-5px, 0, 0);
        }
        100% {
        transform: none;
        }
    } 


    @keyframes slideInUp {
        0% {
        -webkit-transform: translateY(100%);
        transform: translateY(100%);
        visibility: hidden;
        }
        100% {
        -webkit-transform: translateY(0);
        transform: translateY(0);
        visibility:visible;
        }
    } 


    .social .social-icons li a img
    {
        border-radius: 50%;
        padding: 5px;
        height:35px;
        width:35px;
        transition: all 0.8s ease-in-out;

    }

    .social .social-icons li a img:hover
    {

        box-shadow: 0px 0px 6px 4px #8781B4;
    }

    .social-icons li:nth-child(1)
    {
        
        animation-name:bounceInLeft;
        animation-duration:2.5s;
        animation-delay:5.5s;
    }

    .social-icons li:nth-child(2)
    {
        animation-name:bounceInLeft;
        animation-duration:2.5s;
        animation-delay:3.5s;
    }

     .social-icons li:nth-child(3)
    {
         animation-name:slideInUp;
        animation-duration:2.5s;
        animation-delay:2s;
    }

     .social-icons li:nth-child(4)
    {
        animation-name:bounceInRight;
        animation-duration:2.5s;
        animation-delay:3.5s;
    }

     .social-icons li:nth-child(5)
    {
        animation-name:bounceInRight;
        animation-duration:2.5s;
        animation-delay:5.5s;
    }

</style>


<div class="body">
     <h2 class="header animate__animated  animate__fadeInDown">
            Namaste! I am Manjari Jain <span style="font-family:serif;">-</span> <a href="http://www.thehindflora.com">TheHindFlora</a>
    </h2>
    <div id="butter" class="social">
			<ul class="horizontal center social-icons">
					<li > <a href="https://www.linkedin.com/in/manjari-jain-3399b613a/" target="_blank"> 
                         <img src="https://img.icons8.com/fluent/48/000000/linkedin.png"/></a>
                    </li>
					<li> <a href="mailto:manjarijain98@gmail.com" target="_blank"> 
                         <img src="https://img.icons8.com/fluent/48/000000/gmail.png"/></a>
                    </li>
					<li> <a href="https://www.instagram.com/thehindflora/" target="-_blank"> 
                         <img src="https://img.icons8.com/fluent/48/000000/instagram-new.png"/></a>
                    </li>
					<li> <a href="https://www.quora.com/profile/Manjari-Jain-4" target="-_blank"> 
                         <img src="https://img.icons8.com/doodle/48/000000/quora.png"/></a>
                    </li>
		            <li> <a href="https://github.com/JainManjari?tab=repositories" target="-_blank"> 
                         <img src="https://img.icons8.com/material-sharp/48/000000/github.png"/></a>
                    </li>		
	        </ul>
	</div>
    <div class="intro">
        <div class="img-container">
           <img src="designer.gif">
       </div>
       <div class="content">
             I am a MERN Stack developer who loves to build and design optimal websites. Due to this, I love to keep track of all the latest front-end and back-end technologies. I was enrolled in a Teaching Assistantship (FullStack Development Course) for Coding Ninjas. At the end of it, I was the top mentor. I also have created a proper working social media site from scratch (http://www.skyinyou.com).
             <br>
             When I am not designing, then I have a strong passion for coding. My goto programming language is JAVA but I am also equally comfortable with Python and C/C++. I have completed my B. Tech (ECE) from VIT, Vellore, with a 9.23/10 CGPA in 2020. I was the recipient of a scholarship for my excellent academic performance for all 4 years. 
             <br>
             I am currently working with Bank of America as a Software Engineer. In Feb'21, I was lauded with the Bronze Medal-Internationally for my team efforts. My present role is concerned with the UI development of applications using React.
       </div>
    </div>
    <div>
        <a href="https://github.com/JainManjari">
            <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=JainManjari&layout=compact&show_icons=true&theme=buefy" />
        </a>
        <a href="https://github.com/JainManjari">
            <img src="https://github-readme-stats.vercel.app/api?username=JainManjari&hide=prs&layout=compact&show_icons=true&theme=buefy" />
        </a>
    </div>
</div>
