<template>
    <header class="bg-purple-600">
    <div class="max-w-7xl mx-auto px-2 sm:px-4 lg:divide-y lg:divide-gray-700 lg:px-8">
        <div class="relative h-16 flex justify-between">
        <div class="relative z-10 flex items-center lg:hidden">
            <!-- Mobile menu button -->
            <button type="button" class="rounded-md p-2 inline-flex items-center justify-center text-gray-400 hover:bg-gray-700 hover:text-white focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white" aria-controls="mobile-menu" aria-expanded="false">
            <span class="sr-only">Open menu</span>
            <svg class="block h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
            </svg>
            <svg class="hidden h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
            </svg>
            </button>
        </div>
        </div>
        <nav class="hidden lg:py-2 lg:flex lg:space-x-8" aria-label="Global">
        <!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
        <a href="#" class="bg-gray-900 text-white rounded-md py-2 px-3 inline-flex items-center text-sm font-medium" aria-current="page">
            Reiki
        </a>

        <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md py-2 px-3 inline-flex items-center text-sm font-medium">
            Medicina Natural
        </a>

        <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md py-2 px-3 inline-flex items-center text-sm font-medium">
            Grupos de Meditacion
        </a>

        <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md py-2 px-3 inline-flex items-center text-sm font-medium">
            Tienda
        </a>
        </nav>
    </div>

    <!-- Mobile menu, show/hide based on menu state. -->
    <nav class="lg:hidden" aria-label="Global" id="mobile-menu">
        <div class="pt-2 pb-3 px-2 space-y-1">
        <a href="#" class="bg-gray-900 text-white block rounded-md py-2 px-3 text-base font-medium" aria-current="page">Reiki</a>

        <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md py-2 px-3 text-base font-medium">Medicina Natural</a>

        <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md py-2 px-3 text-base font-medium">Grupos de Meditacion</a>

        <a href="#" class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md py-2 px-3 text-base font-medium">Tienda</a>
        </div>
        <div class="border-t border-gray-700 pt-4 pb-3">

        </div>
    </nav>
    </header>
</template>