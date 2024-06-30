# [pwn] phase_coffee_2

Points: 487

Difficulty: medium

Surely all the bugs have been fixed...

This challenge is **part 2** out of 3 challenges.

Completing this challenge will unlock 1 challenge.

Author: Sheepiroo

`nc chals.jellyc.tf 5001`

<details>
<summary>View Hint</summary>

The data type of `coin_balance` is relevant

</details>

<details>
<summary>View Hint</summary>

Integer underflow

</details>

<details>
<summary>View Hint</summary>

A 32-bit integer has a minimum value of `-(2^31) = -2147483648`. Subtracting further will cause `coin balance` to underflow to a large positive number. How many coffees do you need to buy for this to happen?

</details>

<style>
details summary { 
    cursor: pointer;
}
</style>

Files: [phase_coffee_2.zip](./phase_coffee_2.zip)

##
