<template>
    <div class="wrapper">
	<div class="item--list">
		<input class="trigger--input" id="title--one" type="checkbox">
		<div class="trigger-wrapper">
			<label for="title--one">
				<h2 class="skills--title">Soft Skills</h2>
			</label>
			<ul class="content--sk">
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
			</ul>
		</div>
	</div>
	
	<div class="item--list">
		<input class="trigger--input" id="title--two" type="checkbox">
		<div class="trigger-wrapper">
			<label for="title--two">
				<h2 class="skills--title">Hard Skills</h2>
			</label>
			<ul class="content--sk list">
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
				<li>lorem.</li>
			</ul>
		</div>
	</div>
</div>
</template>

<script>
    export default {
    name: "Trigger",
};
</script>

<style lang="scss" scoped>
.wrapper {
	width: 500px;
    display: flex;
    justify-content: space-evenly;
    align-items: center;

	.item--list {
		position: relative;
		width: 200px;
		background: $black;
		border-radius: 5px 20px 5px 20px;
		margin-bottom: 20px;
		padding: 10px;
		box-shadow: 0 2px 6px rgba(50,50,90,.1);
		border: 2px solid $gold;

		.skills--title {
			cursor: pointer;
			padding: 10px;
			font-size: 18px;
			color: $white;
		}

		.skills--title::before {
			content: '';
			display: inline-block;
			height: 12px;
			width: 24px;
			margin-right: 10px;
			background: $gold;
		}

		.skills--title::after {
			content: '+';
			float: right;
			transition: transform .3s ease;
			color: $gold;
		}

		.content--sk {
			background-color: $black;
			padding: 10px;
			color: $gold;
			font-size: 15px;
			line-height: 1.4em;
			display: none;
			transition: opacity 4s ease-out;
			list-style: none;
			text-align: center;
		}

		.trigger--input {
			display: none;
		}

		.trigger--input:checked + .trigger-wrapper .content--sk {
			opacity: 1;
			display: block;
		}

		.trigger--input:checked + .trigger-wrapper .skills--title::after {
			transform: rotate(45deg) scale(1.08);
		}

	}
}
/*MOBILE*/
@media (max-width: 425px){
	.wrapper {
		width: 100%;
		margin: 0 auto;
		display: flex;
		align-items: center;
		justify-content: space-evenly;
		
		.item--list {
			width: 180px;
			display: flex;
		}
		.trigger-wrapper {
			display: flex;
			text-align: center;
			
			.skills--title {
				font-size: 13px;
				width: 100%;
				
			}
			.skills--title::after{
				font-size: 15px;
				
				vertical-align: middle;
			}
			.skills--title::before{
				vertical-align: middle;
				
			}
			.content--sk {
				margin-right: 40px;
			}
		}
	}
}
</style>