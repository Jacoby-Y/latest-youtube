<script>
    const onSignIn = (googleUser) => {
        var profile = googleUser.getBasicProfile();
        console.log('ID: ' + profile.getId()); // Do not send to your backend! Use an ID token instead.
        console.log('Name: ' + profile.getName());
        console.log('Image URL: ' + profile.getImageUrl());
        console.log('Email: ' + profile.getEmail()); // This is null if the 'email' scope is not present.
    }

</script>

<nav>
    <a href="/">Latest YouTube</a>
    <gap/>
    <a href="/">Signup</a>
    <!-- <a href="#" class="g-signin2" data-onsuccess="onSignIn">Login</a> -->
    <div class="g-signin2" data-onsuccess="onSignIn"></div>
</nav>

<style>
    nav {
        padding: 0 1rem;
        height: max-content;
        display: grid;
        grid-template-columns: max-content 1fr repeat(2, max-content);
        background-color: #17191f;
        gap: 1rem;
    }
    nav a {
        padding: 1rem;
        font-size: 1.4rem;
    }
    #login {
        background-color: red;
        border-radius: 1rem;
        padding: 0.6rem 1rem;
        margin: 0.4rem 0;
        transition-duration: 0.1s;
    }
    #login:hover {
        background-color: whitesmoke;
        color: black;
    }
</style>