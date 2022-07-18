<template>
    <div class="flex flex-col w-3/5 h-full mx-auto items-end mt-10">
        <div class="flex gap-x-4">
            <select class="border-b border-gray-400 w-36 text-gray-500" name="" id="">
                <option value="" >color</option>
                <option value="blue" >blue</option>
                <option value="green" >green</option>
                <option value="red" >red</option>
            </select>
            <select class="border-b border-gray-400 w-36 text-gray-500" name="" id="">
                <option value="" >material</option>
                <option value="blue" >aluminum</option>
                <option value="green" >steel</option>
                <option value="red" >carbon fiber</option>
            </select>
            <select class="border-b border-gray-400 w-36 text-gray-500" name="" id="">
                <option value="" >size</option>
                <option value="blue" >small</option>
                <option value="green" >mid</option>
                <option value="red" >big</option>
            </select>
            <button class="bg-black text-white px-3 font-mono">APPLY FILTER</button>
        </div>
        <hr class="w-full mt-8">
        <div class="flex flex-wrap w-full mt-8 gap-y-4">
            <!-- card -->
            <div class="flex flex-col w-56 " v-for="product in products" :key="product.id">
                <div class="w-50 h-50 overflow-clip mb-6 ml-4">
                    <img :src="product.imgSrc" alt="" class="w-full h-auto overflow-clip">
                </div>
                <!-- Slider indicators -->
                <div class="flex w-50 justify-center gap-x-2 mb-2 ml-2">
                    <div class="border w-3 h-3 rounded-full bg-white"></div>
                    <div class="border w-3 h-3 rounded-full bg-white"></div>
                    <div class="border w-3 h-3 rounded-full bg-gray-600"></div>
                    <div class="border w-3 h-3 rounded-full bg-white"></div>
                    <div class="border w-3 h-3 rounded-full bg-yellow-500"></div>
                </div>
                <h1 class="ml-4 mb-4 place-self-center">{{product.productName}}</h1>
                <h1>${{product.price}}</h1>
            </div>
        </div>
        
    </div>
</template>

<script>
    export default {
        data(){
            return{
                products: [
                    {
                        id: '1',
                        imgSrc: 'https://images.unsplash.com/photo-1558981403-c5f9899a28bc?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8M3x8YmlrZXN8ZW58MHx8MHx8&w=1000&q=80',
                        productName: 'Ducatti',
                        price: 75000,
                    },
                    {
                        id: '2',
                        imgSrc: 'https://images.unsplash.com/photo-1558981403-c5f9899a28bc?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8M3x8YmlrZXN8ZW58MHx8MHx8&w=1000&q=80',
                        productName: 'Ducatti',
                        price: 75000,
                    },
                    {
                        id: '3',
                        imgSrc: 'https://images.unsplash.com/photo-1558981403-c5f9899a28bc?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8M3x8YmlrZXN8ZW58MHx8MHx8&w=1000&q=80',
                        productName: 'Ducatti',
                        price: 75000,
                    },
                    {
                        id: '4',
                        imgSrc: 'https://images.unsplash.com/photo-1558981403-c5f9899a28bc?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8M3x8YmlrZXN8ZW58MHx8MHx8&w=1000&q=80',
                        productName: 'Ducatti',
                        price: 75000,
                    },
                    {
                        id: '5',
                        imgSrc: 'https://images.unsplash.com/photo-1558981403-c5f9899a28bc?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8M3x8YmlrZXN8ZW58MHx8MHx8&w=1000&q=80',
                        productName: 'Ducatti',
                        price: 75000,
                    },
                    {
                        id: '6',
                        imgSrc: 'https://images.unsplash.com/photo-1558981403-c5f9899a28bc?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8M3x8YmlrZXN8ZW58MHx8MHx8&w=1000&q=80',
                        productName: 'Ducatti',
                        price: 75000,
                    },
                    {
                        id: '7',
                        imgSrc: 'https://images.unsplash.com/photo-1558981403-c5f9899a28bc?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxzZWFyY2h8M3x8YmlrZXN8ZW58MHx8MHx8&w=1000&q=80',
                        productName: 'Ducatti',
                        price: 75000,
                    },
                ]
            }
        }        
    }
</script>

<style lang="scss" scoped>

</style>