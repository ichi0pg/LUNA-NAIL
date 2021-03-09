<template>
  <footer class="footer">
    <div class="footer-wrap">
      <img class="footer-logo" src="../assets/logo-pink.png">
      <img class="footer-logo2" src="../assets/logo_black.png">
      <nav class="footer-nav">
        <ul>
          <li><a class="link" @click="$router.push('/')">HOME</a></li>
          <li><a class="link" @click="$router.push('/about')">ABOUT</a></li>
          <li><a class="link" @click="$router.push('/menu')">MENU</a></li>
          <li><a class="link" @click="$router.push('/sns')">SNS</a></li>
          <li><a class="link" @click="$router.push('/profile')">PROFILE</a></li>
        </ul>
      </nav>
    </div>
    <div class="wrapper">
      <p><small class="copyright">&copy; 2021 Runa</small></p>
    </div>
  </footer>
</template>

<script>
export default {
  
}
</script>

<style scoped>
.footer-wrap {
  height: 90px;
  padding-top: 10px;
  background-color: #000;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.footer-logo {
  height: 55px;
  margin: 10px 50px;
  display: flex;
}
.footer-logo2 {
  display: none;
}
.footer-nav ul {
  display: flex;
}
.footer-nav {
  margin-right: 30px;
  font-size: 12px;
}
a.footer-nav {
  list-style: none;
}
.wrapper {
  width: 100%;
}
.copyright {
  display: flex;
  justify-content: center;
  width: 100%;
  background-color: #000;
  color: #fac6cb;
  font-size: 10px;
  padding-bottom: 5px;
}

@media screen and (max-width: 768px) {
  .footer-nav {
    display: none;
  }
  .footer-wrap {
    display: flex;
    justify-content: center;
    height: 50px;
  }
  .footer-logo {
    height: 40px;
  }
  .copyright {
    padding-top: 5px;
    font-size: 6px;
  }
}

@media screen and (max-width: 480px){
  .footer-wrap {
    display: none;
  }
  .footer-logo {
    display: none;
  }
  .copyright {
    background-color: rgba( 255, 255, 255, 0.6);
    color: #333;
  }
}
</style>