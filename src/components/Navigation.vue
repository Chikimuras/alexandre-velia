<template>
    <div id="navbar">
      <div id="logo">
        <a href="/" class="logo">Alexandre Velia</a>
      </div>
      <nav>
        <RouterLink to="/"><span>Home</span></RouterLink>
        <RouterLink to="/portfolio"><span>Portfolio</span></RouterLink>
        <RouterLink to="/contact"><span>Contact</span></RouterLink>
        <RouterLink to="/blog"><span>Blog</span></RouterLink>
      </nav>
    </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "navigation"
}
</script>

<style scoped>
  #navbar{

  }
  #logo{
    display: inline-block;
    margin-right: 1.8rem;
  }
  #logo a{
    font-size: 1.5rem;
    font-weight: 700;
    color: #000000;
    text-decoration: none;
  }
  #navbar{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 2rem;
  }
  nav a{
    background: var(--gradient);
    padding: 0.5rem 1rem;
    border-radius: .2rem;
    text-decoration: none;
    text-align: center;
    position: relative;
    margin-inline: .5rem;
  }
  nav a:before{
    content: "";
    position: absolute;
    inset: 0;
    border-radius: .15rem;
    background: #fff;
    transition: inset .1s ease-in-out;
  }
  nav a span{
    text-transform: uppercase;
    color: #000000;
    font-size: .875rem;
    font-weight: 600;
    z-index: 2;
    position: relative;
  }

  nav a:hover::before,
  nav a.router-link-active::before,
  nav a.router-link-exact-active::before{
    inset: 2px;
  }
</style>