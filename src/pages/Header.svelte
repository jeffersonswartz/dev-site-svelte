<script>
    import { link } from "svelte-routing";
</script>

<style>
    .header-container {
        width: 100%;
        /* height: 20px; */

        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 20px;
    }

    .header-container a,
    .header-container a:visited {
        color: #fff !important;
    }

    .header-title {
        font-size: 30px;
        color: #fff;
        font-family: "Yellowtail", cursive;
    }
    img {
        width: 30px;
        filter: invert(1);
        margin-left: 10px;
    }
</style>

<div class="header-container">
    <div class="header-title">
        <a href="/" use:link>Jefferson Swartz</a>
    </div>
    <div class="header-actions">
        <!-- <a href="work" use:link><i class="material-icons">info</i></a> -->
        <!-- <Link to="work"><i class="material-icons">info</i></Link> -->
        <a href="https://twitter.com/iamjfswartz" target="_blank"><img src="images/twitter.svg" alt="twitter"></a>
        <a href="https://www.linkedin.com/in/jeffersonswartz/" target="_blank"><img src="images/linkedin.svg" alt="linkedin"></a>
        <a href="https://github.com/jeffersonswartz" target="_blank"><img src="images/github.svg" alt="github"></a>
    </div>
</div>
