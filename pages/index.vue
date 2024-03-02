<template>
	<MainLayout>
		<div id="IndexPage class mt-4 max-w-[1200px] mx-auto px-2">
			<div
				class="grid xl:grid-cols-6 ld:grid-cols-5 md:grid-cols-4 sm:grid-cols-3 grid-cols-2 gap-4"
			>
				<div v-if="products" v-for="product in products" :key="product">
					<ProductComponent :product="product" />
				</div>
			</div>
		</div>
	</MainLayout>
</template>

<script setup>
import MainLayout from "~/layouts/MainLayout.vue"

const products = [
	{
		id: 1,
		title: "Title 1",
		description: "Description",
		url: "https://picsum.photos/id/7/800/800",
		price: 9999,
	},
	{
		id: 2,
		title: "Title 2",
		description: "Description",
		url: "https://picsum.photos/id/71/800/800",
		price: 3399,
	},
	{
		id: 3,
		title: "Title 3",
		description: "Description",
		url: "https://picsum.photos/id/72/800/800",
		price: 4499,
	},
	{
		id: 4,
		title: "Title 4",
		description: "Description",
		url: "https://picsum.photos/id/73/800/800",
		price: 4499,
	},
	{
		id: 5,
		title: "Title 5",
		description: "Description",
		url: "https://picsum.photos/id/74/800/800",
		price: 1199,
	},
	{
		id: 6,
		title: "Title 6",
		description: "Description",
		url: "https://picsum.photos/id/75/800/800",
		price: 1199,
	},
	{
		id: 7,
		title: "Title 7",
		description: "Description",
		url: "https://picsum.photos/id/76/800/800",
		price: 1099,
	},
	{
		id: 8,
		title: "Title 8",
		description: "Description",
		url: "https://picsum.photos/id/77/800/800",
		price: 2299,
	},
	{
		id: 9,
		title: "Title 9",
		description: "Description",
		url: "https://picsum.photos/id/78/800/800",
		price: 2999,
	},
	{
		id: 10,
		title: "Title 10",
		description: "Description",
		url: "https://picsum.photos/id/79/800/800",
		price: 1999,
	},
	{
		id: 11,
		title: "Title 11",
		description: "Description",
		url: "https://picsum.photos/id/80/800/800",
		price: 1999,
	},
	{
		id: 12,
		title: "Title 12",
		description: "Description",
		url: "https://picsum.photos/id/81/800/800",
		price: 1055,
	},
]
</script>
