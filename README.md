# Coderhouse

#La idea del proyecto es generar un historial de clima y un forecasting del clima, el historial va a servir para entrenar modelos de machine learning, mientras que
el forecasting servirá para predecir la tasa de ausentismo en un hospital. Si bien varias caracteristicas más son necesarias para este modelo, una variable necesaria es el clima, ya que intuyo que es relevante para el modelo.

El primer paso es levantar el container con airflow, para eso es tan simple como realizar un docker compose up, esto levantará el container, luego es necesario entrar a las conexiones de airflow y colocar las credenciales para conectarse a redshift, en mi caso le coloqué el nombre: redshift_coder. Por último debemos colocar Coder_Dag en la carpeta Dags de airflow, una vez allí, Airflow la levantará automáticamente, al tener un schedule programado anteriormente, el mismo correrá todos los días.
