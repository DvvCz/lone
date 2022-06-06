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
		<block type="controls_ifelse" />
		<block type="logic_compare" />
		<block type="logic_operation" />
		<block type="controls_repeat_ext">
			<value name="TIMES">
				<shadow type="math_number">
					<field name="NUM">10</field>
				</shadow>
			</value>
		</block>
		<block type="logic_operation" />
		<block type="logic_negate" />
		<block type="logic_boolean" />
		<block type="logic_null" disabled="true" />
		<block type="logic_ternary" />
		<block type="text_charAt">
			<value name="VALUE">
				<block type="variables_get">
					<field name="VAR">text</field>
				</block>
			</value>
		</block>
	</Blockly>
</section>