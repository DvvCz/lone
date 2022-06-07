<script lang="ts">
    import Button, { Label } from "@smui/button";
</script>

<style>
    div#header {
        height: 10%;
    }
</style>

<section>
    <div id="header">
        Header
    </div>
    <Button on:click={() => console.log("Test")}>
        <Label>Default</Label>
    </Button>
</section>