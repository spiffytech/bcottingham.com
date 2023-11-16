<script lang="ts">
	import HeaderItemInner from './header_item_inner.svelte';

	export let text: string;
	export let icon: string;
	export let link: string | null;

	$: linkTagOpen = link ? `<a href="${link}" class="whitespace-nowrap">` : '';
	$: linkTagClose = link ? `</a>` : '';
</script>

{#if link}
	<a href={link} class="whitespace-nowrap">
		<HeaderItemInner {text} {icon} {link} />
	</a>
{:else}
	<HeaderItemInner {text} {icon} {link} />
{/if}
