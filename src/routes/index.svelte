<script>
	import BigButton from './_component/BigButton.svelte';
	import ProfilePic from './_component/ProfilePic.svelte';

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
    .page {
        flex-direction: column;
        align-items: center;
        display: flex;

    }

    .main {

        width: 830px;
        height: 400px;


        background-color: transparent;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;

    }

    .right {
        width: 380px;
        height: 360px;
    }
		.B80{
				font-size: 80px;
				font-weight: 700;
				color: var(--text-color);
				margin-bottom: 20px;
				margin-top: 20px;
		}
    .B18{
        font-size: 18px;
        font-weight: 700;
        color: var(--text-color);
    }
    .R12{
        font-size: 12px;
        font-weight: 400;
        color: var(--text-color);
    }
		.buttons{
				margin-top: 45px;
		}

		a{
        color: var(--active-color);
        text-decoration: unset;
		}
</style>
<div class='page'>
	<div class='main'>
		<ProfilePic />

		<div class='right'>
			<h1 class='B80'> Hello </h1>
			<h1 class='B18'> A Bit About Me </h1>
			<h1 class='R12'>
				Hi. My Name is Mohammad Reaz Mirzaei.<br>
				Curently, I am a Msc Student at Universiy of Regina.</h1>

			<div class='buttons'>
				<a href='/resume'>
					<BigButton title='Resume' color='red' />
				</a>
				<a href='/projects'>
					<BigButton title='Projects' color='blue' />
				</a>
				<a href='/contact'>
					<BigButton title='Contact' color='orange' />
				</a>
			</div>
		</div>
	</div>
</div>


