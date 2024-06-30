<template>
  <header class="flex justify-between border-b border-slate-200 px-5 py-4">
    <div class="flex items-center gap-3">
      <img src="/logo.png" alt="Logo" class="w-11" />
      <div>
        <h2 class="font-bold text-base uppercase">Vue Sneakers</h2>
        <p class="text-slate-400 text-sm">Магазин лучших кроссовок</p>
      </div>
    </div>

    <ul class="flex items-center gap-10">
      <li class="flex items-center gap-2 text-gray-500 cursor-pointer hover:text-black">
        <img src="/cart.svg" alt="Cart" />
        <p>1205 руб.</p>
      </li>
      <li class="flex items-center gap-3 text-gray-500 cursor-pointer hover:text-black">
        <img src="/heart.svg" alt="Favorite" />
        <span>Закладки</span>
      </li>
      <li class="flex items-center gap-3 text-gray-500 cursor-pointer hover:text-black">
        <img src="/profile.svg" alt="Favorite" />
        <span>Профиль</span>
      </li>
    </ul>
  </header>
</template>
