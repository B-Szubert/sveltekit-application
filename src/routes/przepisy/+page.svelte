<svelte:head>
		<title>Recipes</title>
		<meta name="description" content="List of recipes" />
</svelte:head>



<div id="recipes-container">
	{#each recipes as recipe (recipe.nazwa)}
		<div class="recipe">
			<h2>{recipe.nazwa}</h2>
			<ul>
				{#each recipe.skladniki as ingredient (ingredient)}
					<li>{ingredient}</li>
				{/each}
			</ul>
			<p>{recipe.instrukcje}</p>
		</div>
	{/each}
</div>

<script>
	// import { PrismaClient } from '@prisma/client'
	// const prisma = new PrismaClient()

	// prisma.$connect()

	// async function fetchRecipes() {
	// 	const recipes = await prisma.recipe.findMany({
	// 		include: {
	// 			ingredients: true
	// 		}
	// 	})
		
	// 	console.log(recipes) // Use the recipes variable here or remove it if not needed
	// }

	// fetchRecipes()

	// prisma.$disconnect()
	let recipes = [
		{ nazwa: 'Pasta Carbonara', skladniki: ['makaron', 'bekon', 'jajka', 'ser'], instrukcje: 'Ugotuj makaron. Usmaż bekon. Wymieszaj jajka i ser. Połącz wszystko.' },
		{ nazwa: 'Kurczak Curry', skladniki: ['kurczak', 'proszek curry', 'mleko kokosowe', 'warzywa'], instrukcje: 'Ugotuj kurczaka. Dodaj proszek curry. Dodaj mleko kokosowe. Dodaj warzywa.' },
		{ nazwa: 'Ciasto czekoladowe', skladniki: ['mąka', 'cukier', 'kakao', 'jajka', 'masło'], instrukcje: 'Wymieszaj wszystko. Piecz.'}
	];
</script>

<style>
	#recipes-container {
		background-color: #f2f2f2;
		padding: 20px;
		border-radius: 5px;
	}

	.recipe {
		margin-bottom: 20px;
		border: 1px solid #ccc;
		padding: 10px;
		border-radius: 5px;
	}

	.recipe h2 {
		color: #333;
		font-size: 20px;
		margin-bottom: 10px;
	}

	.recipe ul {
		list-style-type: square;
		margin-left: 30px;
		padding: 0;
	}

	.recipe li {
		margin-bottom: 5px;
	}

	.recipe p {
		color: #666;
	}
</style>