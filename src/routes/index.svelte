<style lang="scss">
    .table {
        background: azure;
    }
    .cell {
        padding: 5px 10px;
        border: solid 1px black;
        &.-title {
            background: #555555;
        }
    }
</style>

<script>
    import { onMount } from "svelte";

    let MyComponent;

    onMount(async () => {
        console.log(122222);
    });
</script>

<svelte:head>
    <title>Sapper project template</title>
</svelte:head>

<table class="table">
    <thead>
        <tr class="table__head-row">
            <th class="cell -title">title</th>
            <th class="cell -title">contents</th>
            <th class="cell -title">Date</th>
        </tr>
    </thead>
    <tbody>
        <tr class="table__body-row">
            <td class="cell">内容</td>
            <td class="cell">aaaa</td>
            <td class="cell">2019-12-24</td>
        </tr>
    </tbody>
</table>
