<template>
  <footer class="footer">
            <div class="container">
                <div class="footer-box">
                    <router-link to="/" class="footer-logo logo"><img src="../assets/images/logo.png" alt="logo"></router-link>
                    <div class="footer-nav">
                        <ul>
                            <li><router-link to="/rest">Ресторанам </router-link></li>
                            <li><router-link to="/rest">Курьерам </router-link></li>
                            <li><router-link to="/rest">Пресс-центр </router-link></li>
                            <li><router-link to="/rest">Контакты</router-link></li>
                        </ul>
                    </div>
                    <div class="footer-social"><img src="../assets/images/social/ig.png" alt="ig-icon">
                        <img src="../assets/images/social/fb.png" alt="fb-icon">
                        <img src="../assets/images/social/vk.png" alt="vk-icon">
                    </div>
                </div>
            </div>
        </footer>
</template>

<script>
export default {

}
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

.footer-nav ul li {
  color: #595959;
  font-size: 18px;
  font-weight: 400;
}

.footer-nav ul li a {
  text-decoration: none;
  color: inherit;
}

.footer-social {
  display: flex;
  align-items: center;
  justify-content: flex-end;
  gap: 20px;
}
</style>