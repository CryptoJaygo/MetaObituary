<script setup>
import { LINKS } from "@/utils/constants";
</script>
<template>
	<section id="footer" class="footer py-28 px-3 bg-bg-soft">
		<div class="footer-inner container max-w-7xl mx-auto">
			<div>
				<h4 class="text-[2.2em] font-bold">Contributors:</h4>
			</div>
			<div class="links mt-[2.2em]">
				<a
					:href="url"
					class="mr-5 text-font-light underline"
					v-for="({ title, url }, idx) of LINKS"
					:key="idx"
					target="_blank"
					>{{ title }}</a
				>
			</div>
			<div class="links mt-[2.2em]">
				<span>We are Open Source:</span>
				<a
					href="https://github.com/CryptoJaygo/MetaObituary"
					class="mr-5 text-font-light underline"
					target="_blank"
					>Github</a
				>
			</div>
			<div class="links mt-[2.2em]">
				<span
					>We accept donations. Ethereum address:
					0xD52A88754e37722D0005B918955B905F6Bc170BA</span
				>
			</div>
		</div>
	</section>
</template>
