<script>
  import ButtonBase from "./components/ButtonBase.svelte";
</script>

<main class="main-content" id="app">
	<header>
		<div class="container">
			<div class="navigation">
				<div class="nav-logo">
					<div class="nav-logo__img">
						<img
							src="/assets/imgs/logo.svg"
							alt="2Eat logo - an icon of a store"
						/>
					</div>
				</div>
				<div class="navigation">
					<!-- <div class="pure-u-4"><button on:click={changeState}>Поменять состояние(кнопки тут не будет)</button></div> -->
					<ul>
						<li><a href="/">О проекте</a></li>
						<li><a href="/">Вопросы и ответы</a></li>
						<li><a href="/">Вход</a></li>
					</ul>
				</div>
			</div>
		</div>
	</header>
	<section class="choose-location">
		<div class="container">
			<div class="choose-location__info">
				<h2>Куда можно сходить</h2>
				<ButtonBase>Найти место</ButtonBase>
			</div>
		</div>
	</section>
	<footer>
		<div class="container">
			<div class="footer">
				<div class="footer__social">
					<a href="/"><img src="/assets/imgs/social/vk.svg" alt=""></a>
					<a href="/"><img src="/assets/imgs/social/instagram.svg" alt=""></a>
					<a href="/"><img src="/assets/imgs/social/telegram.svg" alt=""></a>
				</div>
				<div class="footer__info">
					<ul>
						<li><a href="/">Связаться с нами</a></li>
						<li><a href="/">Пользовательское соглашение</a></li>
					</ul>
				</div>
			</div>
		</div>
	</footer>
</main>

<style type="text/scss">
main {
	max-height: 1vh;
}
header {
	max-height: 90px;
}
.container {
	width: 1110px;
	margin: 0 auto;
}
.navigation  {
	min-width: 72px;
	display: flex;
	align-items: center;
	justify-content: space-between;
	padding: 18px 0;
	font-family: 'Proxima Nova Semibold';

	.nav-logo {
    max-width: 136px;
	}

	ul {
		list-style: none;
		display: flex;
		align-content: center;
		justify-content: space-between;
	}
	li {
		margin-right: 40px;

		&:nth-child(3) {
			margin-right: 16px;
		}
	}
	a {
		text-decoration: none;
		color: #121212;
	}
}
.choose-location {
	margin-top: 92px;
	display: flex;
	flex-direction: column;

	&__info {
		display: flex;
		justify-content: space-between;
		align-items: center;

		h2 {
			font-size: 32px;
			line-height: 40px;
			font-family: 'Proxima Nova Bold';
		}
	}

	

}
.footer {
	margin-top: 700px;
	display: flex;
	justify-content: space-between;
	align-items: center;
	&__social {
		&:not(last-child) {
			margin-right: 12px;
		}
	}
	&__info {
		font-family: 'Proxima Nova Semibold';
		font-size: 16px;

		ul {
			display: flex;
			list-style: none;
		}

		li {
			&:not(:last-child) {
				margin-right: 32px;
			}
		}

		a {
			color: #121212;
			text-decoration: none;
		}
		
	}
}
</style>
