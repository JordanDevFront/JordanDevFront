# Dashboard de Tecnologias

![Dashboard](https://user-images.githubusercontent.com/your-image-here.png)

Este dashboard exibe um gráfico das tecnologias que você domina.

```html
<canvas id="myChart" width="800" height="400"></canvas>
const ctx = document.getElementById('myChart').getContext('2d');
const myChart = new Chart(ctx, {
    type: 'bar',
    data: {
        labels: ['Node', 'React', 'HTML', 'CSS', 'Fastify', 'PostgreSQL', 'SQL Server', 'JavaScript'],
        datasets: [{
            label: 'Domínio das Tecnologias',
            data: [8, 7, 9, 8, 6, 7, 6, 9], // Adicione aqui a pontuação de domínio para cada tecnologia
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
                'rgba(255, 206, 86, 0.2)',
                'rgba(75, 192, 192, 0.2)',
                'rgba(153, 102, 255, 0.2)',
                'rgba(255, 159, 64, 0.2)',
                'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
            ],
            borderColor: [
                'rgba(255, 99, 132, 1)',
                'rgba(54, 162, 235, 1)',
                'rgba(255, 206, 86, 1)',
                'rgba(75, 192, 192, 1)',
                'rgba(153, 102, 255, 1)',
                'rgba(255, 159, 64, 1)',
                'rgba(255, 99, 132, 1)',
                'rgba(54, 162, 235, 1)',
            ],
            borderWidth: 1
        }]
    },
    options: {
        scales: {
            y: {
                beginAtZero: true
            }
        }
    }
});
