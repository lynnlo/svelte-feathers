<script>
  import { getContext } from 'svelte';
  const ctx = getContext('iconCtx') ?? {};
  export let size = ctx.size || '24';
  export let role = ctx.role || 'img';
  export let color = ctx.color || 'currentColor';
  export let tabIndex = ctx.tabIndex || '-1';
  export let fill = ctx.fill || 'none';
  export let ariaLabel = 'sunset';
</script>

<svg
  xmlns="http://www.w3.org/2000/svg"
  width={size}
  height={size}
  viewBox="0 0 24 24"
  fill={fill}
  stroke={color}
  tabIndex={tabIndex}
  stroke-width="2"
  stroke-linecap="round"
  stroke-linejoin="round"
  class={$$props.class}
  {role}
  aria-label={ariaLabel}
  on:click
  on:keydown
  on:keyup
  on:focus
  on:blur
  on:mouseenter
  on:mouseleave
  on:mouseover
  on:mouseout
  ><path d="M17 18a5 5 0 0 0-10 0" /><line x1="12" y1="9" x2="12" y2="2" /><line
    x1="4.22"
    y1="10.22"
    x2="5.64"
    y2="11.64"
  /><line x1="1" y1="18" x2="3" y2="18" /><line x1="21" y1="18" x2="23" y2="18" /><line
    x1="18.36"
    y1="11.64"
    x2="19.78"
    y2="10.22"
  /><line x1="23" y1="22" x2="1" y2="22" /><polyline points="16 5 12 9 8 5" /></svg
>

<!--
@component
[Go to docs](https://svelte-feathers.codewithshin.com)
## Props
@prop export let size = ctx.size || '24';
@prop export let role = ctx.role || 'img';
@prop export let color = ctx.color || 'currentColor';
  export let tabIndex = ctx.tabIndex || '-1';
@prop export let ariaLabel = 'sunset';
-->
