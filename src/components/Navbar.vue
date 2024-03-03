<template>
    <nav class="navbar">
        <div class="navbar-links">
            <a href="#about">About</a>
            <a href="#projects">Projects</a>
            <a href="/" class="navbar-brand"><img src="../assets/ani-logo.png" height="75px" /></a>
            <a href="#skills">Skills</a>
            <a href="#contact">Contact</a>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'Navbar',
};
</script>

<style>
.navbar {
    height: 4em;
    background-color: #edece5;
    padding: 1em 0;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 100;
    display: flex;
    justify-content: center;
}

.navbar-links {
    display: flex;
    gap: 6em;
    align-items: center;
}

.navbar-links a {
    text-decoration: none;
    color: #0F1422;
    font-weight: 500;
    cursor: pointer;
    transition: 0.3s;
}

.navbar-brand {
    margin: 0 2em;
    cursor: pointer;
}
</style>
