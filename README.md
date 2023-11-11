# Delivery_Duration_Prediction
DoorDash Delivery Duration Prediction
Overview
This data project serves as a take-home assignment for data science positions at DoorDash. The goal is to build a model predicting the estimated time for a delivery from the time a consumer submits an order to when it is delivered.

Data Description
The dataset, historical_data.csv, includes a subset of DoorDash deliveries from early 2015 in select cities. Each row represents a unique delivery, with features including time, store details, order information, and market characteristics.

Time Features
market_id: City/region where DoorDash operates.
created_at: UTC timestamp when the consumer submitted the order.
actual_delivery_time: UTC timestamp when the order was delivered.
Store Features
store_id: Unique identifier for the restaurant.
store_primary_category: Cuisine category of the restaurant.
order_protocol: Identifier for the order protocol.
Order Features
total_items: Total number of items in the order.
subtotal: Total order value (in cents).
num_distinct_items: Number of distinct items in the order.
min_item_price: Price of the least expensive item (in cents).
max_item_price: Price of the most expensive item (in cents).
Market Features
total_onshift_dashers: Number of available dashers within 10 miles of the store.
total_busy_dashers: Subset of on-shift dashers currently working on an order.
total_outstanding_orders: Number of orders within 10 miles being processed.
Predictions from Other Models
Models provide predictions for different delivery stages:

estimated_order_place_duration: Time for the restaurant to receive the order (in seconds).
estimated_store_to_consumer_driving_duration: Estimated travel time between store and consumer (in seconds).
Task
Build a model to predict the total delivery duration in seconds, from order submission to delivery.
