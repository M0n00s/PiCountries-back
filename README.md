# PiCountries-back
## Deploy : https://picountriesback.onrender.com

Backend

Se debe desarrollar un servidor en Node/Express con las siguientes rutas:

IMPORTANTE: No está permitido utilizar los filtrados, ordenamientos y paginados brindados por la API externa, todas estas funcionalidades tienen que implementarlas ustedes.

    GET /countries:
        En una primera instancia deberán traer todos los países desde restcountries y guardarlos en su propia base de datos y luego ya utilizarlos desde allí (Debe almacenar solo los datos necesarios para la ruta principal)
        Obtener un listado de los paises.
    GET /countries/{idPais}:
        Obtener el detalle de un país en particular
        Debe traer solo los datos pedidos en la ruta de detalle de país
        Incluir los datos de las actividades turísticas correspondientes
    GET /countries?name="...":
        Obtener los países que coincidan con el nombre pasado como query parameter (No necesariamente tiene que ser una matcheo exacto)
        Si no existe ningún país mostrar un mensaje adecuado
    POST /activity:
        Recibe los datos recolectados desde el formulario controlado de la ruta de creación de actividad turística por body
        Crea una actividad turística en la base de datos
