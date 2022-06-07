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
		<category colour=100 name="Control"/>
		<category colour=200 name="Operators"/>

		<sep/>

		<category colour=300 name="Constants"/>
		<category colour=250 name="Arrays"/>
		<category colour=230 name="Variables" custom="VARIABLE"/>
		<category colour=350 name="Functions" custom="PROCEDURE"/>
		<category colour=120 name="Pin States"/>
		<category colour=140 name="Communicate"/>
		<category colour=160 name="Sensor"/>
		<category colour=210 name="Memory"/>
		<category colour=230 name="Analog"/>
		<category colour=240 name="Audio"/>
		<category colour=320 name="Servo"/>
		<category colour=340 name="Robot"/>
		<category colour=50 name="System"/>
		<sep/>

		<!-- control operators values arrays functions pin states communicate sensor memory analog/pulses audio servo robot system -->
		<category colour=210 name="Propeller">
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