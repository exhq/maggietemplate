<script lang="ts">
    export let discordid: string;
    let name = "maggie";
    const altnames = ["maggie 2", "maggie 3", "maggie 4"];

    function getRandomChild(array) {
        const randomIndex = Math.floor(Math.random() * array.length);
        return array[randomIndex];
    }
</script>

<img class="pfp" src="https://adu.shiggy.fun/v1/{discordid}/avatar" alt="" />
<br />
<h1 on:click={()=> {name = getRandomChild(altnames)}}>{name}</h1>

<style>
    .pfp {
        border-radius: 100%;
    }
</style>
