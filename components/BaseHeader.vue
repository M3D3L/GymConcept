<template>
	<div>
    <!-- component -->
<nav id="header" class="fixed top-0 z-20 w-full text-white bg-black">
	<div id="progress" class="top-0 z-40 h-1"
		style="background:linear-gradient(to right, #FFC100 var(--scroll), transparent 0);"></div>
	<div class="flex flex-wrap items-center justify-between w-full py-3 mx-auto mt-0 md:max-w-4xl">
		<div class="block p-2 pl-8 lg:hidden">
			<a class="text-base font-bold text-yellow-300 no-underline hover:no-underline" href="#">
        (423)-123-4567
			</a>
		</div>
		<div class="block pr-4 lg:hidden">
			<button id="nav-toggle" class="flex items-center px-3 py-2 text-yellow-300 border-gray-600 focus:outline-none">
          <svg fill="text-yellow-300" viewBox="0 0 20 20" class="w-6 h-6 fill-current">
            <title>Menu</title>
            <path fill-rule="evenodd"
              d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM9 15a1 1 0 011-1h6a1 1 0 110 2h-6a1 1 0 01-1-1z"
              clip-rule="evenodd"></path>
          </svg>
        </button>
		</div>
		<div class="z-20 flex-grow hidden w-full p-4 mt-2 bg-black lg:flex lg:items-center lg:w-auto lg:block lg:mt-0 md:bg-transparent"
			id="nav-content">
			<ul class="items-center justify-center flex-1 list-reset lg:flex">
				<li class="mr-3">
					<a class="inline-block px-4 py-2 hover:text-yellow-300 hover:text-underline" href="#">Home</a>
				</li>
				<li class="mr-3">
					<a class="inline-block px-4 py-2 hover:text-yellow-300 hover:text-underline" href="#service">Our Service</a>
				</li>
				<li class="mr-3">
					<a class="inline-block px-4 py-2 hover:text-yellow-300 hover:text-underline" href="#test">Testimonials</a>
				</li>

        <li class="mr-3">
					<a class="inline-block px-4 py-2 hover:text-yellow-300 hover:text-underline" href="#price">Pricing</a>
				</li>

				<li class="mr-3">
					<a class="inline-block px-4 py-2 hover:text-yellow-300 hover:text-underline" href="#contact">Contact</a>
				</li>
			</ul>
		</div>
	</div>
</nav>

<script>
	var h = document.documentElement,
    b = document.body,
    st = 'scrollTop',
    sh = 'scrollHeight',
    progress = document.querySelector('#progress'),
    scroll;
var scrollpos = window.scrollY;
var header = document.getElementById("header");
var navcontent = document.getElementById("nav-content");

document.addEventListener('scroll', function () {
    scroll = (h[st] || b[st]) / ((h[sh] || b[sh]) - h.clientHeight) * 100;
    progress.style.setProperty('--scroll', scroll + '%');
    scrollpos = window.scrollY;

    if (scrollpos > 10) {
        header.classList.add("bg-black");
        navcontent.classList.remove("bg-black");
        navcontent.classList.add("bg-black");
    } else {
        header.classList.remove("bg-black");
        navcontent.classList.remove("bg-black");
        navcontent.classList.add("bg-black");

    }

});

document.getElementById('nav-toggle').onclick = function () {
    document.getElementById("nav-content").classList.toggle("hidden");
}
</script>
				</div>
</template>


