<template>
    <header>
        <h1>Loja em VUE</h1>
        <nav>
           <ul>
             <li>
                <a href="">Home</a>
            </li>
            <li>
                <a href="">Canecas</a>
            </li>
            <li>
                <a href="">Sapatos</a>
            </li>
            <li>
                <a href="">Sobre</a>
            </li>
           </ul>
        </nav>
    </header>
</template>

<style>
    header {
        display: flex;
        height: 6rem;
        align-items: center;
        justify-content: space-between;
        padding: 0 5%;
    }

    ul {
        display: flex;
        gap: 1rem;
        list-style: none;
    }

    li a {
        color: #fff;
    }
</style>