<script lang="ts">
	import Navbar from "$lib/components/core/Navbar.svelte";
	import type { IMenu } from "$lib/types/core";

	let menus: IMenu[] = []
</script>

<div class="map">
	<Navbar menus={menus} name={"map"} color={"green"}/>
	<div class="content">
  		<slot />
	</div>
</div>

<style>
	.map {
		width: 100%;
	}
</style>
