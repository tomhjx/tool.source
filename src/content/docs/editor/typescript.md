---
title: "TypeScript Editor"
---

## Rich TypeScript IntelliSense, Validation


{{<

<div id="editorcontainer" class="td-box--height-full border w-100" ></div>

<link data-name="vs/editor/editor.main" rel="stylesheet" href="https://microsoft.github.io/monaco-editor/node_modules/monaco-editor/min/vs/editor/editor.main.css" />
<script>
    var require = { paths: { vs: 'https://microsoft.github.io/monaco-editor/node_modules/monaco-editor/min/vs' } };
</script>
<script src="https://microsoft.github.io/monaco-editor/node_modules/monaco-editor/min/vs/loader.js"></script>
<script src="https://microsoft.github.io/monaco-editor/node_modules/monaco-editor/min/vs/editor/editor.main.nls.js"></script>
<script src="https://microsoft.github.io/monaco-editor/node_modules/monaco-editor/min/vs/editor/editor.main.js"></script>

<script>
    $(function(){
        var editor = monaco.editor.create(document.getElementById("editorcontainer"), {
            value: ['function x() {', '\tconsole.log("Hello world!");', '}'].join('\n'),
            language: 'typescript'
        });
    })
</script>

>}}