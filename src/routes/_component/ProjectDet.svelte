<script>
	export let title = 'Acomplishment Title';

	export let cl1 = 'dastan';

	export let photo = 'PhotoCommingSoon.png';
	export let alt = 'Project Pic';
</script>

<style>
    .light{
        width: 400px;
        font-size: 12px;
        font-weight: 300;
        color: var(--text-color);
        margin-top: 15px;
        margin-bottom: 0px;
    }

    .bold {
				width: 400px;
        font-size: 15px;
        font-weight: 700;
        color: var(--text-color);
        margin-bottom: 0px;
        margin-top: 0px;
    }
    .group {
        width: calc(100% - 478px);
        height: 211px;
        padding-left: 239px;
        padding-right: 239px;
        margin-top: 50px;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }
		img{
				margin-left: 50px;
		}
</style>
<div class='group'>
	<div >
		<h1 class='bold'>{title}</h1>
		<h2 class='light'>{cl1}</h2>
	</div>
	<img src={photo} alt={alt}>
</div>
