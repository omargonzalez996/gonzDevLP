<script>
  import Icon from "@iconify/svelte";
</script>

<nav>
  <ul>
    <li>
      <a class="icono" href="https://github.com/omargonzalez996/">
        <Icon icon="mdi:github" />
      </a>
    </li>
    <li>
      <a class="icono"  href="https://www.instagram.com/omi.who96/">
        <Icon icon="ri:instagram-fill" />
      </a>
    </li>
    <li>
      <a class="icono"  href="https://www.facebook.com/omi.who">
        <Icon icon="ic:baseline-facebook" />
      </a>
    </li>
    <li>
      <a class="icono"  href="https://steamcommunity.com/profiles/76561198187820919/">
        <Icon icon="mdi:steam" />
      </a>
    </li>
  </ul>
</nav>

<style>
  .icono {
    height: 100px;
    width: 100px;
    color: white;
  }
  nav {
    padding: 1rem;
  }

  ul {
    list-style: none;
    display: flex;
    justify-content: space-evenly;
    padding: 0;
  }

  li {
    cursor: pointer;
    padding: 0.5rem;
    border: none;
    text-shadow: 6px 6px 0px rgba(0, 0, 0, 0.2);
  }

  li:hover {
    color: rgb(200, 230, 255);
    transition: 0.5s ease-in;
  }
</style>
