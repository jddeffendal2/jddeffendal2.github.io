<script setup>
  import eyeTrackingQuestion from "@/assets/eyeTrackingQuestion.png";
  import movieRentalImage from "@/assets/movieRentalImage.png";
  import movieShoppingCart from "@/assets/movieShoppingCart.png";
  import noWebcamQuestion from "@/assets/noWebcamQuestion.png";
</script>

<template>
  <div class="header">
    <h1 class="nameHeader">Jeremiah Deffendall</h1>
    <p class="email">jeremiah.deffendall@gmail.com &#x2022;</p> 
    <p class="phoneNumber"> (765) 228-9183</p>
    <br/><br/><br/><br/>
    <p class="summary"> I am a software developer with a BS Computer Science degree from Ball State University.
I have great front-end and back-end development skills and I am seeking a software
development position. I have previous experience with communicating and developing
software as a part of a team.
    </p>
    <br/><br/><br/><br/>
  </div>
  <div class="education">
    <h1 class="divHeaders">Education</h1>
    <div class="highSchool">
      <p class="schoolTitle">Monroe Central Jr./Sr. High School &nbsp;&nbsp;&nbsp;&nbsp;(August 2015 - May 2019)</p>
      <div class="educationInfo">
        <p>Valedictorian</p>
        <p>GPA: </p>
        <p>Indiana Core 40 With Academic Honoss</p>
      </div>
    </div>
    <br/><br/>
    <div class="college">
      <p class="schoolTitle">Ball State University &nbsp;&nbsp;&nbsp;&nbsp;(August 2019 - May 2023)</p>
      <br/>
      <div class="educationInfo">
        <p>Degree: Bachelor of Science in Computer Science</p>
        <p>GPA: 3.990</p>
        <p>Summa Cum Laude</p>
      </div>
    </div>
    <br/><br/><br/><br/>
  </div>
  <div class="experience">
    <h1 class="divHeaders">My Projects</h1>
    <div class="projects">
      <p class="divSmallTitles">
        Capstone Project - RefReps
      </p>
      <p class="projectDescription">
        RefReps is a referee training company that trains the future generations of referees. <br/><br/>
        We developed a full-stack web application with the goal to improve the efficiency and effectiveness of referee training through video quizzes uploaded by instructors.

        The application lets instructors create multiple types of referee training video quizzes for students to take, including eye-tracking quizzes, word-bank quizzes, and simple predict the foul call quizzes. 
        <br/><br/>I worked on many parts of the project in both the front-end and back-end. For one of my tasks of the project, I implemented an open-source eye-tracking library that was used to evaluate if the referee trainee is effectively learning how to referee by actually watching the play correctly and not just guessing. (achieved through the use of the user's webcam)
      </p>
      <img :src="eyeTrackingQuestion" width="400"> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
      <img :src="noWebcamQuestion" height="214" width="400">
      <br/><br/>
      <p class="divSmallTitles">
        Other Projects:
      </p>
      <br/>
      <p class="divSmallTitles">Movie Rental Website</p>
      <p class="projectDescription">
        Created a movie rental website for a class project that allowed admins to add movies to the website, and for users to "buy" and "rent" movies as well. <br/>
        Tech-stack: Javascript, HTML, CSS, PHP, WAMPServer <br/><br/>
        Github Link: Private Repository (unable to share link)<br/><br/>

        <img :src="movieRentalImage" height="214" width="400"> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
        <img :src="movieShoppingCart" height="214" width="400">
      </p>
      <br/>
      <p class="divSmallTitles">Vessel AIS Website</p>
      <p class="projectDescription">
        Created a website that automatically updates and shows the new locations of vessels on a map based on their most recent AIS messages from a dataset.
        <br/><br/>
        <a class="socialLink2" href="https://github.com/jddeffendal2/ais-website">Github Repository</a> <br/>
      </p>
      <p>

      </p>
    </div>
    <br/><br/><br/><br/>
  </div>
  <div class="skills">
    <h1 class="divHeaders">Skills</h1>
    <div class="mySkills">
      <p class="divSmallTitles">Languages/Frameworks</p>
      <ul class="skillsList">
        <li>Java</li>
        <li>JavaScript</li>
        <li>Typescript</li>
        <li>Node.js</li>
        <li>Vue.js</li>
        <li>C#</li>
        <li>.NET</li>
        <li>Python</li>
        <li>HTML</li>
        <li>CSS</li>
        <li>PHP</li>
        <li>MySQL</li>
        <li>MongoDB</li>
        <li>Kotlin</li>
      </ul>
      <p class="divSmallTitles">Tools</p>
      <ul class="skillsList">
        <li>Visual Studio Code</li>
        <li>Visual Studio</li>
        <li>Git</li>
        <li>Android Studio</li>
        <li>IntelliJ IDEA</li>
      </ul>
    </div>
  </div>
  <div class="interests">
    <h1 class="divHeaders">About Me</h1>
    <div class="aboutMe">
      <div class="divSmallTitles">Interests</div>
      <p class="aboutMeDescription">In my freetime, I enjoy writing code, exercising, playing video games, and playing basketball.</p>
      <div class="divSmallTitles">Awards</div>
      <ul class="aboutMeLIst">
        <li>Valedictorian at Monroe Central High School</li>
        <li>Dean’s List every semester of my college career</li>
        <li>Graduated with Summa Cum Laude from Ball State University</li>
        <li>Indiana and Global Seal of Biliteracy (English and Spanish)</li>
      </ul>
    </div>
  </div>
  <div class="links">
    <h1 class="divHeaders">Social Links</h1>
    <a class="socialLink" href="https://github.com/jddeffendal2">Github</a> <br/>
    <a class="socialLink" href="https://www.linkedin.com/in/jeremiah-deffendall/">LinkedIn</a>
    <br/><br/><br/><br/>
  </div>
</template>

<style scoped>
  .header, .education, .experience, .skills, .interests, .links {
    border-bottom: 1px solid #0ead83;
  }
  .nameHeader {
    color: #0ead83;
    font-size: 70px;
    text-shadow: lightgray 2px 2px;
    margin-left: 160px;
  }
  .divHeaders{
    color: #0ead83;
    font-size: 40px;
    text-shadow: lightgray 2px 2px;
    margin-left: 160px;  
  }
  .email {
    display: inline;
    font-size: 18px;
    color: gray;
    font-weight: bold;
    margin-left: 160px;
  }
  .phoneNumber {
    display: inline;
    font-size: 18px;
    color:#0ead83;
    font-weight: bold;
  }
  .summary {
    color: #595c5b;
    font-size: 18px;
    margin-left: 160px;
    margin-right: 160px;
  }

  .projectDescription, .aboutMeDescription  {
    color: #595c5b;
    font-size: 18px;
    margin-right: 120px;
  }

  .highSchool, .college, .projects, .mySkills, .aboutMe {
    margin-left: 160px;
  }
  .schoolTitle{
    display: inline;
    font-weight: bold;
    font-size: 18px;
    color: #0ead83;
  }
  .schoolDate {
    font-weight: bold;
    font-size: 13px;
    color: gray;
  }
  .educationInfo, .skillsList, .aboutMeLIst {
    font-weight: bold;
    color: gray;
  }
  .divSmallTitles {
    font-weight: bold;
    font-size: 18px;
    color: #0ead83;
  }
  .socialLink {
    margin-left: 160px;
    text-decoration: underline;
    font-weight: bold;
    color: gray;
  }
  .socialLink:hover {
    text-shadow: 1px 1px 1px lightgray;
  }
  .socialLink2 {
    text-decoration: underline;
    font-weight: bold;
    color: gray;
  }
  .socialLink2:hover {
    text-shadow: 1px 1px 1px lightgray;
  }
</style>
