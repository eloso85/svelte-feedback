<script>
	import Component1 from "./components/Component1.svelte";


	let name = "alejandro";
	let catUrl = 'https://cdn.pixabay.com/photo/2017/02/20/18/03/cat-2083492_1280.jpg'
	let src = 'https://cdn.pixabay.com/photo/2017/02/20/18/03/cat-2083492_1280.jpg'

	// Functions

	let count = 0;

	function increment() {
		//assignment
			//count = 10;
		// update statements
			//count ++
		// updating / assigning property
			//obj.count++;
		count ++;
	}


</script>







<h1>My First Svelte component</h1>

<p>Hello World</p>
<h2>My name is {name}</h2>
<div>
	<img alt='cat' src={catUrl} width="200" height="200" >
	<img alt='cat' {src} width="200" height="200" >
	<!-- This is the short hand if the variable is the same as the atribute  -->


	<a href="http://">Link to my youtube channel</a>
</div>

<Component1 />


{count}
<button on:click={increment}>
	click Me
</button>






















<style>
	h1 {
		color: rebeccapurple;
		animation: zoom 5s infinite;
	}

	/* :global(h1) {  exp- the :global() applies styles to all components. 
		color: rebeccapurple;
		animation: zoom 5s infinite;
	} */

	p {
		font-size: 44px;
	}

	@keyframes zoom {
		0%, 100% { transform: scale(3);}
		50% {transform: scale(0.5);}
	}

	/* @keyframes -global-zoom { exp - makes keyframes global psuedo selector
		0%, 100% { transform: scale(3);}
		50% {transform: scale(0.5);}
	} */

</style>


