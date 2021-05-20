<template>
	<div class="min-h-full py-32 text-white bg-black">
		<div class="container flex flex-col items-center mx-auto my-12 md:flex-row md:my-24">
			<div class="flex flex-col items-start justify-center w-1/2 p-8">
				<h1 class="p-2 text-3xl font-bold text-yellow-400 md:text-6xl tracking-loose">Boulder Gym</h1>
				<h2 class="mb-2 text-3xl leading-relaxed md:text-5xl md:leading-snug">Strengthening Lives
				</h2>
				<p class="mb-4 text-sm md:text-base text-gray-50">We help you get in the best shape of your life. Find out how we can help you become strong. Boulder strong.</p>
				<a href="#service"
					class="px-4 py-2 text-yellow-400 bg-transparent border border-yellow-400 rounded shadow hover:bg-yellow-400 hover:text-black hover:shadow-lg ">
					See How</a>
			</div>
			<div class="justify-center w-full p-8 mt-12 mb-6 ml-0 md:mb-0 md:mt-0 md:ml-12">
				<div class="flex flex-wrap items-center content-center justify-center h-full">

							<img class="hidden inline-block p-8 md:mt-0 md:p-0 left-arrow h-80 lg:block opacity-70 hover:opacity-100 grow"  src="../assets/HeroWorkout.jpg">
              <img class="hidden inline-block p-8 md:mt-0 md:p-0 left-arrow h-96 opacity-70 hover:opacity-100 md:block grow"  src="https://images.pexels.com/photos/3289711/pexels-photo-3289711.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260">
              <img class="hidden inline-block p-8 md:mt-0 md:p-0 left-arrow h-80 opacity-70 hover:opacity-100 grow xl:block"  src="../assets/heroPic.jpg">
              </div>

						</div>
					</div>
				</div>
</template>

<style>
.left-arrow {
  clip-path: polygon(100% 0%, 75% 50%, 100% 100%, 25% 100%, 0% 50%, 25% 0%);
}
.grow { transition: all .2s ease-in-out; }
.grow:hover { transform: scale(1.1); }
</style>
