<script>
  import { push, pop, replace } from 'svelte-spa-router';

  let user = { isLoggedIn: false };
  const handleLogin = () => {
    user.isLoggedIn = true;
    push('/home')
  }
</script>

<button on:click={handleLogin}>로그인</button>