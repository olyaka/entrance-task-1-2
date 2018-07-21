# Задание 1 — найди ошибки

1. index.js - фигурные скобки при импорте initMap, т.к. экспорт из map.js сделан не по default, и в остальном коде не используется export default
2. index.html - <div id="map" style="width: 100vw; height: 100vh"></div>, для разворота карты на всю страницу
3. map.js - myMap.geoObjects.add(objectManager) для добавления ObjectManager к карте    
4. mappers.js - coordinates: [obj.lat, obj.long] - широта и долгота перепутана местами
5. details.js - замена стрелочных функций на обычные для методов для возможности обращения к шаблону через this
6. chart.js - yAxes: [{ ticks: { beginAtZero: true} }], максимум оси y не должен быть равен 0, поскольку это количество дронов 
7. map.js - objectManager.clusters.options.set('preset', 'islands#greenClusterIcons'); надо убрать, чтобы иконки кластеров раскрашивались в соответствии с нужными цветами
