<script></script>

<div class="container">
	<div class="first-block">
		<div class="left-side">
			<div class="title">
				<p>Дизайнер одежды</p>
				<h1>Динара Галимова</h1>
			</div>
			<div class="description">
				<h3>
					Lorem ipsum dolor sit amet, consectetur adipisicing elit. Saepe ad corrupti doloremque
					ullam. Corporis adipisci, dolor neque ex repudiandae aperiam.
				</h3>
			</div>

			<div class="button">
				<a class="hover">Подробнее</a>
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
</div>

<style>
	h3 {
		margin: 0 !important; /* Отрицательный отступ между заголовком и текстом */
	}
	.container {
		font-family: 'Cormorant SC', serif;
	}
	.first-block {
		background: url('../images/slide.jpg') no-repeat;
		padding: 50px 40px;
		background-size: 100%;
		height: 100vh;
		display: flex;
		color: #e5dfdf;
		align-items: center;
	}

	.left-side {
		width: 440px;
	}

	.title p {
		font-size: 28px;
		margin: 0;
	}
	.title {
		width: 600px;
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
		padding: 5px 10px;
		border: 8px solid;
		border-radius: 11px;
		-webkit-mask: conic-gradient(from 180deg at top 8px right 8px, #0000 90deg, #000 0)
				var(--_i, 200%) 0 /200% var(--_i, 8px) border-box no-repeat,
			conic-gradient(at bottom 8px left 8px, #0000 90deg, #000 0) 0 var(--_i, 200%) / var(--_i, 8px)
				200% border-box no-repeat,
			linear-gradient(#000 0 0) padding-box no-repeat;
		transition: 0.3s, -webkit-mask-position 0.3s 0.3s;
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
</style>
