<template>
    <div class="nav">
        <div class="nav-bar" >
            <div class="flexStart">
                <a id="threeLines" @click="openNavbar">
                    &equiv;
                </a>
            </div>
            <div class="flexMiddle">
                <a href="#intro" class="active">Introduction</a>
                <a href="#education">Education</a>
                <a href="#projects">Projects</a>
                <a href="#skills">Skills</a>
                <a href="#aboutMe">About Me</a>
                <a href="#socialLinks">Social Links</a>
            </div>
            <div class="flexEnd"></div>
        </div>
        <div class="expandedNavbar" v-if="isActive == true">
            <div id="flexStartTwo" class="flexStartTwo">
                <a id="threeLines" @click="closeNavbar">
                    &equiv;
                </a>
            </div>
            <a href="#intro" class="active" @click="closeNavbar">Introduction</a>
            <a href="#education" @click="closeNavbar">Education</a>
            <a href="#projects" @click="closeNavbar">Projects</a>
            <a href="#skills" @click="closeNavbar">Skills</a>
            <a href="#aboutMe" @click="closeNavbar">About Me</a>
            <a href="#socialLinks" @click="closeNavbar">Social Links</a>
        </div>
    </div>
</template>

<script setup>
import { ref } from "vue";

 const isActive = ref(false);


const openNavbar = function () {
    isActive.value = true;
}
const closeNavbar = function () {
    isActive.value = false;
}

    
</script>

<style scoped>
.nav-bar {
    background-color: #CC998D;
    box-shadow: 0 1px 1px lightgray;
    height: 60px;
    border-radius: 10px;
    padding: 8px 24px;
    position: fixed;
    top: 0;
    width: 100%;
    display: flex;
    gap: 0;
}

.expandedNavbar {
    background-color: #CC998D;
    box-shadow: 0 1px 1px lightgray;
    height: 300px;
    border-radius: 10px;
    padding: 8px 24px;
    position: fixed;
    top: 0;
    width: 100%;
    visibility: hidden;
}

.flexStart { 
    align-content: center;
    align-items: center;
    display: flex;
    justify-content: flex-start;
}

.flexStartTwo { 
    align-content: center;
    align-items: center;
    display: flex;
    justify-content: flex-start;
    margin-top: 30px;
}
.flexMiddle {
    align-content: center;
    align-items: center;
    display: flex;
    justify-content: center;
  }
.flexEnd {
    align-content: center;
    align-items: center;
    display: flex;
    justify-content: flex-end;
}
.nav-bar a, .expandedNavbar a {
    display: block;
    padding: 8px 16px;
    text-decoration: none;
    font-weight: bold;
    color: #ECEBE4;
}

a:hover {
    color: #879C9A;
}

#threeLines {
    transform: scale(1.8, 1.5);
    visibility: hidden;
}

#threeLines:hover {
    cursor: pointer;
}

@media screen and (max-width: 680px) {
  .nav-bar a {
    visibility: hidden;
  }
  #threeLines {
    visibility:visible;
  }

  .expandedNavbar {
    visibility: visible;
  }
}



</style>