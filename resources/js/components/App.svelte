<script>
    import { onMount } from "svelte";
    import { Card } from "attractions";

    onMount(() => {
      console.log("the component has mounted");
    });
</script>

<main>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-8">
                <div class="card">
                    <Card>
                        Example Attractions Component
                    </Card>
                    <Card outline>
                        I'm an example Attractions component.
                    </Card>
                    <div class="card-header">
                        Example Bootstrap Component
                    </div>
                    <div class="card-body">
                        I'm an example Bootstrap component.
                    </div>
                </div>
            </div>
        </div>
    </div>
</main>
<style lang="scss">
    @use 'theme.scss';
    .outline {
        color: theme.$main;
    }
</style>
