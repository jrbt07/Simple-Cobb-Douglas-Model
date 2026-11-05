# Proposal

## What will (likely) be the title of your project?

Simple Cobb-Douglas Utility Model

## In just a sentence or two, summarize your project. (E.g., "A website that lets you buy and sell stocks.")

A program that tells the user the ideal amount to purchase of two goods given a budget constraint

## In a paragraph or more, detail your project. What will your software do? What features will it have? How will it be executed?

The idea is the following:
1). Ask the user for the name of two goods.
2). Ask the user how much does he/she rate the goods in terms of personal preference on a scale of 1-10.
3). Ask the user for the price of each good.
4). Ask the user for the budget he/she wants to allocate for the purchase of these goods.
5). Set up a Cobb-Douglas Function using the user's preferences to get the function's exponents.
6). Set up a budget constraint function based on the given prices and the budget constraint.
7). Get an expression for the Lagrangian: Cobb-Douglas - λ * budget, where λ is a real-valued scalar.
8). Get the different partial derivatives of the lagrangian: one for x, y, and λ.
9). Solve the system of equations obtained from the 3 equations obtained in (8).
10). Summarize the results in a concise message. x is the ideal amount of good 1, y is the ideal amount of good 2, and λ is the additional utility/satisfaction obtained by allocating one more dollar to the budget.
11). Ask the user if he/she wants to try this program for other goods.

The program will deal with incorrect inputs, such as negative budgets or negative prices. It will also alert the user when inapropriate is used, which can happen when entering the rating of a good. For exampel, the user might enter a number that is not in [1,10] or a word. The program will gently ask the user to change the input until a satisfactory response is inputed.

I will assume that goods are fractional: I can buy 1.2 units of something. This is to make the program as precise as possible and to avoid rounding imprecision.

## If planning to combine 1051's final project with another course's final project, with which other course? And which aspect(s) of your proposed project would relate to 1051, and which aspect(s) would relate to the other course?

N.A.

## If planning to collaborate with 1 or 2 classmates for the final project, list their names, email addresses, and the names of their assigned TAs below.

N.A.

## In the world of software, most everything takes longer to implement than you expect. And so it's not uncommon to accomplish less in a fixed amount of time than you hope.

### In a sentence (or list of features), define a GOOD outcome for your final project. I.e., what WILL you accomplish no matter what?

The program will tell the user how much amount of each good to buy given the budget constraint and the marginal utility obtained from an additional dollar added to the budget.

### In a sentence (or list of features), define a BETTER outcome for your final project. I.e., what do you THINK you can accomplish before the final project's deadline?

If I can manage to prompt the user to tell the program is the goods are fractional or not. If fractional, then return decimals as an answer (if applicable), and if not, then round down to obtain an integer.

### In a sentence (or list of features), define a BEST outcome for your final project. I.e., what do you HOPE to accomplish before the final project's deadline?

Graph the Cobb-Douglas function as well as the budget constraint function to give the user a visual representation of the optimization being made.

## In a paragraph or more, outline your next steps. What new skills will you need to acquire? What topics will you need to research? If working with one of two classmates, who will do what?

I will do a bunch of function for each mini task, and one big function that will run when the program is executed. This function, which I will name project(), will contain all the other functions, so it will be the "visible" part of the program.

As for the skills, exception handling might be necessary. I also expect to learn Sympy basics to solve the system of equations and to get the partial derivatives from the lagrangian function. If I decide to go further, learning Matplotlib will help me display the Cobb-Douglas function alognside the budget constraint function that will help the user visualize the math behind the program.
