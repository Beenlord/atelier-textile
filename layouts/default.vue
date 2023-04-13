<template>
	<div class="DefaultLayout">
		<Header />
		<Navbar />
		<Nuxt />
		<Preloader />
		<Icons />
	</div>
</template>

<script>
import Icons from '@/components/dynamic/Icons.vue';

export default {
  components: {
    Icons,
  },
  data() {
    return {
    };
  }
};
</script>

<style lang="scss">
.DefaultLayout {
	margin: 0 auto;
	.Navbar {
		position: sticky;
		top: 0;
	}
}
</style>
