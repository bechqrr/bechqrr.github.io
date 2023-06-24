html{
    font-family: "Nunito", sans-serif;
}

body{
    margin:0;
}

/* Nav bar START */
.nav-bar{
    width: 100%;
    color: white;
    text-align: center;
    font-size: large;
}

.nav-bar li {
    display: inline;
}

.nav-bar a{
    margin-right: 1%;
    margin-left: 1%;
    background-color: white;
    color: black;
    text-decoration: none;
    transition: all 0.2s ease;
}

.nav-bar a:hover{
    background-color: #f2f2f2;
    color: #52ab98;
    padding: 5px;
    border-radius: 5px;
}

.nav-bar ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}

.mobile-nav-bar{
    width: 100%;
    height: 35px;
    color: black;
    text-align: center;
    font-size: large;
}

#repo{
    position: absolute;
    right: 1rem;
    flex-direction: column;
    justify-content: space-between;
    text-decoration: none;
    background-color: #f2f2f2;
    color: #52ab98;
    padding: 5px;
    border-radius: 10px;
}
/* Nav bar END */


.parent{
    display: flex;
}

.parent.contacts{
    height: 100vh;
}

.sub-1.contact{
    padding-left: 10%;
    padding-right: 10%;
    background-color: #c8d8e4;
}

.sub-1.contact p{
    color: black;
}

.contacts-links{
    color: black;
    font-size: larger;
    margin: 4.5%;
    text-align: justify;
}

.sub-1{
    flex: 50%;
    height: auto;
    background-color: #2b6777;
}

.sub-1 p{
    color: white;
    font-size: larger;
    margin: 7%;
    text-align: justify;
}

#github {
    display: flex;
    text-align: left;
    align-items: center;
    justify-content: center;
}

#github #icon i {
    font-size: 46px;
    color: rgba(255, 255, 255, 0.6);
    font-style: normal;
    margin-right: 10px;
}

#github #label {
    text-decoration: none;
}

#github #username {
    font-size: 24px;
    color: rgba(255, 255, 255, 0.6);
}

#github #description {
    font-size: 14px;
    color: rgba(255, 255, 255, 0.6);
}

.github-card{
    display: flex;
    background-color: #1e4652;
    width: 270px;
    height: 80px;
    justify-content: center;
    margin: auto;
    margin-top: 10%;
    border-radius: 15px;
    margin-bottom: 5vh;
}

.sub-2{
    flex: 30%;
    background-color: #c8d8e4;
    display: flex;
    flex-direction: column;
    justify-content: center;
}

.sub-2 img{
    border-radius: 50%;
}

.title{
    text-align: center;
    color: white;
}

.title.contacts{
    color: black;
}

.toggle-button{
    position: absolute;
    top: .75rem;
    left: 1rem;
    display: none;
    flex-direction: column;
    justify-content: space-between;
    width: 30px;
    height: 21px;
}

.toggle-button .bar {
    height: 3px;
    width: 100%;
    background-color: black;
    border-radius: 10px;
}

.link{
    color: #52ab98;
    position: relative;
    text-decoration: none;
}

.link::before{
    text-decoration: underline;
    content: '';
    position: absolute;
    bottom: 0;
    right: 0;
    width: 0;
    height: 2px;
    background-color: #0ea36a;
    transition: width 0.6s cubic-bezier(0.25, 1, 0.5, 1);
}

.sub-3{
    background-color: #ebd6d6;
    height: auto;
    display: flex;
    flex-direction: column;
}

.cards-proj{
    margin: 10vh;
    justify-content: center;
    display: flex;
    flex-wrap: wrap;
}

.card{
    background-color: #ada2a2;
    width: 60vh;
    height: auto;
    justify-content: center;
    border-radius: 15px;
    opacity: 0.8;
    color: white;
    font-size: large;
    margin: 2vh;
    padding: 2vh;
    text-align: center;
    --hover: #ef8f6e;
    transition: all .35s ease-out;
}

.card:hover,
.card:focus {
  -webkit-animation: card 1s;
          animation: card 1s;
  box-shadow: 0 0 0 2em rgba(255, 255, 255, 0);
  transform: scale(1.05) perspective(1px);
  transition: all .5s ease-in-out;
}

@-webkit-keyframes card {
  0% {
    box-shadow: 0 0 0 0 var(--hover);
  }
}

.repo-card{
    background-color: #615d5d;
    justify-content: center;
    height: 8vh;
    line-height: 8vh;
    width: 35vh;
    margin: auto;
    margin-top: 10%;
    border-radius: 15px;
    margin-bottom: 5vh;
}

#repo-inside{
    color: #723f99;
}

#repo-inside #label{
    text-decoration: none;
}

#repo-inside #icon{
    color: #723f99;
}

#repo-inside #description {
    font-size: large;
    color: rgba(255, 255, 255, 0.6);
}

@media only screen and (max-width: 600px) {
    .toggle-button {
        display: flex;
    }

    .nav-bar {
        display: none;
    }

    .nav-bar{
        flex-direction: column;
        align-items: flex-start;
    }

    .nav-bar ul{
        width: 100%;
        flex-direction: column;
    }

    .nav-bar ul li a {
        display: block;
        margin: 15px;
        font-size: larger;
    }

    .nav-bar.active{
        display: flex;
    }

    .parent{
        flex-direction: column;
    }

    .sub-2 img{
        margin: 5vh;
    }
}

@media only screen and (min-width: 601px) {
    .mobile-nav-bar {
        display: none;
    }
}

@media (hover: hover) and (pointer: fine) {
    .link:hover::before{
      left: 0;
      right: auto;
      width: 100%;
    }
}
