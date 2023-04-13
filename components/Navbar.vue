<template>
	<nav class="Navbar">
		<b-container class="Navbar__container">
			<ul class="Navbar__side Navbar__side_left">
				<li><a href="/">Главная</a></li>
				<li><a href="/">Ассортимент</a></li>
				<li><a href="/">Все товары</a></li>
			</ul>
			<ul class="Navbar__side Navbar__side_right">
				<li><a href="/">Портфолио</a></li>
				<li><a href="/">Контакты</a></li>
				<li><a href="/">Заказать</a></li>
			</ul>
		</b-container>
	</nav>
</template>

<style lang="scss">
.Navbar {
	background: var(--lg-color-first);

	&__container {
		height: calc(var(--header-height) / 1.5);
		display: flex;
		align-items: center;
		justify-content: space-between;
	}

	&__side {
		display: flex;

		li {
			list-style: none;
			white-space: nowrap;
		}

		a {
			color: var(--ff-color-fifth);
		}

		&_left {
			li {
				margin-right: 2rem;
			}
		}
		&_right {
			li {
				margin-left: 2rem;
			}
		}
	}
}
@media screen and (max-width: 1000px) {
	.Navbar {
		&__container {
			justify-content: flex-end;
		}
		&__side li {
			margin-left: 2rem;
			margin-right: 0;
		}
	}
}
@media screen and (max-width: 580px) {
	.Navbar {
		&__side:last-child {
			display: none;
		}
	}
}
</style>
