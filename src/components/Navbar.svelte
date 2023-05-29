<script>
  import Icon from "@iconify/svelte";
</script>

<nav>
  <ul>
    <li>
      <a class="icono" href="https://github.com/omargonzalez996/">
        <Icon icon="mdi:github" class="big-icon" />
      </a>
    </li>
    <li>
      <a class="icono" href="https://www.instagram.com/omi.who96/">
        <Icon icon="ri:instagram-fill" class="big-icon" />
      </a>
    </li>
    <li>
      <a class="icono" href="https://www.facebook.com/omi.who">
        <Icon icon="ic:baseline-facebook" class="big-icon" />
      </a>
    </li>
    <li>
      <a
        class="icono"
        href="https://steamcommunity.com/profiles/76561198187820919/"
      >
        <Icon icon="mdi:steam" class="big-icon" />
      </a>
    </li>
    <li>
      <a class="icono" href="https://wa.me/524661342722">
        <Icon icon="ri:whatsapp-fill" class="big-icon" />
      </a>
    </li>
    <li>
      <a class="icono" href="mailto:ejemplo@example.com">
        <Icon icon="material-symbols:mail" class="big-icon" />
      </a>
    </li>
  </ul>
</nav>

<style>
  a :global(.big-icon) {
    font-size: 80px;
    color: white;
    &:hover {
      color: whitesmoke;
      font-size: 90px;
      transition: 0.2s ease-in;
    }
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
  }
  @media (max-width: 534px) {
    a :global(.big-icon) {
    font-size: 50px;
    color: white;
  }
</style>
