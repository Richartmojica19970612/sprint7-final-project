# sprint7-final-project

# Proyecto ConnectaTel - Análisis de Usuarios y Uso

## 🎯 Objetivo
Analizar los datos de clientes y su comportamiento de uso (mensajes, llamadas y minutos) para:
- Detectar problemas de calidad en los datos.
- Identificar segmentos de clientes según edad y nivel de uso.
- Encontrar patrones de consumo y outliers.
- Generar conclusiones accionables para la mejora de planes y estrategias comerciales.

## 📂 Datasets utilizados
- **users_latam.csv** → Información de clientes (edad, ciudad, plan, fecha de registro).
- **usage.csv** → Registros de uso (tipo de evento: llamadas o mensajes, duración, longitud).
- **plans.csv** → Información de planes disponibles (Básico, Premium).

## 🔎 Etapas del análisis
1. **Exploración inicial (EDA)**  
   - Revisión de estructura, tipos de datos y valores nulos.  
   - Detección de sentinels y valores inválidos (ej. edad = -999).  

2. **Diagnóstico de nulos (MAR)**  
   - Confirmación de que los nulos en `duration` y `length` dependen de `type`.  

3. **Agregación de uso por usuario**  
   - Cantidad de mensajes, llamadas y minutos de llamadas.  
   - Combinación con dataset de usuarios.  

4. **Clasificación de segmentos**  
   - Por nivel de uso: Bajo, Medio, Alto.  
   - Por edad: Joven, Adulto, Adulto Mayor.  

5. **Visualización y detección de outliers**  
   - Histogramas y boxplots para variables clave.  
   - Identificación de patrones extremos de consumo.  

6. **Conclusiones y recomendaciones de negocio**  
   - Segmentos más valiosos.  
   - Oportunidades de mejora en planes y estrategias comerciales.

## ⚙️ Cómo ejecutar el notebook
1. Abre el archivo en **Google Colab**.  
2. Asegúrate de tener los datasets en la carpeta correcta o en tu Google Drive.  
3. Ejecuta las celdas en orden para reproducir el análisis.  

## 📖 Guía de reproducción
- Clona el repositorio:  
  ```bash
  git clone https://github.com/<usuario>/<repositorio>.git
