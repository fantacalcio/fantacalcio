<script>
	export let href = '#';
	export let text = 'Download';

	/**
	 * @type {(() => void) | null}
	 */
	export let clickAction = null;

	function handleClick() {
		if (clickAction) {
			clickAction();
		}
	}
</script>

<a
	class="group inline-block rounded-full bg-gradient-to-r from-gray-200 via-gray-300 to-gray-500 p-[2px] hover:text-white focus:outline-none focus:ring active:text-opacity-75"
	{href}
	on:click={() => handleClick()}
>
	<span
		class="block rounded-full bg-white px-8 py-3 text-sm font-medium group-hover:bg-transparent"
	>
		{text}
	</span>
</a>
