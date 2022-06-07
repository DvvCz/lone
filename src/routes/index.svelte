<script lang="ts">
	import Blockly from "../components/Blockly.svelte";
	import Header from "../components/Header.svelte";
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Lone IDE" />
</svelte:head>

<section>
	<Header/>
	<Blockly>
		<category name="Functions" custom="PROCEDURE"></category>
		<category name="Variables" custom="VARIABLE"/>
		<category name="Propeller">
			<block type="text_charAt">
				<value name="VALUE">
					<block type="variables_get">
						<field name="VAR">text</field>
					</block>
				</value>
			</block>
		</category>
	</Blockly>
</section>

<style>
	:global(body) {
		margin: 0;
		padding: 0;
	}
</style>