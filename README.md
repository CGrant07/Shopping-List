NumberOfRecipes = int(input("How many meals are you planning? "))
ListOfMeals = []
Ingredients = {}
ListOfIngredients = []
for meals in range(NumberOfRecipes):
    ListOfMeals.append(input("List one of the meals: "))

print(ListOfMeals)
for i in range(NumberOfRecipes):
    while True:
        Ingredient = str(input("what is an ingredient in " + ListOfMeals[i] + "? "))
        print(Ingredient)
        if Ingredient == "next":
            ListOfIngredients = []
            break
        else:
            ListOfIngredients.append(Ingredient)
            Ingredients[ListOfMeals[i]] = ListOfIngredients
            print(Ingredients)


