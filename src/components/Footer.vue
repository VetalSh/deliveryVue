<template>
  <footer class="footer">
    <div class="container footer-box">
      <router-link to="/" class="header-logo logo">
        <img src="../assets/img/logo.png" alt="logo" />
      </router-link>
      <div class="footer-nav">
        <ul>
          <router-link to="/rest">Ресторанам</router-link>
          <router-link to="/rest">Курьерам</router-link>
          <router-link to="/rest">Пресс-центр</router-link>
          <router-link to="/rest">Контакты</router-link>
        </ul>
      </div>
      <div class="footer-social">
        <img src="../assets/img/social/insta.png" alt="insta" class="social-image" />
        <img src="../assets/img/social/facebook.png" alt="FB" class="social-image" />
        <img src="../assets/img/social/vk.png" alt="VK" class="social-image" />
      </div>
    </div>
  </footer>
</template>

<script>
export default {};
</script>

<style scoped>
.footer {
  display: flex;
  align-items: center;
  min-height: 156px;
  padding: 60px 0;
}

.footer-box {
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 36px;
  flex-wrap: wrap;
}

.footer-nav {
  flex-grow: 1;
}

.footer-nav ul {
  display: flex;
  align-items: center;
  list-style: none;
  padding: 0;
  margin: 0;
  gap: 15px;
  flex-wrap: wrap;
}

.footer-nav ul a {
  color: #595959;
  font-size: 18px;
  font-weight: 400;
  text-decoration: none;
  cursor: pointer;
}

.footer-social {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 20px;
}
</style>