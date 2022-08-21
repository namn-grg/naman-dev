<script>
    let headingText = 'Naman Garg';
</script>

<header>
    <h2>{headingText}</h2>
    <div class="navbar">
        <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#experience">Experience</a></li>
            <li><a href="#contact">Contact</a></li>
            <li><a href="https://naman/resume">Resume</a></li>
        </ul>
    </div>
</header>

<style>
    header {
        color: #f5f5f5;
        font-family: 'Overpass Mono', monospace;
        text-align: center;
        margin-top: 20px;
    }

    h2 {
        font-size: 22px;
        font-weight: 500;
        font-family: 'Overpass', sans-serif;
        color: #b3b3b3;
        margin-top: -20px;
        margin-bottom: 20px;
    }

    a {
        text-decoration: none;
        color: inherit;
        border-bottom: none;
        padding: 5px 0;
    }

    .navbar {
        background-color: #141b1f;
        padding: 5px;
        box-shadow: 0px 0px 20px 5px #4c5154;
        border-radius: 20px;
    }

    ul {
        font-size: 20px;
        list-style: none;
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        margin: 0;
        padding: 0;
    }

    a {
        position: relative;
    }

    a:hover {
        background: transparent;
    }

    a::after {
        content: '';
        width: 100%;
        height: 0;
        display: block;
        position: absolute;
        bottom: 3px;
        left: 0;
        background: #4c5154;
    }

    a:hover::after {
        height: 2px;
    }

    a:hover {
        font-weight: 300;
    }

    /* Mobile Styling */
    @media only screen and (max-width: 550px) {
        .navbar {
            border-radius: 0;
            left: 0;
            /* width: 100vw; */
            margin: 0;
            font-size: 15px;
            margin-bottom: -30px;
        }

        h2 {
            font-size: 20px;
        }
    }
</style>
