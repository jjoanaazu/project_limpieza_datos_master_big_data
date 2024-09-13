# Proyecto Limpieza de Datos MSc Big Data Science
### Trabajo de Preparación y Limpieza de Datos. Predecir si el cliente de un hotel va a cancelar o no una reserva.
- Joaquín Joana Azuara - Máster Big Data Science - Universidad de Navarra
- LinkedIn: https://www.linkedin.com/in/joaqu%C3%ADn-joana-azuara-92911a21b/
- Fuente: Kaggle https://www.kaggle.com/datasets/ahsan81/hotel-reservations-classification-dataset


Contexto
No hay ninguna duda de que a los hoteles no les interesa que se cancelen reservar de habitaciones por motivos económicos (tanto desde el punto de vista de los beneficios como de los costes fijos (CF) y variables (CV)). Por ello, considero que sería de gran interés que las cadenas hoteleras puedan predecir con un relevante nivel de seguridad, si un cliente puede llegar a cancelar una reserva según las características de este.


Algunos de los intereses que tienen los hoteles en todo esto son:


Maximizar la ocupación: si el hotel es capaz de predecir con precisión cuántos clientes van a cancelar la reserva, puede ajustar su estrategia de precios para así maximizar la ocupación y minimizar las habitaciones vacías. Incluso dentro de esta misma estrategia, se pueden establecer precios dependiendo del margen de cancelación que se deje (por ejemplo, no tendría el mismo precio una habitación que deja un margen de cancelacion de la reserva de una semana que de otra que deja un mes. Serían más caras y más baratas respectivamente).


Reducción de los costes: si por ejemplo, el hotel ofrece una gran variedad de servicios y la ocupación rondara un 70%, podría minimizar costes variables (CV) pudiendo prescindir de algunos servicios...


Capacidad de tomar medidas con antelación: Si el modelo es realmente fiable, es decir, que me clasifica correctamente las que sí se cancelan de las que no se cancelan. Si se lograra este grado de fiabilidad, los hoteles serían capaces de hacer contraofertas a aquellos clientes que tienen posibilidades de que cancelen sus reservas. Es importante que el modelo sea fiable, porque si no, podemos estar haciendo ofertas a usuarios que no nos interesa hacérsolo.


Variables


- Booking_ID: Identificador único de cada reserva
- no_of_adults: numero de adultos
- no_of_children: numero de niños
- no_of_weekend_nights: Número de noches de fin de semana (sábado o domingo) en el que el huésped se alojó o reservó para - - alojarse en el hotel
- no_of_week_nights: Número de noches de semana (de lunes a viernes) que el huésped se alojó o reservó para alojarse en el hotel
- type_of_meal_plan: Tipo de régimen de comidas reservado por el cliente:
- required_car_parking_space: ¿El cliente necesita una plaza de aparcamiento? (0 - No, 1- Sí)
- room_type_reserved: Tipo de habitación reservada por el cliente. Los valores son cifrados (codificados) por INN Hotels.
- lead_time: Número de días entre la fecha de reserva y la fecha de llegada
- arrival_year: Año de llegada
- arrival_month: Mes de llegada
- arrival_date: Día de llegada
- market_segment_type: Designación del segmento de mercado.
- repeated_guest: ¿El cliente es un invitado repetido? (0 - No, 1- Sí)
- no_of_previous_cancellations: Número de reservas anteriores que fueron canceladas por el cliente antes de la reserva actual.
- no_of_previous_bookings_not_canceled: Número de reservas anteriores no canceladas por el cliente antes de la reserva actual
- avg_price_per_room: Precio medio por día de la reserva; Los precios de las habitaciones son dinámicos. (en euros)
- no_of_special_requests: Número total de solicitudes especiales realizadas por el cliente (por ejemplo, piso alto, vista desde la habitación, etc.)
- booking_status: Bandera que indica si la reserva fue cancelada o no. (VARIABLE OBJETIVO)
Objetivo


**El objetivo es ser capaces de precedir si un cliente va a mantener o cancelar la reserva de hotel. Para ello se empleará un modelo de regresión logística (de clasificación).**
