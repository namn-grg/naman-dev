<script>
    import Heading from '../shared/Heading.svelte';
    let headingText = 'About';
</script>

<div id="about">
    <Heading {headingText} invisibleOnPhone="true" />
    <div class="section-content">
        <img class="my-photo" src="./images/my-photo.jpg" alt="Naman Garg" />
        <p class="about-me">
            Hello, I am Naman. Welcome to my website!
            <br />
            <br />
            I am a 2nd year undergrad at
            <a href="https://iiitd.ac.in/" target="_blank">IIIT Delhi</a>,
            majoring in ECE. My major interests lies in CSE subjects. I am
            currently a improving my DSA.
            <br />
            <br />
            I'm constantly learning new things and technology.
            <br />
            I play badminton and seldom go to gym .I read manga or manhua or manhwa
            (whichever you are familier with).
        </p>
    </div>
</div>

<style>
    #about {
        margin-top: 40px;
        font-family: 'Overpass Mono', monospace;
        font-weight: 300;
        margin-bottom: -20px;
        color: #f5f5f5;
        font-size: large;
    }

    .section-content {
        width: 100%;
        display: flex;
        flex-direction: row;
        margin-top: 30px;
        align-items: center;
        justify-content: center;
        vertical-align: middle;
        line-height: 1.75;
    }

    .my-photo {
        height: 350px;
        width: 350px;
        padding: 40px;
        -webkit-filter: drop-shadow(0px 0px 20px #4c5154);
        filter: drop-shadow(0px 0px 20px #4c5154);
        border-radius: 50%;
    }

    p {
        vertical-align: middle;
    }

    @media only screen and (max-width: 700px) {
        .section-content {
            flex-direction: column;
        }
    }

    /* Mobile Styling */
    @media only screen and (max-width: 550px) {
        .section-content {
            flex-direction: column;
            align-items: center;
        }

        .my-photo {
            height: 200px;
            width: 200px;
            padding-top: 20px;
            padding-bottom: 10px;
        }

        #about {
            margin-top: 50px;
        }
    }
</style>
