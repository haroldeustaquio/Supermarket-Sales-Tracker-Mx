# Clustering of Sales Transaction

## Project Overview

This project applies clustering techniques to a real-world dataset with the goal of segmenting customers based on their purchasing behaviors and demographic characteristics. By identifying natural customer groupings, the company can enhance its marketing and sales strategies. This analysis focuses on understanding customer behavior across different product sectors, allowing the company to personalize its approach and optimize business outcomes.

## Business Context

The dataset comes from a company aiming to optimize its marketing and sales strategies based on customer behavior. The primary objectives of this analysis are to:

- **Segment Customers**: Group customers into segments based on demographic characteristics (such as age, marital status, education level) and purchasing patterns (such as product preferences, spending habits).
- **Product Sector Analysis**: Analyze product sectors to identify sales trends and customer behavior for specific categories, lines, and sub-lines.
  
By leveraging clustering, the company aims to:
  
- **Personalize Marketing Strategies**: Tailor marketing campaigns to each customer segment, offering relevant products and promotions.
- **Identify New Business Opportunities**: Discover potential markets or customer needs that can be addressed with new product development or expansion into different sectors.
- **Enhance Customer Experience**: Provide more personalized services, improving customer satisfaction and loyalty by understanding their specific needs and preferences.

## Data Description

The dataset contains a wide variety of variables relevant to customer purchases and demographics:

- **Product-related variables**: `Sector`, `Tipo`, `Linea`, `Sublinea`, `Presentacion`, `Gramaje`, `Producto`, `Descripcion`
- **Transaction details**: `Fecha`, `Transaccion`, `Pedido`, `Cantidad`, `Precio`, `Precio_Max`, `Dif_PrecioMax`, `Importe`
- **Customer demographics**: `Cliente`, `Clave_Cliente`, `No._Hijos`, `Antiguedad`, `Edad`, `Edad_Rango`, `Escolaridad`, `Estado_Civil`, `Estado`, `Sexo`
- **Business identifiers**: `Empresa`, `Anio`
- **Other variables**: `Funcion`, `Grupo`

These variables provide detailed insights into the purchasing behavior of clients, allowing the company to better understand both their demographics and how they interact with different product categories.

## Clustering Algorithms Used

The following clustering algorithms were used in this project:

- **K-Means Clustering**: A classic partitioning algorithm that assigns each data point to the closest cluster center based on distance.
- **Agglomerative Clustering**: This is useful for building a hierarchy of clusters, joining data into larger groups based on similarities, starting with each data point as its own cluster. It is particularly effective for discovering hierarchical structure in data.

## Requirements

Make sure you have the following Python libraries installed:

- `pandas`
- `numpy`
- `matplotlib`
- `scikit-learn`