<script>
	import { page } from '$app/stores';

	let navigations = [
		{
			url: '/resume',
			title: 'Resume'
		},
		{
			url: '/projects',
			title: 'Projects'
		},
		{
			url: '/contact',
			title: 'Contact'
		}
	];
</script>
<style>
    header {
        width: calc(100% - 70px);
        height: 25px;
        padding: 20px 35px;
        background: transparent;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
    }

    .circle {
        height: 20px;
        width: 20px;
        background: var(--orange-color);
        border-radius: 100%;
    }

    .title {
        margin-left: 10px;
        font-weight: 600;
        font-size: 15px;
    }

    .left, .right ul {
        display: flex;
        justify-content: center;
        align-content: center;
        flex-direction: row;
    }

    h2 {
        margin: 0;
        padding: 0;
				color: var(--text-color);

    }
    .right {
        font-size: 15;
				font-weight: 300;
        color: var(--text-color);

    }

    .right ul {
        list-style: none;

    }

    .right ul li {
        margin: 10px;
        display: flex;
    }

    a {
        color: var(--text-color);
        text-decoration: unset;

    }



    .vl {
        width: 1px;
        height: 20px;
        border-radius: 4px;
        background-color: var(--text-color);
        margin-left: 15px;
    }

    .right ul li:last-child {
        margin-right: unset;
    }

    .active {
        color: var(--active-color);
    }
</style>

<header>

	<div class='left'>
		<div class='circle'></div>
		<h2 class='title'>
			<a href='/'>Mohammad Reza Mirzaei</a>
		</h2>
	</div>

	<div class='right'>
		<ul>
			{#each navigations as navigation,i}
				<li>

						<a href='{navigation.url}'
						 class:active={$page.path.startsWith(navigation.url)}>
						{navigation.title}
					</a>

					{#if (i !== navigations.length - 1)}
						<span class='vl'></span>
					{/if}
				</li>
			{/each}
		</ul>
	</div>
</header>
