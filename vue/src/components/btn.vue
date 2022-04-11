<template>
  <button class="btn">
    <span class="shape"></span>
    <span class="slot">
      <slot></slot>
    </span>
  </button>
</template>

<!-- Standard pill button -->

<script>
</script>

<!-- ––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––– -->

<style scoped>

.btn {
  position: relative;

	/* // Center contents */
	display: inline-flex;
	align-items: center;
	justify-content: center;

	/* // Clear possibly inheritted underline */
	text-decoration: none;

	/* // Typography */
	color: white;
	/* fluid font-size, body-font-size, body-font-size-min */
	font-weight: 700;
  border: none;
  background: transparent;
  font-size: 16px;
}
  /* // Make backgound state */
.shape {

  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: var(--blue);
  border-radius: 20px;
  /* transition background .4s, transform .1s, box-shadow .2s
  +tablet-up()
    border-radius btn-desktop-h * 0.5
  +tablet-down()
    border-radius btn-mobile-h * 0.5
    &.size-small
      height btn-small-h * 0.5 */
}

.slot {
  /* // Align slotted stuff */
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 10px 20px;
  text-decoration: none;

	/* // Overlap the shape */
	position: relative;

	/* // Push edges away */
	/* fluid padding-h, btn-pad-h, btn-pad-h-min
	.size-small &
		fluid padding-h, btn-pad-h, btn-pad-h-small */

}

	/* // Set height
	position relative
	+tablet-up()
		height btn-desktop-h
	+tablet-down()
		height btn-mobile-h
		&.size-small
			height btn-small-h */



	/* // Disable cursor when disabled
	&[disabled]
		cursor default */

	/* // Add hover/active effects
	&:not([disabled])
		+hover(true)
			.shape
				background var(--blue)
				transition-duration .2s
		+active()
			.shape
				transform scaleX(0.925)

		// Add custom focus state
		.js-focus-visible &.focus-visible:focus
			outline none
			.shape
				box-shadow inset 0 0 0 2px lighten(primary-color, 10%)
				transition-duration .1s */

	/* // Prevent content from spilling out
	overflow hidden */



	/* // Disabled state
	[disabled] &
		background-color grey-bkgd */

/*
.icon-spinner
	margin-left 7px
	font-size 0.8em
	animation spin 0.5s linear infinite

	// Transition effects
	&.v-enter-active, &.v-leave-active
		transition opacity 0.1s
	&.v-enter, &.v-leave-to
		opacity 0 */


</style>
