<script lang="ts">
	export let text: string;
	export let icon: string;
	export let link: string | null;
</script>

<i class="bi-{icon}"></i>
<span
	class="{link && 'underline'}
			print:no-underline">{text}</span
>
