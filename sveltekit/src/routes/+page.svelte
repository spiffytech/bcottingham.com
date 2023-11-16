<script lang="ts">
	import '../../node_modules/bootstrap-icons/font/bootstrap-icons.min.css';

	import HeaderItem from './header_item.svelte';
</script>

<div class="mx-4 my-2">
	<div class="flex items-baseline gap-x-8">
		<h1 class="font-rh text-3xl">Brian Cottingham</h1>
		<span class="font-src-sans">
			<HeaderItem
				icon="envelope-at"
				text="brian@bcottingham.com"
				link="mailto:brian@bcottingham.com"
			/>
			| <HeaderItem icon="telephone" text="919-259-8970" link="tel:+1-919-259-8970" />
			| <HeaderItem
				icon="braces"
				text="github.com/spiffytech"
				link="https://github.com/spiffytech"
			/>
			| <HeaderItem icon="pen" text="spiffy.tech" link="https://spiffy.tech" />
		</span>
	</div>
</div>
