<script>
    import supabase from '$lib/db';

    async function logout() {
   	 const { error } = await supabase.auth.signOut();

   	 if (error) alert(error.message); // alert if error
    }

    

</script>
<div class="container">
<table class="table">
    <thead>
      <tr>
        <th scope="col">#</th>
        <th scope="col">1</th>
        <th scope="col">2</th>
        <th scope="col">3</th>
        <th scope="col">4</th>
        <th scope="col">-</th>
        <th scope="col">5</th>
        <th scope="col">6</th>
        <th scope="col">7</th>
        <th scope="col">8</th>
        <th scope="col">9</th>
        <th scope="col">10</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th scope="row">Mon</th>
        
        
      </tr>
      <tr>
        <th scope="row">Tues</th>
       
      </tr>
      <tr>
        <th scope="row">Wed</th>
        
      </tr>
      <tr>
        <th scope="row">Thurs</th>
        
      </tr>
      <tr>
        <th scope="row">Fri</th>
        
      </tr>
    </tbody>
  </table>
</div>

<!-- Sign Out -->
<section class="container px-4 py-3 text-center">
    <button class="btn btn-secondary" on:click={logout}>Logout</button>
</section>	

