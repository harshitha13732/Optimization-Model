# Optimization-Model

*COMPANY*: CODTECH IT SOLUTIONS

*NAME*: GARLAPATI HARSHITHA

*INTERN ID*: CT08DZ2406

*DOMAIN*: DATA SCIENCE

*DURATION*: 6 WEEKS (AUG-2ND 2025 TO SEP-17TH 2025)

*MENTOR*: NEELA SANTOSH

*DESCRIPTION*: 

Bakery Production Optimization Model

>Introduction

Running a bakery is not just about baking delicious bread, cakes, and pastries—it’s also about making smart business decisions. Every bakery has limited resources like workers’ time, oven capacity, and flour. At the same time, customers demand certain quantities of products, and each product gives a different level of profit.

This project uses Optimization Techniques (Linear Programming and Integer Programming) to answer an important question:
-->“How many breads, cakes, and pastries should the bakery produce to maximize profit without running out of resources?”


>Problem Setup

We have three products:

-->Bread – Low profit but requires fewer resources.

-->Cake – Higher profit but consumes more labour, oven hours, and flour.

-->Pastry – Balanced in terms of profit and resources.

Each of these products has:

-->Profit per unit (e.g., Cake = 8 units of profit),

-->Resource requirements (labour hours, oven hours, flour),

-->Demand limits (maximum number of items customers want).

The bakery also has fixed capacities:

-->100 labour hours,

-->50 oven hours,

-->60 kg of flour.


>Building the Optimization Model

We use the PuLP library in Python to build the model. Here’s how it works:

Decision Variables → How many units of Bread, Cake, and Pastry to produce.

Objective Function → Maximize total profit across all products.


Constraints →

-->Total labour used ≤ 100 hours

-->Total oven time used ≤ 50 hours

-->Total flour used ≤ 60 kg

-->Each product ≤ demand limit

We solve this problem in two ways:

-->Continuous Model (LP): Allows fractional production (e.g., 25.5 cakes). Useful for analysis.

-->Integer Model (IP): Only whole numbers (e.g., 25 cakes). This is realistic for a real bakery.


>Visualizing Results

After solving, we visualize the results with Matplotlib:

-->Bar charts showing how many of each product should be made.

-->Bar charts showing profit contribution of each product.

This makes it easier for bakery managers to understand the solution instead of just looking at numbers.


>Sensitivity Analysis

What if the bakery had more workers or fewer?

We test different values of labour hours (from 80 → 120) and see how profit changes. This helps the bakery answer:

-->“If I hire 10 extra workers, how much more profit can I make?”


>Resource Usage and Slack

The model also calculates:

-->Resource used → e.g., 95 labour hours.

-->Slack (leftover capacity) → e.g., 5 hours not used.

This shows which resources are bottlenecks. If flour is fully used but labour is not, it means flour is the main limitation.


>Real-World Applications

This model is not just for bakeries—it’s useful anywhere resources are limited:

-->Manufacturing: Deciding how many products to make with limited machines and materials.

-->Restaurants: Choosing menu items based on kitchen and staff limits.

-->Supply Chains: Optimizing warehouses, trucks, and stock.

-->Project Management: Allocating budget, manpower, and time.


This project shows how mathematical optimization helps businesses make better decisions. Instead of guessing, the bakery can calculate the best production plan that maximizes profit while respecting real-world limits.

In simple terms:

-->The bakery makes smarter choices, uses resources wisely, and earns more profit.


*OUTPUT*:

