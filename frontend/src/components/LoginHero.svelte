<script lang="ts">
	import CrunchyrollLoginDialog from "./CrunchyrollLoginDialog.svelte";
	import { Button } from "bits-ui";

	let open = false;
</script>

<CrunchyrollLoginDialog bind:open />
<Button.Root
	on:click={() => (open = true)}
	class="inline-flex h-12 items-center justify-center rounded-input bg-dark
  px-[21px] text-[15px] font-semibold text-background shadow-mini
  hover:bg-dark/95 active:scale-98 active:transition-all"
>
	Login
</Button.Root>
