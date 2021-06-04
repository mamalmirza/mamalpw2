<script>


	import EduDet from '../_component/EduDet.svelte';
	import PubDet from '../_component/PubDet.svelte';


</script>

<style>

    .dastan {
        width: calc(100% - 478px);
        height: 43px;
        padding-top: 25px;
        padding-left: 239px;
        padding-right: 239px;
        background: transparent;
        display: flex;
        flex-direction: row;
        align-items: center;
        justify-content: space-between;

    }

    .group {
        width: calc(100% - 478px);
        padding-left: 239px;
        padding-right: 239px;
        padding-bottom: 1px;
        margin-top: 40px;
        display: flex;
        flex-direction: row;
        justify-content: space-between;
				border-bottom: 1px solid var(--gray-color);

    }
    .group1 {
        width: calc(100% - 478px);
        padding-left: 239px;
        padding-right: 239px;
        padding-bottom: 1px;
        margin-top: 40px;
        display: flex;
        flex-direction: row;
        justify-content: space-between;


    }

    h4 {
        font-size: 35px;
        font-weight: 700;
        color: var(--text-color);
        margin: 0px;
    }

    h1 {
        font-size: 20px;
        font-weight: 700;
        color: var(--text-color);
        margin: 0px;
    }

</style>


<div class='dastan'>
	<h4>Resume</h4>
	<a href='https://www.mixd.co.uk/' target='_blank'>
		<img src='download.png' alt='Download Icon'>
	</a>
</div>

<div class='main'>


<div class='group'>
	<h1>Education</h1>
	<div>
		<EduDet year='2021 - Present' tl1='Univesity of Regina | ' tl2='Master of Applied Sience' />
		<EduDet year='2015 - 2020' tl1='K.N. Toosi University of Technology | ' tl2='Bachelor’s Degree' />
	</div>
</div>

<div class='group'>
	<h1>Publication</h1>
	<div>
		<PubDet year='2020' tl1='An Open-Source Motion Planning' tl2='Algorithm for Semi-Autonomous'
						tl3='Rescue Robots in RoboCup'
						cl1='M. R. Mirzaei, N. Karimi, E. Najafi |' cl2='21st International Conference on Research and'
						cl3='Education in Mechatronics (REM). Cracow. Poland.' />

	</div>
</div>

<div class='group'>
	<h1>Experince</h1>
	<div>
		<EduDet year='2021 - Present' tl1='Research Assistant'
						cl1='Dastan Lab |' cl2='University of Regina' />
		<EduDet year='2019 - 2021' tl1='Research Assistant '
						cl1='Dr. Esmaeil Najafi’s Research Group |' cl2='K. N. Toosi University of Technology' />
		<EduDet year='2019 - 2021' tl1='Research Assistant '
						cl1='Dr. Mohammad Ravanidi’s Lab |' cl2='K. N. Toosi University of Technology' />
		<EduDet year='2016 - 2019' tl1='Research Assistant '
						cl1='KN2C Lab |' cl2='K. N. Toosi University of Technology' />

	</div>
</div>

<div class='group'>
	<h1>Honors</h1>
	<div>
		<PubDet year='2018' tl1='3rd Place, RoboCup Asia Pacific'
						cl1='Real Rescue Robots League |' cl2='Iran' />
		<PubDet year='2018' tl1='3rd Place, RoboCup Iran Open'
						cl1='Real Rescue Robots League |' cl2='Iran' />
		<PubDet year='2018' tl1='Best in Class innovation, RoboCup Iran Open'
						cl1='Real Rescue Robots League |' cl2='Iran' />
		<PubDet year='2017' tl1='5th Place, RoboCup'
						cl1='Real Rescue Robots League |' cl2='Japan' />
		<PubDet year='2017' tl1='3rd Place, RoboCup Iran Open'
						cl1='Real Rescue Robots League |' cl2='Iran' />

	</div>
</div>

<div class='group1'>
	<h1>VOLUNTEER & Extra-curricular</h1>
	<div>
		<PubDet year='2021' tl1='Executive Committee'
						cl1='The 29th Annual International Conference of the' cl2='Iranian Association of Mechanical Engineers |' cl3='Iran' />
		<PubDet year='2019' tl1='Executive Committee'
						cl1='International Nasircup 2019 Competition |' cl2='Iran' />
		<PubDet year='2019' tl1='Executive Committee'
						cl1='The 7TH International Conference on E-Learning ' cl2='E-Teaching |' cl3='Iran' />
		<PubDet year='2019' tl1='Executive Committee'
						cl1='2nd K.N.Toosi University Bussines School |' cl2='Iran' />
		<PubDet year='2017' tl1='Central Council of Film & '  tl2= 'Photography of University'
						cl1='K. N. Toosi University of Technology |' cl2='Japan' />


	</div>
</div>


</div>


