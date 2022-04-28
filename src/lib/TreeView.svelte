<script>
	export let lineColor = '#e7e7e7';
	export let iconBackgroundColor = '#ffffff';
	export let iconColor = '#c2c2c2';
	export let branchHoverColor = '#cccccc';
</script>

<ul
	class="tree"
	style="--line-color: {lineColor}; --icon-background-color:{iconBackgroundColor}; --icon-color:{iconColor}; --branch-hover-color:{branchHoverColor}"
>
	<slot />
</ul>

<style>
	.tree {
		margin: 1em;
		box-sizing: content-box;
	}

	.tree :global(ul) {
		list-style-type: none;
		margin: 0;
		padding: 0;
	}

	.tree :global(ul li) {
		padding: 1em 0 0 1em;
	}

	.tree > :global(li:last-child) {
		padding-bottom: 0;
	}

	.tree :global(li:last-child:before) {
		height: 1em;
		bottom: auto;
	}

	.tree > :global(li:last-child:before) {
		display: none;
	}

	/* ————————————————————–
    Tree branches
    */
	.tree :global(.tree_label:after) {
		position: absolute;
		top: 0;
		left: -1.5em;
		display: block;
		height: 0.5em;
		width: 1em;
		border-bottom: 2px solid var(--line-color);
		border-left: 2px solid var(--line-color);
		border-radius: 0 0 0 0.3em;
		content: '';
	}

	.tree :global(li:before) {
		position: absolute;
		top: 0;
		bottom: 0;
		left: -0.5em;
		display: block;
		width: 0;
		border-left: 2px solid var(--line-color);
		content: '';
	}
</style>
