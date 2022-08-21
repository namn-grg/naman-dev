<div class="social-icons">
    <div class="container">
        <img
            class="logo github"
            src="./images/socials/github.svg"
            alt="github logo"
        />
        <a href="https://github.com/naman-ng/" target="_blank">
            <p class="logo-label">GitHub</p>
        </a>
    </div>
    <div class="container">
        <img
            class="logo linkedin"
            src="./images/socials/linkedin.svg"
            alt="linkedin logo"
        />
        <a href="https://linkedin.com/in/naman-garg-35564a239/" target="_blank">
            <p class="logo-label">LinkedIn</p>
        </a>
    </div>
    <div class="container">
        <img
            class="logo twitter"
            src="./images/socials/twitter.svg"
            alt="twitter logo"
        />
        <a href="https://twitter.com/gragnaman/" target="_blank">
            <p class="logo-label">Twitter</p>
        </a>
    </div>
</div>

<style>
    .social-icons {
        display: flex;
        flex-direction: row;
        flex-wrap: wrap;
        margin-top: -15px;
        margin-bottom: 20px;
    }

    .logo {
        width: 30px;
        fill: #141b1f;
    }

    .logo-label {
        padding-left: 5px;
    }

    .container {
        display: flex;
        flex-direction: row;
        padding-left: 0;
        padding-right: 40px;
    }

    a {
        text-decoration: none;
        position: relative;
        border-bottom: none;
    }

    a::after {
        content: '';
        width: 94%;
        height: 0;
        display: inline;
        position: absolute;
        bottom: -19px;
        left: 6px;
        background: #4c5154;
        /* transition: all 0.3s ; */
    }

    a:hover::after {
        height: 2px;
    }

    a:hover {
        color: inherit;
        background: transparent;
    }
</style>
