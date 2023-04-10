<template>
	<header class="Header">
		<b-container class="Header__container">
			<div class="Header__item Header__item_left">
				<span>г. Москва</span><br />
				Херсонская&nbsp;ул. 20к3
			</div>
			<div class="Header__item Header__item_left">
				<span>Время работы:</span><br />
				10:00-19:00 Ежедневно
			</div>
			<div class="Header__logo">
				<img src="/logo.png" alt="Логотип Atelietextile">
			</div>
			<div class="Header__item Header__item_right">
				<span>E-mail:</span><br />
				hometextile.mn@ya.ru
			</div>
			<div class="Header__item Header__item_right">
				<span>Номер телефона:</span><br />
				<a href="tel:+79164126914">+7 (916) 412-69-14</a>
			</div>
		</b-container>
		<Navbar class="Header__navbar" />
	</header>
</template>

<style lang="scss">
.Header {
	height: var(--header-height);
	position: relative;
	z-index: 2;
	background-color: var(--bg-color-first);

	&__container {
		height: 100%;
		display: grid;
		align-items: center;
		grid-template-columns: 2fr 2fr 4fr 2fr 2fr;
	}

	&__item,
	&__logo {
		text-align: center;

		&_left {
			text-align: left;
		}

		&_right {
			text-align: right;
		}
	}
	&__item {

		span {
			color: var(--ff-color-third);
		}
	}
	&__logo {
		height: 100%;
		position: relative;
		z-index: 3;

		img {
			position: absolute;
			top: 0; left: 50%;
			transform: translateX(-50%);
		}
	}

	&__navbar {
		width: 100%;
		position: absolute;
		top: 100%; left: 0;
	}
}
</style>
