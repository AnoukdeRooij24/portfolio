<nav>
    <a href="/">About me</a>
    <a href="/work">See my work</a>
    <a href="/experiments">See my experiments</a>
    <a href="/contact">Get in contact</a>
</nav>

<style>
    a {
    font-family: "glory";
    font-weight: 700;
    font-size: clamp(1rem, 2.5vw, 1.5rem);
    color: var(--accent-color);
    text-decoration: none;
    position: relative;
    display: block;
    transition: 0.5s;

        &::after {
        position: absolute;
        content: "";
        top: 100%;
        left: 0;
        width: 100%;
        height: 3px;
        border-radius: 3px;
        background: var(--accent-color);
        transform: scaleX(0);
        transform-origin: right;
        transition: transform 0.5s;
        }

        &:hover {
        color: var(--accent-color);
        }

        &:hover::after {
        transform: scaleX(1);
        transform-origin: left;
        }
}

nav {
    display: flex;
    flex-direction: row;
    gap: 1em;

}

</style>