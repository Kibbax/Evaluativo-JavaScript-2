
#Global Learning - Municipalidad de Yerba Buena - 2023 
#Evaluativo JavaScript

14 de Junio de 2023 - Límite: 24 de Junio de 2023 
Criterios de evaluación
El problema a resolver consta de una consigna en la cual se detalla la funcionalidad que deben
programar. Los criterios de evaluación son los siguientes:
● La función será evaluada mediante 5 testeos independientes. Cada test superado
equivale a +2 de la nota final.
● Se evaluará el código limpio y organizado. +2 .
● Nombres de variables y funciones en inglés. +1 .
● Código declarativo. +1 .
● Código documentado. +1 .
● Creatividad a la hora de manipular el DOM con JavaScript. Min: +1 | Max: +5.
Nota máxima si se consideran todos los apartados realizados con buenas prácticas:
● Nota máxima: 20 / 20.
Criterios de entrega
La resolución del problema debe estar en un archivo javascript individual con el siguiente
nombre dentro de una carpeta /scripts que se encuentre en el directorio raíz del repositorio:
● movies-filter.js
El ejercicio deberá respetar el nombre de la función indicado en el enunciado y ser entregado en
un repositorio de GitHub junto a la implementación con HTML y CSS de una landing page. La
web debe permitir interactuar con filtros (botones y/o inputs) para ir obteniendo y mostrando en
pantalla los resultados correspondientes haciendo uso de la función desarrollada. Se tendrá en
consideración el apartado visual en caso de que no se superen todos los apartados necesarios
mencionados en los criterios de evaluación.

#Problema USERS ( 1 ) MOVIES ( 2 )
En base a una lista de usuarios y una lista de películas vistas por dichos usuarios, realizar una
función que permita obtener un nuevo arreglo de objetos en el cual cada objetos consta con el
nombre del usuario, su email, su dirección completa, su compañía, el título de la película vista y
la calificación de la misma. La función debe poseer un filtro por fecha, por calificación y por id
de usuario. Si no se envía un userId, la función deberá devolver todas las películas que cumplan
las condiciones de los filtros de fecha y calificación para todos los usuarios existentes.
Nombre de función y parámetros necesarios:
filterMovies({ users, movies, userId, fromDate, toDate, rate });
Cada objeto del arreglo debe tener la siguiente estructura:
{
id: user.id,
username: user.username.
email: user.email,
fullAddress: `${user.address.street} - ${user.address.city}`
company: user.company.name,
movie: movie.title,
rate: movie.rate
}





[
  {
    "userId": 10,
    "id": 1,
    "title": "The Godfather",
    "genre": "Thriller",
    "watched": "2022-04-01 09:40:48",
    "rate": 7.6,
    "image": "https://i.ebayimg.com/images/g/X~cAAOSwz2ZiaB2w/s-l1600.jpg"
  },
  {
    "userId": 7,
    "id": 2,
    "title": "The Texas Chain Saw Massacre",
    "genre": "Horror",
    "watched": "2020-05-25 13:11:24",
    "rate": 7.4,
    "image": "https://m.media-amazon.com/images/I/91ei8JE0SDL.jpg"
  },
  {
    "userId": 1,
    "id": 3,
    "title": "The Shining",
    "genre": "Horror",
    "watched": "2022-02-24 00:21:22",
    "rate": 5.8,
    "image": "https://cdn.posteritati.com/posters/000/000/061/864/the-shining-md-web.jpg"
  },
  {
    "userId": 3,
    "id": 4,
    "title": "Toy Story",
    "genre": "Animation|Children|Comedy|Fantasy",
    "watched": "2022-06-17 23:21:12",
    "rate": 5.9,
    "image": "https://m.media-amazon.com/images/I/71aBLaC4TzL.jpg"
  },
  {
    "userId": 8,
    "id": 5,
    "title": "Halloween: The Curse of Michael Myers",
    "genre": "Horror|Thriller",
    "watched": "2020-04-18 15:47:33",
    "rate": 0.7,
    "image": "https://m.media-amazon.com/images/I/91UHof7cKKL.jpg"
  },
  {
    "userId": 5,
    "id": 6,
    "title": "Die Hard",
    "genre": "Action|Crime|Thriller",
    "watched": "2020-06-15 22:49:31",
    "rate": 3.3,
    "image": "https://cdn.shopify.com/s/files/1/1057/4964/products/Die-Hard-Vintage-Movie-Poster-Original-1-Sheet-27x41-7126.jpg"
  },
  {
    "userId": 2,
    "id": 7,
    "title": "The Dark Knight Rises",
    "genre": "Action|Adventure|Crime",
    "watched": "2022-11-16 04:22:21",
    "rate": 4.7,
    "image": "https://m.media-amazon.com/images/I/81G+2LJQJeL.jpg"
  },
  {
    "userId": 3,
    "id": 8,
    "title": "Fight Club",
    "genre": "Action|Crime|Drama|Thriller",
    "watched": "2022-10-26 07:04:17",
    "rate": 4,
    "image": "https://m.media-amazon.com/images/I/81D+KJkO4SL.jpg"
  },
  {
    "userId": 5,
    "id": 9,
    "title": "Avengers: Infinity War",
    "genre": "Action|Adventure|Sci-Fi",
    "watched": "2022-07-12 20:36:17",
    "rate": 2.8,
    "image": "https://i.ebayimg.com/images/g/kukAAOSw-YZa8mLH/s-l1600.jpg"
  },
  {
    "userId": 7,
    "id": 10,
    "title": "The Hangover",
    "genre": "Comedy",
    "watched": "2020-08-13 01:17:10",
    "rate": 1.4,
    "image": "https://www.tvguide.com/a/img/catalog/provider/1/2/1-172442538.jpg"
  },
  {
    "userId": 4,
    "id": 11,
    "title": "Your Name",
    "genre": "Animation|Drama|Fantasy|Romance",
    "watched": "2020-10-06 00:08:50",
    "rate": 1,
    "image": "https://i0.wp.com/www.septimacaja.com/wp-content/uploads/xq1Ugd62d23K2knRUx6xxuALTZB.jpg"
  },
  {
    "userId": 9,
    "id": 12,
    "title": "How to Train Your Dragon",
    "genre": "Adventure|Animation|Children|Fantasy",
    "watched": "2022-01-11 23:06:04",
    "rate": 9.1,
    "image": "https://m.media-amazon.com/images/M/MV5BMjA5NDQyMjc2NF5BMl5BanBnXkFtZTcwMjg5ODcyMw@@._V1_FMjpg_UX1000_.jpg"
  },
  {
    "userId": 8,
    "id": 13,
    "title": "Robin Hood",
    "genre": "Adventure|Animation|Children|Comedy|Musical",
    "watched": "2021-08-05 18:57:45",
    "rate": 5.8,
    "image": "https://pics.filmaffinity.com/Robin_Hood-466796044-large.jpg"
  },
  {
    "userId": 6,
    "id": 14,
    "title": "Whiplash",
    "genre": "Drama|Musical",
    "watched": "2022-04-23 00:44:02",
    "rate": 0.7,
    "image": "https://flxt.tmsimg.com/assets/p10488558_p_v12_ai.jpg"
  },
  {
    "userId": 5,
    "id": 15,
    "title": "Life Is Beautiful",
    "genre": "Comedy|Drama|Romance|War",
    "watched": "2022-05-02 20:00:04",
    "rate": 6.4,
    "image": "https://flxt.tmsimg.com/assets/p22005_p_v8_aa.jpg"
  }
]