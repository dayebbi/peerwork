# Birthday Problem


## Veridical Paradox
The birthday problem is a veridical paradox: a proposition that at first appears counterintuitive, but is in fact true showing that only 23 individuals are required to reach a 50% probability of a shared birthday. By considering comparisons made between every possible pair of individuals, With 23 individuals, there are (23 × 22) / 2 = 253 pairs to consider, which is well over half the number of days in a year (182.5 or 183).
Real-world applications include a cryptographic attack called the birthday attack, which uses this probabilistic model to reduce the complexity of finding a collision for a hash function, as well as calculating the approximate risk of a hash collision existing within the hashes of a given size of population.


## Calculating the probability
- Compute an apporximate probability; at least two have the same birthday in a group of n people
- For simplicity,
    - Variations in the distribution(leap years, twins, seasonal, or weekday) are disregard
    - Assuming that all 365 possible birthdays are equally likely

Let's say p(n) is the probability of at least two of the n people sharing a birthday, p(n') is the possibility that all n birthdayts are different.

p(n') = 1 x (1 - 1/365) x (1 - 2//365) x (1 - 3/365) x ... x (1 - (n-1)/365))
      = (365 x 364 x 363 x ... (365-n+1)) / 365^n
      = 365!/365^n(365-n)!
![Final_Function] (https://wikimedia.org/api/rest_v1/media/math/render/svg/97247979ca9c9ce1de6ae233eb2ad1f1bca4ea22)


### Example: Conditional probability with 23
P(A) = 1 − P(A')

P(A) = the probability that at least two people in the room have the same birthday
P(A') = the probability that no two people in the room have the same birthday

Let's call event N = probability of person N may not have the same birthday as any of persons 1 through
 N-1
(the event that all 23 people have different birthdays is the same as the event that person 2 does not have the same birthday as person 1, and that person 3 does not have the same birthday as either person 1 or person 2, and so on, and finally that person 23 does not have the same birthday as any of persons 1 through 22)

P(A') = (365/365) x (364/365) x (363/365) x (362/365) x ... x (343/365)
      = (365)^-23 x (365 x 364 x 363 x ... x 343) 
Evaluating equation (2) gives P(A′) ≈ 0.492703
Therefore, P(A) ≈ 1 − 0.492703 = 0.507297 (50.7297%).
