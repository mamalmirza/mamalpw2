<style>
    footer {
        width: calc(100% - 60px);
        height: 75px;
        padding: 30px 30px;
        background: transparent;

    }

    .bar {

        width: calc(100% - 60px);
        height: 43px;
        padding-top: 25px;
        padding-left: 30px;
        padding-right: 30px;
        background-color: transparent;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
        border-top: 1px solid var(--gray-color);

    }

    .title {
        margin-bottom: 5px;
        font-size: 15px;
        font-weight: bolder;
        padding: 0px;


    }

    .detail {
        font-size: 12px;
        font-weight: lighter;
        margin: 0px;
        padding: 0px;
    }

    img {
        padding-right: 10px;
    }

    div {
        margin-left: 10px;
        margin-right: 10px;
    }
    a {
        color: var(--text-color);
        text-decoration: unset;

    }

</style>
<footer>
	<div class='bar'>
		<!---
		<div>
			<h1 class='title'> Phone </h1>
			<h2 class='detail'> +1 (639) 571-6707 </h2>
		</div>
		-->
		<div>
			<h1 class='title'> Email </h1>
			<h2 class='detail'> <a href='mailto:mirzaei.mohammadreza1997@gmail.com'> mirzaei.mohammadreza1997@gmail.com </a></h2>
		</div>
		<div>
			<h1 class='title'> Follow Me </h1>
			<!---
			<img src='twitter.png' alt='twitter logo'>
			--->
			<a href='https://www.linkedin.com/in/mohammad-reza-mirzaei-a9a2b213b/'><img src='linkedin.png'
																																									alt='linkedin logo'></a>
		</div>
		<div>
			<h2 class='detail'> © 2021 Mamal. </h2>
		</div>

	</div>

</footer>