<script>
	import { TreeBranch, TreeLeaf, TreeView } from '../lib/index';
</script>

<h1>Welcome to SvelteKit</h1>
<TreeView lineColor="gray" iconBackgroundColor="gray" iconColor="white" branchHoverColor="blue">
	<TreeBranch rootContent="Languages">
		<TreeLeaf>C#/.NET</TreeLeaf>
		<TreeBranch>
			<TreeLeaf>C#/.NET</TreeLeaf>
			<TreeLeaf>
				<span class="tree_label">C#/.NET</span>
			</TreeLeaf>
			<TreeBranch rootContent="Languages">
				<TreeLeaf>C#/.NET</TreeLeaf>
				<TreeBranch>
					<TreeLeaf>C#/.NET</TreeLeaf>
					<TreeLeaf>
						<span class="tree_label">C#/.NET</span>
					</TreeLeaf>
				</TreeBranch>
				<TreeLeaf><span class="tree_label">C#/.NET</span></TreeLeaf>
			</TreeBranch>
		</TreeBranch>
		<TreeLeaf><span class="tree_label">C#/.NET</span></TreeLeaf>
	</TreeBranch>
	<TreeBranch defaultClosed>
		<TreeLeaf><span class="tree_label">C#/.NET</span></TreeLeaf><TreeLeaf
			><span class="tree_label">C#/.NET</span></TreeLeaf
		><TreeLeaf><span class="tree_custom">Specified tree item view</span></TreeLeaf>
	</TreeBranch>
</TreeView>

<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>
