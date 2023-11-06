<script setUp></script>

<template>
    <div class="nav">
        <nav class="nav-bar">
            <ul>
                <div class="flexStart">
                    <li><a href="#intro" class="active">Introduction</a></li>
                    <li><a href="#education">Education</a></li>
                    <li><a href="#projects">Projects</a></li>
                    <li><a href="#skills">Skills</a></li>
                    <li><a href="#aboutMe">About Me</a></li>
                    <li><a href="#socialLinks">Social Links</a></li>
                </div>
                <li class="flexEnd"><a href="" id="threeLines">
                        &equiv;
                    </a>
                </li>
            </ul>
        </nav>
    </div>
</template>

<style scoped>
.nav-bar {
    background-color: lightgray;
    box-shadow: 0 1px 1px lightgray;
    height: 60px;
    border-radius: 8px;
    padding: 8px 24px;
    position: fixed;
    top: 0;
    width: 100%;
    display: flex;
}

.nav-bar .icon {
    display: none;
}

.nav-bar ul {
    list-style: none;
}

.flexStart { 
    align-content: center;
    align-items: center;
    display: flex;
    justify-content: flex-start;
}

.flexEnd {
    align-content: center;
    align-items: center;
    display: flex;
    justify-content: center;
}
.nav-bar a {
    /* float: left; */
    /* display: block; */
    padding: 8px 16px;
    text-decoration: none;
    font-weight: bold;
    color: #0ead83;
}
#threeLines {
    /* font-size:20px; */
    transform: scale(1.8, 1.5);
    visibility: hidden;
}

@media screen and (max-width: 680px) {
  .nav-bar a {
    visibility: hidden;
  }
  #threeLines {
    visibility:visible;
  }
}



</style>