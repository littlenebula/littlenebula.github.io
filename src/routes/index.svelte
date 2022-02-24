<script lang="ts">
  
</script>

<header>
    <img src="logo.svg" alt="" />
    <h1>Little Nebula</h1>
</header>

<footer>
    A <a href="https://nathanhoad.net">Nathan Hoad</a> project.
</footer>


<style>
    :global(body) {
      margin: 0;
      padding: 0;  
      background: #111;
      color: #f9f9f9;
    }

    header {
        max-width: 900px;
        margin: 80px auto;
        text-align: center;
    }

    header > img[src^="logo"] {
        animation-name: float;
        animation-duration: 2s;
        animation-timing-function: ease-in-out;
        animation-iteration-count: infinite;
        animation-direction: alternate;
    }

    @keyframes float {
        0% {
            transform: translateY(-3%);
        }
        100% {
            transform: translateY(3%);
        }
    }

    h1 {
        font-size: 50px;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-weight: normal;
        letter-spacing: 1px;
    }

    footer {
        text-align: center;
        position: absolute;
        bottom: 30px;
        left: 0;
        width: 100%;
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        font-size: 14px;
        color: #ccc;
    }
    footer a {
        color: #ccc;
    }
</style>