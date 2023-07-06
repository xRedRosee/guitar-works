<template>
    <nav class="navbar">
        <NuxtLink to="/" class="nav-name">
            <img src="gw-logo.png" alt="guitarworks logo" class="logo">
        </NuxtLink>
        <ul class="nav-list">
            <li class="nav-item">
                <NuxtLink to="/overons" class="nav-text">over ons</NuxtLink>
            </li>
            <li class="nav-item">
                <NuxtLink to="/onswerk" class="nav-text">ons werk</NuxtLink>
            </li>
            <li class="nav-item">
                <NuxtLink to="/prijzen" class="nav-text">prijzen</NuxtLink>
            </li>
            <li class="nav-item">
                <NuxtLink to="/selectseries" class="nav-text">Select Series</NuxtLink>
            </li>
            <li class="nav-item">
                <NuxtLink to="/pedalboards" class="nav-text">pedalboards</NuxtLink>
            </li>
            <li class="nav-item">
                <NuxtLink to="/contact" class="nav-text">contact</NuxtLink>
            </li>
        </ul>
        <button class="hamburgermenu" @click="hamburgerMenu">
            <span class="line"></span>
            <span class="line"></span>
            <span class="line"></span>
        </button>
    </nav>
</template>
<script>
export default {
    name: "Navbar",
    setup() {
        const route = useRoute()
    },
    data() {
        return {
            hamburgerOpen: false,
        }
    },
    methods: {
        hamburgerMenu() {
            const navBar = document.querySelector('.navbar');
            const navList = document.querySelector('.nav-list');
            const hamburger = document.querySelector('.hamburgermenu');

            if (this.hamburgerOpen == false) {
                // open the hamburger        
                navBar.classList.toggle("active");
                navList.classList.toggle("active");
                hamburger.classList.toggle("active");
                return this.hamburgerOpen = true;

            } else if (this.hamburgerOpen == true) {
                // close hamburger
                navBar.classList.remove("active");
                navList.classList.remove("active");
                hamburger.classList.remove("active");
                return this.hamburgerOpen = false;
            }
        }
    }

}
</script>
<style>
.navbar {
    width: 100%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: auto;
    flex-direction: row;
}

.nav-list {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: row;
    justify-content: flex-end;
    gap: 30px;
    margin-right: 30px;
    margin-top: 10px;
    width: 100%;
}

.logo {
    height: 70px
}

.nav-item {
    margin: 0;
    padding: 0;
}

.nav-text {
    margin: 0;
    padding: 0;
    color: var(--black);
    text-decoration: none;
    font-family: var(--normalfont);
    font-weight: var(--normalfontnormal);
    font-size: 24px;
    position: relative;
    cursor: pointer;
}

.nav-text:after {
    content: '';
    width: 0px;
    height: 1px;
    position: absolute;
    top: 100%;
    left: 0;
    background: var(--black);
    transition: 300ms;
}

.nav-text:hover:after {
    width: 100%;
}

.nav-text:not(:hover):after {
    right: 0;
    left: auto;
}

.hamburgermenu {
    background-color: none;
    outline: none;
    border: none;
    background: none;
    display: none;
}

.line {
    width: 30px;
    height: 2px;
    background-color: var(--black);
    margin: 6px auto;
    display: block;
    -webkit-transition: all 0.3s ease-in-out;
    transition: all 0.3s ease-in-out;
}

/* -------------------------------------------- media queries */
@media screen and (max-width: 768px) {
    .navbar {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        height: 100%;
        width: 100%;
        background-color: var(--white);
        margin: 0;
        padding: 0;
        height: 50px;
        z-index: 99;
    }

    .navbar.active {
        position: fixed;
        top: 0;
    }

    .nav-list {
        list-style: none;
        margin: 0;
        padding: 0;
        display: none;
        flex-direction: column;
        align-items: flex-end;
        justify-content: space-evenly;
        right: 0;
        width: 100%;
        top: 52px;
        z-index: 99;
        position: fixed;
        background-color: var(--white);
    }

    .nav-list.active {
        display: flex;
        height: 100%;
        justify-content: flex-start;
    }

    .nav-text {
        margin-right: 16px;
        font-size: 50px;
    }

    .hamburgermenu {
        display: block;
    }


    .hamburgermenu.active .line:nth-child(2) {
        opacity: 0;
    }

    .hamburgermenu.active .line:nth-child(1) {
        transform: translateY(8px) rotate(45deg);
    }

    .hamburgermenu.active .line:nth-child(3) {
        transform: translateY(-8px) rotate(-45deg);
    }
}
</style>