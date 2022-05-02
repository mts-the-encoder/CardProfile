<template>
    <div class="wrapper">
	<div class="lista-item">
		<input class="trigger-input" id="faq-titulo-1" type="checkbox">
		<div class="trigger-wrapper">
			<label for="faq-titulo-1">
				<h2 class="faq-titulo">Soft Skills</h2>
			</label>
			<p class="faq-conteudo">Lorem ipsum dolor sit amet consectetur adipisicing elit. Cumque eligendi vero in dolorum similique perspiciatis dolor placeat aut reiciendis, ducimus atque doloremque, sed consequatur! Voluptatum soluta harum provident quia maiores?.</p>
		</div>
	</div>
	
	<div class="lista-item">
		<input class="trigger-input" id="faq-titulo-2" type="checkbox">
		<div class="trigger-wrapper">
			<label for="faq-titulo-2">
				<h2 class="faq-titulo">Hard Skills</h2>
			</label>
			<p class="faq-conteudo">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ad ab placeat molestias libero sit animi itaque doloremque magni nesciunt, dignissimos quos minus ratione perferendis, eum, consequuntur a cumque accusantium accusamus..</p>
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
}

.lista-item {
    width: 200px;
	background: $black;
	border-radius: 4px;
	margin-bottom: 20px;
	padding: 10px;
	box-shadow: 0 2px 6px rgba(50,50,90,.1);
}

.faq-titulo {
	cursor: pointer;
	padding: 10px;
	font-size: 1.4em;
	font-family: monospace;
	color: $white;
}

.faq-titulo::before {
	content: '';
	display: inline-block;
	height: 12px;
	width: 24px;
	margin-right: 10px;
	background: $white;
}

.faq-titulo::after {
	content: '+';
	float: right;
	transition: transform .3s ease;
}

.faq-conteudo {
    background-color: $black;
	padding: 10px;
	color: $gold;
	font-family: Helvetica;
	font-size: .875em;
	line-height: 1.4em;
	display: none;
}

.trigger-input {
	display: none;
}

.trigger-input:checked + .trigger-wrapper .faq-conteudo {
	display: block;
}

.trigger-input:checked + .trigger-wrapper .faq-titulo::after {
	transform: rotate(45deg) scale(1.08);
}
</style>