<script>
    import Heading from '../shared/Heading.svelte';
    import Socials from '../shared/Socials.svelte';
    import ContactForm from '../shared/ContactForm.svelte';
    let headingText = 'Contact';

    function topFunction() {
        document.body.scrollTop = 0; // For Safari
        document.documentElement.scrollTop = 0; // For Chrome, Firefox, IE and Opera
    }
</script>

<div id="contact">
    <Heading {headingText} />
    <p class="text">
        You can get in touch with me by emailing me at <a
            href="naman21171@iiitd.ac.in">naman21171@iiitd.ac.in</a
        >.
    </p>
    <p>You can follow me on:</p>
    <Socials />
    <ContactForm />
    <p on:click={topFunction} id="scrollToTop">Back to top ↑</p>
</div>

<style>
    #contact {
        margin-top: 40px;
    }

    .text {
        margin-top: 50px;
    }

    #scrollToTop {
        white-space: nowrap;
        cursor: pointer;
        width: fit-content;
        position: relative;
        padding-bottom: 0;
        margin-bottom: 0;
        font-size: smaller;
        border-bottom: solid 2px #4c5154;
    }

    #scrollToTop:hover {
        font-weight: 500;
        background: #141b1f;
        transition: all 0.1s ease-in-out;
    }

    p {
        color: #f5f5f5;
    }
</style>
