<script>
	import BigButton from '../_component/BigButton.svelte';
	import InputInfo from '../_component/InputInfo.svelte';
	import Message from '../_component/Message.svelte';
</script>

<style>
    .page {
        flex-direction: column;
        align-items: center;
        display: flex;

    }

    .main {

        width: 953px;
        height: 300px;

				margin-top: 25px;
				margin-bottom: 25px;
        background-color: transparent;
        display: flex;
        flex-direction: row;
        align-items: top;
        justify-content: space-between;

    }

    .row1 {

        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
    }

    .row {
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;
    }

    .title {
        margin-top: 0px;
        margin-bottom: 5px;
        font-size: 15px;
        font-weight: 700;
        padding: 0px;


    }

    .detail {
        font-size: 12px;
        font-weight: 300;
        margin: 0px;
        padding: 0px;
    }

    .bigtitle {
        margin-bottom: 5px;
        margin-top: 0px;
        font-size: 35px;
        font-weight: 700;
    }

    .l1 {
        padding-bottom: 30px;
    }

    .l2 {
        padding-bottom: 15px;
    }
		.circle{
				width: 120px;
				height: 120px;
				padding-right: 15px;
				padding-top: 15px;
		}

</style>


<div class='page'>
	<div class='main'>
		<div class='left'>
			<div class='l1'>
				<h1 class='bigtitle'>Contact</h1>
				<h2 class='detail'> Looking forward hearing from you</h2>
			</div>
			<div class='l2'>
				<h1 class='title'> Phone </h1>
				<h2 class='detail'> +989333406081 </h2>
			</div>

			<div>
				<h1 class='title'> Email </h1>
				<h2 class='detail'> mirzaei.mohammadreza1977@gmail.com </h2>
			</div>
		</div>
		<div class='right'>
			<div class='row'>
				<InputInfo />
				<InputInfo title='Last Name'/>
			</div>
			<div class='row'>
				<InputInfo title='Email*' req='required'/>
				<InputInfo  title='Subject'/>
			</div>

			<div class='row1'>
				<Message />
				<div class='circle'>
					<BigButton title='Submit' />
				</div>
			</div>

		</div>
	</div>
</div>