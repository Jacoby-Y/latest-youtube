<nav>
    <a href="/">Latest YouTube</a>
    <gap/>
    <a href="/">Signup</a>
    <a href="/" id="login">Login</a>
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