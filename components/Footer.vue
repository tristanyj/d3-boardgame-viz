<template>
  <div :class="['nav-container', $style.container]">
    <div :class="$style.separator" />
    <div :class="$style.entry">
      Source code
      <NuxtLink
        to="https://github.com/tristanyj/d3-boardgame-forest"
        target="_blank"
        :class="$style.link"
        >Github
      </NuxtLink>
    </div>
    <div :class="$style.entry">
      Inspired by
      <NuxtLink
        to="https://shirleywu.studio/filmflowers/"
        target="_blank"
        :class="$style.link"
        >Shirley Wu's Films Flowers
      </NuxtLink>
    </div>
    <div :class="$style.entry">
      Data from
      <NuxtLink
        to="https://boardgamegeek.com/browse/boardgame"
        target="_blank"
        :class="$style.link"
        >BoardGameGeek
      </NuxtLink>
    </div>
  </div>
</template>

<style lang="scss" module>
.container {
  gap: 8px;
  padding: 0px;
}

.separator {
  width: 100%;
  max-width: 200px;
  margin: 20px auto 30px auto;
  height: 1px;
  background-color: #000;
  opacity: 0.1;
}

.entry {
  color: var(--mauve-11);
}

.link {
  background-color: var(--mauve-2);
  padding: 2px;
  margin-left: 2px;
  border-radius: 5px;
  color: var(--mauve-12);

  &:hover {
    background-color: var(--mauve-3);
  }
}
</style>
