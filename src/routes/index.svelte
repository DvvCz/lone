<script lang="ts">
	import Blockly from "$lib/Blockly.svelte";
	
	let Count = 0;
</script>

<svelte:head>
<title>Home</title>
<meta name="description" content="Lone IDE" />
</svelte:head>

<section>
	<Blockly>
		<category name="Functions" custom="PROCEDURE"></category>
		<category name="Variables" custom="VARIABLE"/>
		<block type="text_charAt">
			<value name="VALUE">
				<block type="variables_get">
					<field name="VAR">text</field>
				</block>
			</value>
		</block>
	</Blockly>
</section>