<script lang="ts">
	import '../app.css';
	let { children } = $props();
</script>

{@render children()}

<!-- SVG Filter -->
 
<!-- Apollo: `filter: url(#Apollo)` -->
<svg id="svg-filter-apollo" class="absolute -left-full w-0 h-0">
	<filter id="Apollo" filterUnits="objectBoundingBox" primitiveUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
	  <feColorMatrix values="0.8 0.6 -0.4 0.1 0,
		0 1.2 0.05 0 0,
		0 -1 3 0.02 0,
		0 0 0 50 0" result="final" in="SourceGraphic"></feColorMatrix>
	</filter>
</svg>

<!-- BlueNight: `filter: url(#BlueNight)` -->
<svg id="svg-filter-bluenight" class="filter absolute -left-full w-0 h-0">
	<filter id="BlueNight" filterUnits="objectBoundingBox" primitiveUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
	  <feColorMatrix
		type="matrix"
		values="1.000 0.000 0.000 0.000 0.000
					  0.000 1.000 0.000 0.000 0.05
					  0.000 0.000 1.000 0.000 0.400
					  0.000 0.000 0.000 1.000 0.000"
	  ></feColorMatrix>
	</filter>
</svg>

<!-- GreenFall: `filter: url(#GreenFall)` -->
<svg id="svg-filter-greenfall" class="filter absolute -left-full w-0 h-0">
	<filter
	  id="GreenFall"
	  x="-20%"
	  y="-20%"
	  width="140%"
	  height="140%"
	  filterUnits="objectBoundingBox"
	  primitiveUnits="userSpaceOnUse"
	  color-interpolation-filters="linearRGB"
	>
	  <feColorMatrix
		type="matrix"
		values="0.5 -0.4 0.3332 0 0
			0 0.4 0.3 0 0
			0 0 0.5 0 0
			0 0 0 500 -20"
		x="0%"
		y="0%"
		width="100%"
		height="100%"
		in="SourceGraphic"
		result="colormatrix"></feColorMatrix>
	</filter>
</svg>

<!-- Noir: `filter: url(#Noir)` -->
<svg id="svg-filter-noir" class="filter absolute -left-full w-0 h-0">
	<filter
	  id="Noir"
	  x="-20%"
	  y="-20%"
	  width="140%"
	  height="140%"
	  filterUnits="objectBoundingBox"
	  primitiveUnits="userSpaceOnUse"
	  color-interpolation-filters="linearRGB"
	>
	  <feColorMatrix type="saturate" values="0" x="0%" y="0%" width="100%" height="100%" in="SourceGraphic" result="colormatrix1"
	  ></feColorMatrix>
	  <feBlend mode="lighten" x="0%" y="0%" width="100%" height="100%" in="colormatrix1" in2="colormatrix1" result="blend"></feBlend>
	  <feBlend mode="multiply" x="0%" y="0%" width="100%" height="100%" in="colormatrix1" in2="diffuseLighting" result="blend1"></feBlend>
	</filter>
</svg>

<!-- NoirLight: `filter: url(#NoirLight)` -->
<svg id="svg-filter-noirlight" class="filter absolute -left-full w-0 h-0">
	<filter
	  id="NoirLight"
	  x="-20%"
	  y="-20%"
	  width="140%"
	  height="140%"
	  filterUnits="objectBoundingBox"
	  primitiveUnits="userSpaceOnUse"
	  color-interpolation-filters="linearRGB"
	>
	  <feColorMatrix type="saturate" values="0" x="0%" y="0%" width="100%" height="100%" in="SourceGraphic" result="colormatrix2"
	  ></feColorMatrix>
	  <feBlend mode="saturation" x="0%" y="0%" width="100%" height="100%" in="SourceGraphic" in2="colormatrix2" result="blend2"></feBlend>
	  <feBlend mode="screen" x="0%" y="0%" width="100%" height="100%" in="colormatrix2" in2="blend2" result="blend3"></feBlend>
	  <feColorMatrix type="luminanceToAlpha" x="0%" y="0%" width="100%" height="100%" in="blend3" result="colormatrix3"></feColorMatrix>
	  <feBlend mode="exclusion" x="0%" y="0%" width="100%" height="100%" in="blend3" in2="colormatrix3" result="blend5"></feBlend>
	</filter>
</svg>

<!-- Rustic: `filter: url(#Rustic)` -->
<svg id="svg-filter-rustic" class="filter absolute -left-full w-0 h-0">
	<filter id="Rustic" filterUnits="objectBoundingBox" primitiveUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
	  <feColorMatrix
		type="matrix"
		in="SourceGraphic"
		result="colormatrix"
		values="0.39215686274509803 0.39215686274509803 0.39215686274509803  0 0
			0.3333333333333333 0.3333333333333333 0.3333333333333333  0 0
			0.30980392156862746 0.30980392156862746 0.30980392156862746  0 0
			0 0 0 1 0"
	  ></feColorMatrix>
	</filter>
</svg>

<!-- Summer: `filter: url(#Summer)` -->
<svg id="svg-filter-summer" class="filter absolute -left-full w-0 h-0">
	<filter id="Summer" filterUnits="objectBoundingBox" primitiveUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
	  <feColorMatrix
		type="matrix"
		values="1.300 0.200 0.000 0.000 0.000
			0.300 0.600 0.200 0.000 0.000
			0.200 1.000 0.200 0.000 0.000
			0.000 0.000 0.000 1.000 0.000"
	  ></feColorMatrix>
	</filter>
</svg>

<!-- XPro: `filter: url(#XPro)` -->
<svg id="svg-filter-xpro" class="filter absolute -left-full w-0 h-0">
	<filter id="XPro" filterUnits="objectBoundingBox" primitiveUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
	  <feColorMatrix
		type="matrix"
		values="1.70 -0.20 0.00 0.00 0.00
					  0.10 0.800 0.30 0.00 0.00
					  0.20 0.300 0.50 0.00 0.00
					  0.00 0.00 0.00 1.00 0.00"
	  ></feColorMatrix>
	</filter>
</svg>