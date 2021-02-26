<script>
	function selectVideo() {
		video = videos[Math.floor(Math.random() * videos.length)];
	}

	const videos = [
		{
			name: "Across Sideways Reach - Shown in Cross Sit",
			video:
				'<iframe width="560" height="315" src="https://www.youtube.com/embed/Ihu91p4c0hA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>',
		},
		{
			name: "Backward Reach - Shown in Deep Squat",
			video:
				'<iframe width="560" height="315" src="https://www.youtube.com/embed/imrGl6dU9hY" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>',
		},
		{
			name: "Forward Reach - Shown in Cross Sit",
			video:
				'<iframe width="560" height="315" src="https://www.youtube.com/embed/z4vOsMwcn78" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>',
		},
		{
			name: "Rotational Backward Reach - Shown in Side Bent Sit",
			video:
				'<iframe width="560" height="315" src="https://www.youtube.com/embed/doPd0DnI_j0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>',
		},
		{
			name: "Sideways Reach - Shown in Deep Kneel",
			video:
				'<iframe width="560" height="315" src="https://www.youtube.com/embed/2TISlOiRllc" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>',
		},
		{
			name: "Upward Reach - Shown in Bent Sit",
			video:
				'<iframe width="560" height="315" src="https://www.youtube.com/embed/sHWTYzvKOlE" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>',
		},
		{
			name: "Deep Squat",
			video:
				'<iframe width="560" height="315" src="https://www.youtube.com/embed/c32s75S1zUM" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>',
		},
		{
			name: "Deep Knee Bend",
			video:
				'<iframe width="560" height="315" src="https://www.youtube.com/embed/CF1rlB58EuA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>',
		},
		{
			name: "Kneel",
			video:
				'<iframe width="560" height="315" src="https://www.youtube.com/embed/lAb_t1gzy3g" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>',
		},
		{
			name: "Tripod Transition",
			video:
				'<iframe width="560" height="315" src="https://www.youtube.com/embed/Q35KsSr7Tc0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>',
		},
		{
			name: "Tripod Transition",
			video:
				'<iframe width="560" height="315" src="https://www.youtube.com/embed/Q35KsSr7Tc0" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>',
		},
		{
			name: "Side Bent Sit Reverse",
			video:
				'<iframe width="560" height="315" src="https://www.youtube.com/embed/eHRsWxgud5E" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>',
		},
	];
	let video = {};

	selectVideo();
</script>

<main>
	<h1>Mouvement aléatoire de MovNat</h1>
	<h3>{video.name}</h3>
	{@html video.video}
	<div>
		<button on:click={selectVideo}>Donnez m'en un autre !</button>
	</div>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
