<script setup>
    const count = useState('count', () => 4);
    let expirienceInfo = [
        {
            year: 2024,
            company: 'ABC Corp',
            position: 'Software Engineer',
            description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed auctor, arcu at consectetur luctus, velit ligula tristique velit, non fermentum velit lectus vel velit.'
        },
        {
            year: 2022,
            company: 'XYZ Inc',
            position: 'Senior Software Engineer',
            description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed auctor, arcu at consectetur luctus, velit ligula tristique velit, non fermentum velit lectus vel velit.'
        }
    ]

</script>
<template>
    <div class="w-160 mx-auto">
        <div class="p-6 grid grid-cols-2" v-for="el in expirienceInfo">
            <div @mouseenter="console.log('///')" class="bg-red-100">
                {{ el.year }}
            </div>
            <div @click="console.log('===')">
                {{ el.company }}
            </div>
        </div>
    </div>
</template>
