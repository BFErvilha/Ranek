<template>
  <div id="app">
    <TheHeader />
    <main id="main">
      <router-view/>
    </main>
    <TheFooter />
  </div>
</template>
<script>
import TheHeader from "@/components/TheHeader.vue"
import TheFooter from "@/components/TheFooter.vue"

export default {
  components:{
    TheHeader,
    TheFooter,
  }
  
}
</script>

<style lang="scss">

@import url('https://fonts.googleapis.com/css2?family=Nunito:ital,wght@0,200;0,300;0,400;0,600;0,700;0,800;0,900;1,200;1,300;1,400;1,600;1,700;1,800;1,900&display=swap');

*{
  box-sizing: border-box;
}

body, ul , li, h1,h2,p{
  padding: 0px;
}
ul{
  list-style: none;
}

body{
  font-family: 'Nunito';
  color: #345;
  background: url('./assets/pattern.svg') repeat top;
}

a{
  color: #345;
  text-decoration: none;
}

img{
  max-width: 100%;
  display:block;
}

/* width */
::-webkit-scrollbar {
  width: 7px;
}

/* Track */
::-webkit-scrollbar-track {
  background: #f1f1f1; 
}
 
/* Handle */
::-webkit-scrollbar-thumb {
  background:  #87F; 
  border-radius: 30px;
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #65d; 
}

.btn{
  display: block;
  padding: 10px 30px;
  background: #87F;
  border-radius: 4px;
  color: #fff;
  text-align: center;
  font-size: 1rem;
  box-shadow: 0 4px 8px rgba(30,60,90,0.2);
  transition: all 0.3s;
  border: none;
  font-family: 'Nunito';
  cursor: pointer;

  &:hover{
    background: #65d;
    transform: scale(1.1);
  }
}

#app{
  display: flex;
  min-height: 100vh;
  flex-direction: column;

  #main{
    flex: 1;
  }
}

input,textarea{
  border-radius: 4px;
  border: 1px solid white;
  padding: 15px;
  box-shadow: 0 4px 8px rgba(30,60,90,0.1);
  transition: all;
  font-size: 1rem;
  font-family: 'Nunito';
  margin-bottom: 15px;

  &:hover,
  &:focus{
    outline: none;
    box-shadow: 0 6px 12px rgba(30,60,90,0.2);
    border-color: #87f;
  }
}
</style>
