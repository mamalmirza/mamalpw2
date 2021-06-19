<script>
	import PubDet from '../_component/PubDet.svelte';
	import ProjectDet from '../_component/ProjectDet.svelte';
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
    h4 {
        font-size: 35px;
        font-weight: 700;
        color: var(--text-color);
        margin: 0px;
    }
</style>



<div class='dastan'>
	<h4>Projects</h4>

</div>

<ProjectDet title='Camera Dolly' cl1='Designing a camera dolly with a hydraulic manipulator.'
						photo='Dolly.png'/>
<ProjectDet title='Sub-sea Wire Saw' cl1='Designing a sub-sea wire saw for sub-sea pipe maintenance.'
						photo='Sub.png'/>
<ProjectDet title='Motion Planner of a Mobile Robot in a Partially Observable Environment'
						cl1='Modeling motion planning problem for a mobile robot in an unknown environment.'
						photo='Motion.png'/>
<ProjectDet title='Rescue Robot'  cl1='Designing the chassis of a rescue robot for RoboCup Rescue Competitions.'
						photo='Arta.png'/>
<ProjectDet title='Smart Pill Box' cl1='Designing a pill box to remind dementia patients to take their pills.'/>
<ProjectDet title='Self-Stabilizing Spoon' cl1='Designing a spoon to control the hand vibration of dementia patients.'/>

