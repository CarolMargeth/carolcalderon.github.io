---
title: My new project
image: /assets/images/etienne-girardet-360034-unsplash.jpg
description: Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nam, voluptatibus, odio. Saepe dolorem magni qui, porro consectetur quia nobis! Doloribus mollitia id labore placeat autem cum rem, dolorum quos nesciunt.
company: Another Company
date:  2023-09-15
layout: post
---
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec lacinia erat et neque fermentum, sit amet interdum eros lobortis. Sed pharetra tincidunt libero, in aliquet diam eleifend a. Ut semper velit nisi, vel imperdiet ipsum ultricies sed. In sit amet sollicitudin orci, a volutpat nulla. Morbi egestas, dolor ac viverra iaculis, felis lacus pellentesque nisi, vitae semper mauris odio ut ipsum. Sed ultrices velit ac maximus varius. Nunc scelerisque est ex, eu interdum risus fringilla eget. Aenean hendrerit in augue lobortis egestas. Praesent posuere enim tincidunt mollis tincidunt. Mauris a dolor tristique, tincidunt est a, tincidunt felis.


<canvas id="myChart" width="400" height="200"></canvas>
<script>
var ctx = document.getElementById("myChart");
var myChart = new Chart(ctx, {
    type: 'bar',
    data: {
        labels: ["Red", "Blue", "Yellow", "Green", "Purple", "Orange"],
        datasets: [{
            label: 'Colors',
            data: [6, 5, 4, 3, 2, 1],
            backgroundColor: [
                'rgba(255, 99, 132, 0.2)',
                'rgba(54, 162, 235, 0.2)',
                'rgba(255, 206, 86, 0.2)',
                'rgba(75, 192, 192, 0.2)',
                'rgba(153, 102, 255, 0.2)',
                'rgba(255, 159, 64, 0.2)'
            ],
            borderColor: [
                'rgba(255,99,132,1)',
                'rgba(54, 162, 235, 1)',
                'rgba(255, 206, 86, 1)',
                'rgba(75, 192, 192, 1)',
                'rgba(153, 102, 255, 1)',
                'rgba(255, 159, 64, 1)'
            ],
            borderWidth: 1
        }]
    },
    options: {
        scales: {
            yAxes: [{
                ticks: {
                    beginAtZero:true
                }
            }]
        }
    }
});
</script>

new line to check how this is working







space



