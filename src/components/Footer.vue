<template>
  <div id="footer">
    <div class="container">
    <div class="logo">
      <h2>Alexandre Velia</h2>
    </div>
    <div class="content">
      <div class="infos">
        <ul>
          <li><p><i class="fa-solid fa-location-dot"></i> Auvergne Rhône-Alpes, France</p></li>
          <li><p><i class="fa-solid fa-phone"></i> <a href="phone:+33783063262">+33 7 83 06 32 62</a></p></li>
          <li><p><i class="fa-solid fa-envelope"></i> <a href="mailto:alexandre.m.velia@gmail.com">alexandre.m.velia@gmail.com</a></p></li>
        </ul>
      </div>
      <div class="nav">
        <nav>
          <RouterLink to="/"><span>Home</span></RouterLink>
          <RouterLink to="/portfolio"><span>Portfolio</span></RouterLink>
          <RouterLink to="/contact"><span>Contact</span></RouterLink>
          <RouterLink to="/blog"><span>Blog</span></RouterLink>
        </nav>
      </div>
    </div>
    </div>
  </div>
  <div class="copyright">
    <p>© {{ year }} Alexandre Velia. All rights reserved.</p>
  </div>
</template>

<script>
export default {
  name: "Footer",
  data(){
    return{
      year: new Date().getFullYear()
    }
  }
}
</script>

<style scoped>
#footer,
.copyright{
  background: #1b1b1b;
  color: #fff;
}

#footer{
  padding: 4rem 0;
}

.copyright{
  padding: 1rem 0;
  text-align: center;
}

.content{
  display: flex;
  gap: 3rem;
  align-items: center;
}
nav a{
  display: block;
}

nav a.router-link-active,
nav a.router-link-exact-active{
  color: #fff;
  text-decoration: underline;
}

a{
  color: #fff;
}

a:hover{
  text-decoration: underline;
}

ul{
  list-style: none;
  padding-inline-start: 0;
}

li{
  margin-bottom: 1rem;
}

i{
  margin-right: .5rem;
}

.logo h2{
  color: #fff;
  -webkit-background-clip: initial;
  -webkit-text-fill-color: inherit;
  background: none;
  font-size: 2.18rem;
}
</style>