# Assignment1
## MSDS 460 Homework Assignment 1 -- Linear Programming Example 
Bailey Scoville

## Objective
The objective of this linear programming problem is to find the combination of the five foods that minimizes my weekly food costs while ensuring I ingest the weekly recommended amounts of sodium, energy, protein, vitamin D, calcium, iron, and potassium.

## Foods
 - x1 - Kodiak Cakes® Plant-Based Classic Protein Flapjack & Waffle Mix - $0.79 per serving
 - x2 - Kirkland Signature Cheese, Fruit & Nut Snack Packs - $0.85 per serving
 - x3 - Trader Joe’s Tortilla Española - $ 0.92 per serving
 - x4 - BOOST Original Balanced Nutritional Powder Drink Mix, Very Vanilla - $1.42 per serving
 - x5 - Trader Joe’s Indian Fare Madras Lentils - $1.25 per serving
 - NOTE - images of nutrition labels are included in the [repository](https://github.com/bscov/Assignment1)

## Standard Form Equation - Original Problem
 - Objective function: Min Z = (6.29/8)*x1 + (13.59/16)*x2 + (5.49/6)*x3 + (33.99/24)*x4 + (2.49/2)*x5
 - Subject to:
 - 440x1 + 160x2 + 320x3 + 170x4 + 510x5 + x6 = (5000*7) - maximum sodium (mg)
 - 230x1 + 180x2 + 150x3 + 220x4 + 150x5 + x7 = (2000*7) - minimum energy (kcal)
 - 14x1 + 8x2 + 5x3 + 10x4 + 7x5 + x8 = (50*7) - minimum protein (g)
 - 1x1 + 0.1x2 + 0.2x3 + 6x4 + 0.1x5 + x9 = (20*7) - minimum vitamin D (mcg)
 - 24x1 + 150x2 + 30x3 + 260x4 + 40x5 + x10 = (1300*7) - minimum calcium (mg)
 - 3x1 + 0.4x2 + 0.8x3 + 3.6x4 + 2.1x5 + x11 = (18*7) - minimum iron (mg)
 - 155x1 + 80x2 + 320x3 + 290x4 + 360x5 + x12 = (4700*7) - minimum potassium (mg)
 - xi ≥ 0, ∀ i

## Tools
The linear programming code utilizes the Python PuLP library to minimize the cost function.

## Results
### Original Problem
The optimal solution includes only two of the five foods: Tortilla Española (x3) and BOOST Drink Mix (x4). To meet the weekly dietary constraints, I would need to eat 79.4 servings of Tortilla Española and 25.84 servings of BOOST Drink Mix. The total of this diet is $109.24. 

### Altered Problem
To meet the weekly dietary constraints and include at least one serving of each food, I would need to consume 1 serving of Kodiak Cakes Mix, 1 serving of Cheese, Fruit & Nut Packs, 78.15 servings of Tortilla Española, 25.16 servings of BOOST Drink Mix, and 1 serving of Madras Lentils. The total of this diet is $110.02, only $0.78 more than the original recommended diet. 

