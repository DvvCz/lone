<script lang="ts">
    import Logo from "../components/Logo.svelte";

    import Button, { Label } from "@smui/button";
    import Fab, { Icon } from "@smui/icon-button";
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
                    <Fab color="secondary">
                        <Icon class="material-icons">check</Icon>
                    </Fab>
                    <Fab color="secondary">
                        <Icon class="material-icons">download</Icon>
                    </Fab>
                    <Fab color="secondary">
                        <Icon class="material-icons">sim_card_download</Icon>
                    </Fab>
                    <Fab color="secondary">
                        <Icon class="material-icons">dvr</Icon>
                    </Fab>
                    <Fab color="secondary">
                        <Icon class="material-icons">timeline</Icon>
                    </Fab>
                </Section>
            </Row>
        </TopAppBar>
    </div>
</section>