<template>
    <indexJumbotron :items="sliderData" class="mb-5"/>
</template>

<script>
import indexJumbotron from '../components/indexJumbotron.vue';

export default {
	name: "Homepage",
	components: { indexJumbotron},
data() {
        return {
    sliderData : [
        {
        title: "Category",
        caption: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere laboriosam illum adipisci? Minima laudantium velit repellat quia, iure voluptatem nemo. Quod debitis eaque beatae repellendus veritatis placeat praesentium voluptate consequuntur!",
        img : "https://picsum.photos/seed/dolet/1519/512",
        
        },
        {
        title: "Category",
        caption: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere laboriosam illum adipisci? Minima laudantium velit repellat quia, iure voluptatem nemo. Quod debitis eaque beatae repellendus veritatis placeat praesentium voluptate consequuntur!",
        img : "https://picsum.photos/seed/lorem/1519/512",
        
        },
        {
        title: "Category",
        caption: "Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere laboriosam illum adipisci? Minima laudantium velit repellat quia, iure voluptatem nemo. Quod debitis eaque beatae repellendus veritatis placeat praesentium voluptate consequuntur!",
        img : "https://picsum.photos/seed/ipsum/1519/512",
        
        },

    ],
    };
    },
};
</script>

<style lang="scss" scoped>
</style>