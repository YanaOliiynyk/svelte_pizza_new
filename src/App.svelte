<script>
    import Header from "./Header.svelte";
    import PizzaCard from "./PizzaCard.svelte";

	let arrayPizza = [
		{
			'image': '/img/pizza/pizza.png',
			'name': 'pizza1',
			'price': 350,
			'size':[
				{
					name: '20cm',
					value:20
				},
				{
					name: '30cm',
					value:30
				},
				{
					name: '40cm',
					value:40
				}],
			'type':[{
				name: 'thin'
			},{
				name: 'tradition'
			}]
		},
		{
			'image': '/img/pizza/pizza2.png',
			'name': 'pizza2',
			'price': 350,
			'size':[
				{
					name: '20cm',
					value:20
				},
				{
					name: '30cm',
					value:30
				},
				{
					name: '40cm',
					value:40
				}],
				'type':[{
				name: 'thin',
				value: 1
			},{
				name: 'tradition',
				value: 2
			}]
		},
		{
			'image': '/img/pizza/pizza3.png',
			'name': 'pizza3',
			'price': 350,
			'size':[
				{
					name: '20cm',
					value:20
				},
				{
					name: '30cm',
					value:30
				},
				{
					name: '40cm',
					value:40
				}],
				'type':[{
				name: 'thin',
				value: 1
			},
			{
				name: 'tradition',
				value: 2
			}]
		},
		{
			'image': '/img/pizza/pizza4.png',
			'name': 'pizza4',
			'price': 350,
			'size':[
				{
					name: '20cm',
					value:20
				},
				{
					name: '30cm',
					value:30
				},
				{
					name: '40cm',
					value:40
				}],
				'type':[{
				name: 'thin',
				value: 1
			},{
				name: 'tradition',
				value: 2
			}]
		},
		{
			'image': '/img/pizza/pizza.png',
			'name': 'pizza5',
			'price': 350,
			'size':[
				{
					name: '20cm',
					value:20
				},
				{
					name: '30cm',
					value:30
				},
				{
					name: '40cm',
					value:40
				}],
				'type':[{
				name: 'thin',
				value: 1
			},{
				name: 'tradition',
				value: 2
			}]
		},
		{
			'image': '/img/pizza/pizza2.png',
			'name': 'pizza6',
			'price': 350,
			'size':[
				{
					name: '20cm',
					value:20
				},
				{
					name: '30cm',
					value:30
				},
				{
					name: '40cm',
					value:40
				}]
		},
		{
			'image': '/img/pizza/pizza3.png',
			'name': 'pizza7',
			'price': 350,
			'size':[
				{
					name: '20cm',
					value:20
				},
				{
					name: '30cm',
					value:30
				},
				{
					name: '40cm',
					value:40
				}],
				'type':[{
				name: 'thin',
				value: 1
			},{
				name: 'tradition',
				value: 2
			}]
		},
		{
			'image': '/img/pizza/pizza4.png',
			'name': 'pizza8',
			'price': 350,
			'size':[
				{
					name: '20cm',
					value:20
				},
				{
					name: '30cm',
					value:30
				},
				{
					name: '40cm',
					value:40
				}],
				'type':[{
				name: 'thin',
				value: 1
			},{
				name: 'tradition',
				value: 2
			}]
		},
	];
</script>

<Header/>
<section id="menu">
	<div class="container">
		{#each arrayPizza as pizza}
			<PizzaCard {...pizza}/>
		{/each}
	</div>
</section>