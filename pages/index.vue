<script setup>
    const count = useState('count', () => 4);
    let expirienceInfo = [
        {
            year: '2024-наст-время',
            company: 'Venture',
            position: 'Frontend-разработчик',
            description: 'Разработка внутренних сервисов учета по подсчету и визуализации данных о процессах внутри компании. Есть опыт использования ApexCharts, LitePicker, Tabler, Tailwind, Vuex, Axios. Обязаннсоти: внесение изменений, добавление функционала в существующий проект (HTML/CSS/Vue2), составление e-mail письма средствами HTML/CSS/php, запросы к БД (SQL), обработка результатов запроса (php)'
        },
        {
            year: 2020-2023,
            company: '',
            position: 'Учитель программирования',
            description: 'Web-разработка: Обучение основам HTML/CSS, работа с фреймворком Bootstrap. Внедрение javascript в проекты на HTML/CSS. Настройка и взаимодействие проекта с базами данных(PHP/MySQL).'
        }
    ]

</script>
<template>
    <div class="w-160 mx-auto">
        <div class="grid grid-cols-3" v-for="el in expirienceInfo">
            <div @mouseenter="console.log('///')" class="bg-green-100 p-4">
                {{ el.year }}
            </div>
            <div @click="console.log('===')" class=" p-4">
                {{ el.company }}
            </div>
            <div class=" p-4 mulish-500">
                {{ el.description }}
            </div>
        </div>
    </div>
</template>
