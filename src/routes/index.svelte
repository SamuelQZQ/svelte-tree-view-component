<script>
	import { TreeBranch, TreeLeaf, TreeView } from '../lib/index';
</script>

<TreeView>
    <TreeBranch rootContent="Languages">
		<TreeLeaf>JavaScript</TreeLeaf>
		<TreeLeaf>C#</TreeLeaf>
	</TreeBranch>
	<TreeBranch rootContent="Frameworks">
		<TreeLeaf>Svelte</TreeLeaf>
		<TreeLeaf>React</TreeLeaf>
	</TreeBranch>
</TreeView>
<h1>Welcome to SvelteKit</h1>
<TreeView>
	<TreeBranch rootContent="Languages">
		<TreeLeaf>JavaScript/Typescript</TreeLeaf>
		<TreeLeaf>C#/.NET</TreeLeaf>
		<TreeBranch rootContent="Rust">
			<TreeLeaf>project</TreeLeaf>
			<TreeLeaf>
				<span style="color:red">project 2</span>
			</TreeLeaf>
			<TreeBranch rootContent="project 3">
				<TreeLeaf>Detail 1</TreeLeaf>
				<TreeLeaf>Detail 2</TreeLeaf>
			</TreeBranch>
		</TreeBranch>
		<TreeLeaf>C++</TreeLeaf>
	</TreeBranch>
	<TreeBranch defaultClosed rootContent="Close by default">
		<TreeLeaf>Svelte</TreeLeaf>
		<TreeLeaf>Vue</TreeLeaf>
		<TreeLeaf>React</TreeLeaf>
	</TreeBranch>
</TreeView>

<p>
	Visit <a href="https://github.com/SamuelQZQ/svelte-tree-view-component"
		>github.com/SamuelQZQ/svelte-tree-view-component</a
	> to read the documentation
</p>

<style>
	:global(body) {
		background: #2a2a2a;
		color: white;
	}
</style>
