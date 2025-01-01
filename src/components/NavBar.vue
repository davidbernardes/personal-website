<template>
    <nav>
            <ul>
            </ul>
            <ul>
                <li>
                    <a href="#about"  class="contrast outline" aria-label="Documentation">Sobre</a>
                </li>
                <li>
                    <a href="#services"  class="contrast outline" aria-label="Download">Serviços</a>
                </li>
                <li>
                    <a href="#projects"  class="contrast outline" aria-label="Download">Projetos</a>
                </li>
                <li>
                    <a href="#"  class="contrast outline" aria-label="Download">Currículo</a>
                </li>
            </ul>
            <ul>
            </ul>
    </nav> 
</template>

<style scoped>
nav{
    margin-top: 2em;
    background-color: var(--background-color);
}
a:hover{
    display: block;
    max-width: 100px;
    margin-top: 1rem;
    border-bottom: .125rem solid var(--primary);
    content: "";
}
</style>