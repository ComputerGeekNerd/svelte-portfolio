<script>
    let imgsrc = "/assets/logo.png";
</script>

<header class="header">
    <div class="logo">
        <img src="{imgsrc}?tr=w-400" alt="logo" class="logo-img"/>
        <h1 class="logo-title">Raksha A</h1>
    </div>

    <nav class="nav">
        <ul class="nav-list">
            <li class="nav-item">
                <a>Home</a>
            </li>
            <li class="nav-item">
                <a>About</a>
            </li>
            <li class="nav-item">
                <a>Work</a>
            </li>
            <li class="nav-item">
                <button class="nav-contact">Get in Touch</button>
            </li>
        </ul>
    </nav>
</header>

<style lang="scss">
    @import url('https://fonts.googleapis.com/css2?family=Bitter:ital@1&display=swap');

* {
    color: #f5cac2;
    font-family: 'Bitter', serif;
}

.header {
    position: fixed;
    display: flex;
    flex-flow: row nowrap;
    width: 100%;
    background: #303179;/* fallback for old browsers */
    background: -webkit-linear-gradient(to right, #303179, #1D2B64);  /* Chrome 10-25, Safari 5.1-6 */
    background: linear-gradient(to right, #303179, #1D2B64); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
    justify-content: space-between;
}

.logo {
    display: flex;
    align-items: center;
    margin-left: 2rem;
}

.logo {
    &-title {
        margin-left: 2rem;
    }

    &-img {
        object-fit: contain;
        width: 3rem;
        height: 3rem;
        // padding: 0 0.4rem;
    }
}

.nav {
    justify-content: flex-end;
}

.nav {
    &-list {
        display: flex;
        flex-flow: row nowrap;
        height: 100%;
        align-items: center;
        margin-top: 0;
    }

    &-item {
        margin-right: 3rem;
        list-style-type: none;
        font-size: 1.2em;
    }

    &-item a:hover {
        color: #fc575e;
        text-decoration: none;
        cursor: pointer;
    }

    &-contact {
        border: none;
        margin: 0;
        padding: 0.3rem 0.6rem;
        background: #fc575e;
    }

    &-item button:hover {
        background: #009ffd;
        text-decoration: none;
        cursor: pointer;
    }
}
</style>