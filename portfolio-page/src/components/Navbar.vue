<template>
    <div class="nav">
        <nav class="nav-bar" v-if="!isActive">
            <div class="flexStart">
                <a href="" id="threeLines" @click="openNavbar">
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
        </nav>
        <nav class="expandedNavbar" v-else>
            <p> hello</p>
        </nav>
    </div>
</template>

<script setup>
import { ref } from "vue";

 const isActive = ref(false);


const openNavbar = function () {
    isActive.value = true;
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
    background-color: #0ead83;
    box-shadow: 0 1px 1px lightgray;
    height: 100px;
    border-radius: 10px;
    padding: 8px 24px;
    position: fixed;
    top: 0;
    width: 100%;
}

.flexStart { 
    align-content: center;
    align-items: center;
    display: flex;
    justify-content: flex-start;
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
.nav-bar a {
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

@media screen and (max-width: 680px) {
  .nav-bar a {
    visibility: hidden;
  }
  #threeLines {
    visibility:visible;
  }
}



</style>