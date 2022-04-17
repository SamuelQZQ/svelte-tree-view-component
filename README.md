# [svelte-tree-view-component](https://github.com/SamuelQZQ/svelte-tree-view-component) [![version](https://img.shields.io/npm/v/svelte-tree-view-component?style=flat-square)](https://www.npmjs.com/package/svelte-tree-view-component) [![package minified size](https://img.shields.io/bundlephobia/min/svelte-tree-view-component?style=flat-square&color=important)](https://bundlephobia.com/result?p=svelte-tree-view-component) [![package size](https://img.shields.io/bundlephobia/minzip/svelte-tree-view-component?style=flat-square)](https://bundlephobia.com/result?p=svelte-tree-view-component)

A beautiful and easy to use Tree View component for Svelte.

## **[REPL Demo](https://svelte.dev/repl/8b1d026ca6e845bc83bffa5781a519ca?version=3.47.0)**

Screenshot:

![](https://raw.githubusercontent.com/SamuelQZQ/svelte-tree-view-component/main/screeshot.gif)

## Install
```
npm i svelte-tree-view-component
```

## How to use

### Basic usage
```jsx
<TreeView >
    <TreeBranch rootContent="Languages">
        <TreeLeaf>JavaScript</TreeLeaf>
        <TreeLeaf>C#</TreeLeaf>
    </TreeBranch>
    <TreeBranch rootContent="Frameworks">
        <TreeLeaf>Svelte</TreeLeaf>
        <TreeLeaf>React</TreeLeaf>
    </TreeBranch>
</TreeView>
```

### Nested branch
```jsx
<TreeView >
    <TreeBranch rootContent="Languages">
        <TreeLeaf>JavaScript</TreeLeaf>
        <TreeBranch rootContent="Frameworks">
            <TreeLeaf>Svelte</TreeLeaf>
            <TreeLeaf>React</TreeLeaf>
        </TreeBranch>
    </TreeBranch>
</TreeView>
```

### Customized leaf
```jsx
<TreeView >
    <TreeBranch rootContent="Languages">
        <TreeLeaf><div style="color:red;">Red</div></TreeLeaf>
    </TreeBranch>
</TreeView>
```

### Customized branch
```jsx
<TreeView >
    <TreeBranch >
        <div style="color:red;" slot="root">Red</div>
        <svelte:fragment slot="children">
            <TreeLeaf>Svelte</TreeLeaf>
            <TreeLeaf>React</TreeLeaf>
        </svelte:fragment>
    </TreeBranch>
</TreeView>
```

### Change colors/Theme
```jsx
<TreeView     
    lineColor="#ff0000"
    iconBackgroundColor="#ff0000"
    iconColor="#000000"
    branchHoverColor="#ff0000">
    <TreeBranch rootContent="Languages">
        <TreeLeaf>JavaScript</TreeLeaf>
        <TreeLeaf>C#</TreeLeaf>
    </TreeBranch>
</TreeView>
```

## Reference
- [Codepen: Pure CSS Tree Menu](https://codepen.io/bisserof/pen/nrMveb)