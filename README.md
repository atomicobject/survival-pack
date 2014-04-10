You are a survior of zombie apocalypse. You are moving from town-to-town collecting the most valuable items necessary for survival. You have backpack that can only hold a certain amount of weight and it is your job is to choose the best set of items based on their weight and value.

**Write a API in [Grape](https://github.com/intridea/grape) with an API endpoint called** <code>/v1/survival-pack</code>.

That API endpoint will be given the following data via a <code>POST</code> request:

* a set of survival items with a name and unique weight and value combination
* an overall weight restriction

It will produce an optimal set of survival items which:

* are within the total weight restriction
* maximize your chance of survival

Requirements:

* use bundler - https://github.com/bundler/bundler
* include multiple high-level test cases to validate your solution (like the one included below)
* provide instructions in a README for submitting a survival pack to the API
* deploy it to [Heroku](https://id.heroku.com/login) or similar service

Input:

    max weight: 400

    available survival items:

    name    weight value
    ammo        9   150
    tuna       13    35
    water     153   200
    spam       50   160
    knife      15    60
    hammer     68    45
    rope       27    60
    saw        39    40
    towel      23    30
    rock       52    10
    seed       11    70
    blanket    32    30
    skewer     24    15
    dull-sword 48    10
    oil        73    40
    peanuts    42    70
    almonds    43    75
    wire       22    80
    popcorn     7    20
    rabbit     18    12
    beans       4    50
    laptop     30    10

Result:

    best value:

    name    weight value
    beans       4    50
    popcorn     7    20
    wire       22    80
    almonds    43    75
    peanuts    42    70
    seed       11    70
    rope       27    60
    knife      15    60
    spam       50   160
    water     153   200
    tuna       13    35
    ammo        9   150

Hint:

* read this - http://en.wikipedia.org/wiki/Knapsack_problem

