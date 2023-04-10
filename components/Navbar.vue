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
		display: flex;
		justify-content: space-between;
	}

	&__side {
		display: flex;
		padding: 12px 0;

		li {
			list-style: none;
		}

		a {
			color: var(--ff-color-fifth);
		}

		&_left {
			li {
				margin-right: 12px;
			}
		}
		&_right {
			li {
				margin-left: 12px;
			}
		}
	}
}
</style>
