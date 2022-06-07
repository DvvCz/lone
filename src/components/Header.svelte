<script lang="ts">
    import Logo from "../components/Logo.svelte";

    import Button, { Label } from "@smui/button";
    import IconButton, { Icon } from "@smui/icon-button";
    import TopAppBar, { Row, Section } from "@smui/top-app-bar";

    let lightMode = false;
</script>

<style>
    div#header {
        height: 10%;
    }
</style>

<section>
    <div id="header">
        <TopAppBar variant="static" color={"primary"}>
            <Row>
                <Section>
                    <Logo/>
                </Section>
                <Section>
                    <Button on:click={() => lightMode = !lightMode}>
                        <Label>Default</Label>
                    </Button>
                </Section>
                <Section>
                    <IconButton toggle bind:pressed={lightMode}>
                        <Icon class="material-icons" on>dark_mode</Icon>
                        <Icon class="material-icons">light_mode</Icon>
                    </IconButton>
                </Section>
            </Row>
        </TopAppBar>
    </div>
</section>