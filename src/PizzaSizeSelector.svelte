 <script>

export let size = [];


    let selectedValue = size[0].value;

    $: windowPosition = getPosition(selectedValue);

    function getPosition(){
        let value = size.findIndex(fn => {
            if(fn.value == selectedValue){
                return true;
            }
        });

        return (33*value).toString() + '%';
    }

 </script>
 
 <div class="selector">
    <div class="type">
    </div>
    <div class="size">
        <span class="window" style="left: {windowPosition};"></span>
        {#each size as item}
        <label>
            <input type="radio" bind:group={selectedValue} name="size" value="{item.value}">
            {item.name}
        </label>
        {/each}
    </div> 
</div>