<script lang="ts">
    import { onMount } from 'svelte';
    import Blockly from 'blockly';
    onMount(() => {
        Blockly.inject(document.getElementById("blocklyDiv"), {
            toolbox: document.getElementById("toolbox")
        });
    });
</script>

<style scoped>
    #blocklyDiv {
        height: 90%;
        width: 100%;
        position: absolute;
        bottom: 0;
        text-align: left;
    }
</style>

<div>
    <div id="blocklyDiv" />
    <xml id="toolbox" style="display:none">
        <slot />
    </xml>
</div>