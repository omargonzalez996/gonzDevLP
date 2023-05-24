<script>
  let activeItem = null;

  function setActive(item) {
    activeItem = item;
  }
</script>

<nav>
  <ul>
    <li class:selected={activeItem === 'home'} on:click={() => setActive('home')}>Home</li>
    <li class:selected={activeItem === 'about'} on:click={() => setActive('about')}>About</li>
    <li class:selected={activeItem === 'services'} on:click={() => setActive('services')}>Services</li>
    <li class:selected={activeItem === 'contact'} on:click={() => setActive('contact')}>Contact</li>
  </ul>
</nav>

<style>
  nav {
    background-color: #333;
    color: #fff;
    padding: 1rem;
  }

  ul {
    list-style: none;
    display: flex;
    justify-content: space-between;
    padding: 0;
  }

  li {
    cursor: pointer;
    padding: 0.5rem;
    border-radius: 4px;
  }

  li:hover {
    background-color: #555;
  }

  .selected {
    background-color: #777;
  }
</style>
