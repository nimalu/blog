<template>
    <header>
        <NuxtLink class="site-title" to="/">niklaslutze</NuxtLink>
        <nav>
            <NuxtLink to="/posts">Posts</NuxtLink>
        </nav>
    </header>
    <main>
        <NuxtPage />
    </main>
</template>

<style>
:root {
    --almost-black: #15171B;
    --grey: #909296;
    --grey-dark: #303236;
    --grey-light: #a1a1aa;
    --dark-purple: #451952;
    --red-purple: #662549;
    --flower-red: #ae445a;
    --flower-red-dark: #5e141a;
    --honey: #f39f5a;

    --content-width: 48em;
    --content-padding: 1rem;
}

body {
    background-color: var(--almost-black);
    color: white;
    font-family: sans-serif;
}

header {
    max-width: var(--content-width);
    margin-left: auto;
    margin-right: auto;

    padding: 2rem var(--content-padding);

    display: flex;
}

.site-title {
    color: var(--honey);
    font-weight: bold;
    font-size: 1.3rem;
    flex-grow: 1;
}

nav a {
    color: var(--grey);
    font-weight: bold;
}
nav a:hover {
    color: var(--flower-red);
}

main {
    max-width: var(--content-width);
    margin-left: auto;
    margin-right: auto;
    padding: 0 var(--content-padding);
}

h1 {
    font-weight: bold;
    font-size: 3.5rem;
    line-height: 3.6rem;
}

h2 {
    font-weight: bold;
    font-size: 2rem;
    padding: 2rem 0 1rem 0;
}

p {
    line-height: 1.6rem;
    color: var(--grey-light);
    padding: 2rem 0;
}

p > a {
    color: var(--honey);
    text-decoration: underline;
    text-decoration-color: var(--flower-red-dark); 
    transition: linear all 0.2s;
}
p > a:hover {
    text-decoration-color: var(--flower-red); 
}
</style>
