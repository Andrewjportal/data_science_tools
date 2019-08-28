## Challenge 1

There are 10 kids what to order ice cream. Each one can choose between chocolate, vanilla or strawberry. You'll collect their choices and make one order, something like: 5 chocolate, 3 vanilla and 2 strawberry. How many possible orders can you make, where every flavor is represented (8c, 1v, 1s is valid but 8c, 2v, 0s is not valid)?

**Answer #1:** If you write out the possibilities, chocolate can be between 8 to 1. If chocolate is 8, there is only one option for vanilla, which is 1. If chocolate is 7, there are two options for vanilla (1 or 2), and so on. If we sum up those options, we get our answer, 1+2+3+4+5+6+7+8 = 36.

**Answer #2:** You want two dividers between 1 and 10 to split the orders. The first block will be chocolate, the second vanilla and third strawberry. There are 9 gaps (between 1 and 10). The order of the two choices doesn't matter. So it's 9C2, which is 9x8/2 = 36.


## Challenge 2

Six individuals are sitting in a circle. I have six cards, three red and three blue. If I randomly hand each one a card, what is the probability that the colors would perfectly alternate, that is no two adjacent person has the same color?

**Answer:** What the first person (player 0) gets doesn't matter. With the color he got, there are 2 more left and we have to choose 2 from the other 5 to get that color. That's 5C2 = 5x4/2 = 10. Of those ten, only one suits our need: player 2 and 4 getting that color. So the probability is 1/10 = 0.1.
