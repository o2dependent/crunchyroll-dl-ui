<script lang="ts">
	import CrunchyrollLoginDialog from "./CrunchyrollLoginDialog.svelte";
	import { Button } from "bits-ui";

	let open = false;
</script>

<CrunchyrollLoginDialog bind:open />
<div class="flex flex-col justify-center items-center h-full">
	<div class="prose container mx-auto px-4 w-full py-6">
		<h1>Welcome to Lowky crunchy-cli UI</h1>
		<p>
			Enter your Crunchyroll login below to get started. All credentials will
			only be stored on your computer.
		</p>
		<Button.Root
			on:click={() => (open = true)}
			class="inline-flex h-12 items-center justify-center rounded-input bg-dark
		px-[21px] text-[15px] font-semibold text-background shadow-mini
		hover:bg-dark/95 active:scale-98 active:transition-all"
		>
			Login
		</Button.Root>
	</div>
</div>
