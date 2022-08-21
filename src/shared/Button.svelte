<script>
    export let type;
</script>

<button {type}>
    <slot />
</button>

<style>
    button {
        background: #141b1f;
        outline: none;
        color: white;
        font-family: 'Overpass', sans-serif;
        font-weight: lighter;
        border: solid 1px #4c5154;
        cursor: pointer;
        padding: 8px 15px;
        border-radius: 3px;
        box-shadow: 1px 2px 5px #4c5154;
    }

    button:hover {
        background: #263036;
    }

    button:active {
        background: #141b11;
    }
</style>
