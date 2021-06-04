<script>
	export let tl1 = 'Acomplishment Title';
	export let tl2 = '';
	export let tl3 = '';
	export let year = '2018-2019';
	export let cl1 = '';
	export let cl2 = '';
	export let cl3 = '';
	export let cl4 = '';



</script>

<style>
    .acomplishment {
        width: 400px;
        display: flex;
        flex-direction: row;
        margin-bottom: 30px;
				padding-top: 10px;
    }
    .box1{
        margin-left: 87px;


    }
    .light{
        font-size: 12px;
        font-weight: 300;
        color: var(--text-color);

    }
    .light1{
        font-size: 12px;
        font-weight: 300;
        color: var(--text-color);
        margin-top: 0px;
        margin-bottom: 0px;
    }

    .bold {
        font-size: 15px;
        font-weight: 700;
        color: var(--text-color);
        margin-bottom: 0px;
        margin-top: 0px;
    }
    h1{
        margin: 0px;
    }
		h2{
				padding-top: 5px;
		}


</style>

<div class='acomplishment'>

	<h1 class='light'>{year}</h1>
	<div class='box1'>
		<h1 class='bold'>{tl1}<br>{tl2}<br>{tl3}</h1>
		<h2 class='light1'>{cl1}<br>{cl2}<br>{cl3}<br>{cl4}</h2>
	</div>


</div>