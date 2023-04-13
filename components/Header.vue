<template>
	<header class="Header">
		<b-container class="Header__container">
			<div class="Header__item Header__item_left">
				<span>г. Москва</span><br />
				<a href="https://yandex.ru/maps/-/CCU8A-d~oA" target="_blank">Херсонская&nbsp;ул. 20к3</a>
			</div>
			<div class="Header__item Header__item_left">
				<span>Время работы:</span><br />
				<div>10:00-19:00 Ежедневно</div>
			</div>
			<!--<div class="Header__logo">-->
			<!--	<img src="logo.png" alt="Логотип Atelietextile">-->
			<!--</div>-->
			<div class="Header__item Header__item_right">
				<span>E-mail:</span><br />
				<div>hometextile.mn@ya.ru</div>
			</div>
			<div class="Header__item Header__item_right">
				<span>Номер телефона:</span><br />
				<a href="tel:+79164126914">+7 (916) 412-69-14</a>
			</div>
		</b-container>
	</header>
</template>

<style lang="scss">
.Header {
	width: 100%;
	height: var(--header-height);
	position: relative;
	z-index: 2;
	background-color: var(--bg-color-first);

	&__container {
		height: 100%;
		display: grid;
		align-items: center;
		grid-template-columns: 2fr 4fr 4fr 2fr;
		grid-gap: 1.5rem;
	}

	&__item,
	&__logo {
		width: 100%;
		text-align: center;

		&_left {
			text-align: left;
		}

		&_right {
			text-align: right;
		}
	}

	&__item {
		* {
			font-family: var(--font-philosopher);
			color: var(--ff-color-first);
			text-decoration: none;
			white-space: nowrap;
		}
		span {
			font-size: 1.5rem;
			line-height: 1;
			color: var(--ff-color-third);
		}
		a {
			&:hover {
				color: var(--ff-color-first);
			}
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
}
@media screen and (max-width: 1000px) {
	.Header {
		&__container {
			grid-template-columns: 2fr 2fr;
		}
		&__item:nth-child(2),
		&__item:nth-child(3) {
			display: none;
		}
	}
}
@media screen and (max-width: 580px) {
	.Header {
		&__container {
			grid-template-columns: 2fr;
		}
		&__item:not(:last-child) {
			display: none;
		}
	}
}
</style>
