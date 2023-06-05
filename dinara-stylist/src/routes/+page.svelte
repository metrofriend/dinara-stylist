<script>
	let innerWidth;
	function onSubmit(token) {
		document.getElementById('demo-form').submit();
	}
</script>

<svelte:window bind:innerWidth />
<div class="container">
	<div class="first-block">
		<header>
			<div class="header-nav">
				<a href="">Обо мне</a>
				<a href="">Портфолио</a>
				<div class="logo">
					<h3>Dinara style</h3>
				</div>
				<a href="">Связаться со мной</a>
				<a href="">Контакты</a>
			</div>
		</header>
		<div class="content">
			<div class="content-content">
				<div class="content-text">
					<div class="title">
						<p>Стилист</p>
						<h1>Динара Галимова</h1>
					</div>
					<div class="content-description">
						<h3>
							Lorem ipsum dolor sit amet, consectetur adipisicing elit. Saepe ad corrupti doloremque
							ullam. Corporis adipisci, dolor neque ex repudiandae aperiam.
						</h3>
					</div>
					{#if innerWidth < 1000}
						<div class="button">
							<a class="" href="#">Подробнее</a>
						</div>
					{:else}
						<div class="button">
							<a class="hover" href="#">Подробнее</a>
						</div>
					{/if}
				</div>
			</div>
		</div>
	</div>
	<div class="main">
		<div class="achievements">
			<div class="text-block">
				<h3 class="number">100+</h3>

				<p class="text-desc">проектов сделано</p>
			</div>
			<div class="text-block">
				<h3 class="number">100+</h3>

				<p class="text-desc">проектов сделано</p>
			</div>
			<div class="text-block">
				<h3 class="number">100+</h3>

				<p class="text-desc">проектов сделано</p>
			</div>
			<div class="text-block">
				<h3 class="number">100+</h3>

				<p class="text-desc">проектов сделано</p>
			</div>
		</div>
		<div class="quote">
			<div class="quote-desc">
				<h4>// Клиент сказал</h4>
				<h2>
					" Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum, pariatur. Voluptatibus ex
					quod maiores quibusdam quae odio dolor voluptates enim. "
				</h2>
				<p>- Иван Иванов. Владелец магазина</p>
			</div>
			<div class="quote-image">
				<!-- ДОДЕЛАТЬ -->
				<img src="" alt="" />
				<!-- ДОДЕЛАТЬ -->
			</div>
		</div>
		<div class="separator" />

		<div class="formbold-form-wrapper">
			<h3 class="form-title">Записаться на разбор гардероба</h3>
			<form action="" method="POST" class="mt-30">
				<div class="formbold-mb-5">
					<label for="name" class="formbold-form-label"> Имя Фамилия </label>
					<input
						type="text"
						name="name"
						id="name"
						placeholder="Иван Иванов"
						class="formbold-form-input"
					/>
				</div>
				<div class="formbold-mb-5">
					<label for="phone" class="formbold-form-label"> Номер телефона </label>
					<input
						type="text"
						name="phone"
						id="phone"
						placeholder="+7 111 111 11 11"
						class="formbold-form-input"
					/>
				</div>

				<div class="formbold-mb-5 formbold-pt-3">
					<label class="formbold-form-label-spec formbold-form-label-2">
						Назначьте время звонка
					</label>
					<p class="form-subtitle">
						Менеджр позвонит Вам в удобное для вас время чтобы записать вас на прием
					</p>
					<div class="flex flex-wrap formbold--mx-3">
						<div class="w-full sm:w-half formbold-px-3">
							<div class="formbold-mb-5 w-full">
								<label for="date" class="formbold-form-label"> Число </label>
								<input type="date" name="date" id="date" class="formbold-form-input" />
							</div>
						</div>
						<div class="w-full sm:w-half formbold-px-3">
							<div class="formbold-mb-5">
								<label for="time" class="formbold-form-label"> Время </label>
								<input type="time" name="time" id="time" class="formbold-form-input" />
							</div>
						</div>
					</div>
				</div>

				<div>
					<button class="formbold-btn">Записаться</button>
				</div>
			</form>
		</div>
	</div>
</div>

<style>
	/* TOOLS */
	.mt-30 {
		margin-top: 30px;
	}

	a {
		color: #fff;
		text-decoration: none;
	}
	/* TOOLS */

	a {
		text-decoration: none;
	}
	h3 {
		margin: 0 !important; /* Отрицательный отступ между заголовком и текстом */
	}
	.container {
		font-family: 'Cormorant SC', serif;
	}

	header {
		display: flex;
		align-items: center;
		color: #fff;
		font-size: 18px;
		padding: 30px 200px;
		justify-content: space-between;
		background: #000000;
		opacity: 0.7;
	}
	.header-nav {
		display: flex;
		justify-content: space-between;
		flex-grow: 1;
	}
	/* .header-nav a {
		color: #fff;
	} */
	.first-block {
		background: url('../images/slide.jpg') no-repeat;
		background-size: 100%;
		height: 100vh;
	}

	.content {
		display: flex;
		align-items: center;
		height: calc(100%-80px);
	}

	.content-content {
		color: #ffffff;
		padding: 50px 140px;
	}

	.content-text {
		width: 60%;
	}
	.content-description {
		width: 65%;
	}

	.title p {
		font-size: 24px;
		margin: 0;
		width: 20%;
		font-weight: 800;
	}
	.title {
	}
	.title h1 {
		font-size: 72px;
		margin: 0 !important;
		padding: 0 !important;
	}

	.button {
		margin-top: 60px;
	}
	.hover {
		font-size: 28px;
		font-weight: 800;
		padding: 5px 10px;
		color: #fff;
		border: 1px solid;
		border-color: #cc9966;
		border-radius: 11px;
		-webkit-mask: conic-gradient(from 180deg at top 8px right 8px, #0000 90deg, #000 0)
				var(--_i, 200%) 0 /200% var(--_i, 8px) border-box no-repeat,
			conic-gradient(at bottom 8px left 8px, #0000 90deg, #000 0) 0 var(--_i, 200%) / var(--_i, 8px)
				200% border-box no-repeat,
			linear-gradient(#000 0 0) padding-box no-repeat;
		/* transition: 0.1s, -webkit-mask-position 0.3s 0.3s; */
		animation: move 5s infinite;
	}
	.hover:hover {
		--_i: 100%;
		transition: 0.3s, -webkit-mask-size 0.3s 0.3s;
	}

	/* MAIN */

	.achievements {
		display: flex;
		justify-content: space-around;
		align-items: center;
		padding: 50px 0px;
	}

	.text-block .number {
		font-size: 64px;
		font-weight: 600;
	}

	/* QUOTE */

	.quote {
		padding: 50px 40px;
		background: #000;
		color: #fff;
	}

	.quote-desc {
		width: 65%;
	}

	.separator {
		height: 2px;
		background-color: #000;
		width: 80%;
		margin: 0 auto;
		margin-top: 30px;
	}

	/*  */

	.form-title {
		font-size: 36px;
		text-align: center;
	}

	.form-subtitle {
		margin-top: 5px;
		font-size: 14px;
		margin-bottom: 20px;
	}
	.formbold-mb-5 {
		margin-bottom: 20px;
	}
	.formbold-pt-3 {
		padding-top: 12px;
	}
	.formbold-main-wrapper {
		display: flex;
		align-items: center;
		justify-content: center;
		padding: 48px;
	}

	.formbold-form-wrapper {
		margin: 0 auto;
		margin-top: 40px;
		max-width: 550px;
		width: 100%;
		background: white;
	}
	.formbold-form-label {
		display: block;
		font-weight: 500;
		font-size: 16px;
		color: #07074d;
		margin-bottom: 12px;
	}

	.formbold-form-label-spec {
		display: block;
		font-weight: 500;
		font-size: 16px;
		color: #07074d;
	}
	.formbold-form-label-2 {
		font-weight: 600;
		font-size: 20px;
	}

	.formbold-form-input {
		width: 100%;
		padding: 12px 24px;
		border-radius: 6px;
		border: 1px solid #e0e0e0;
		background: white;
		font-weight: 500;
		font-size: 16px;
		color: #6b7280;
		outline: none;
		resize: none;
	}
	.formbold-form-input:focus {
		border-color: #cc9966;
		box-shadow: 0px 3px 8px rgba(0, 0, 0, 0.05);
	}

	.formbold-btn {
		text-align: center;
		font-size: 16px;
		border-radius: 6px;
		padding: 14px 32px;
		border: none;
		font-weight: 600;
		background-color: #cc9966;
		color: white;
		width: 100%;
		cursor: pointer;
	}
	.formbold-btn:hover {
		box-shadow: 0px 3px 8px rgba(0, 0, 0, 0.05);
	}

	.formbold--mx-3 {
		margin-left: -6px;
		margin-right: -6px;
	}
	.formbold-px-3 {
		padding-left: 12px;
		padding-right: 12px;
	}
	.flex {
		display: flex;
	}
	.flex-wrap {
		flex-wrap: wrap;
	}
	.w-full {
		width: 100%;
	}
	@media (min-width: 540px) {
		.sm\:w-half {
			width: 50%;
		}
	}
</style>
