<script>
    export let image = '';
    export let name = 'Pizza';
    export let price = '100';

    export let size =[];
    import Button from "./Button.svelte";
    import PizzaSizeSelector from "./PizzaSizeSelector.svelte";
</script>

<div class="pizza-card">
    <div class="img">
        <img src="{image}" alt="X">
    </div>
    <div class="name">{name}</div>
    <PizzaSizeSelector size={size}/>
    <div class="price-block">
        <div class="price">Від {price} грн</div>
          <Button>Купити</Button>
    </div>
</div>