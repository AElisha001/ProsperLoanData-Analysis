# (Prosper loan data analysis)


## Dataset

> The data for this investigation is gotten from prosper.com. The dataset contains information on borrowers' profile, and listing informations. prosper is an online peer-to-peer lending marketplace, where credit worthy borrowers can request a loan and investors can invest in "notes" (or portions) of each loan [ref](www.prosper.com/invest-t1). Basically, the aim of this analysis is to investigate how income levels of borrowers who seek loan on prosper actually influence the loan process. 
It is however, a known fact that income plays an important role in loan sourcing. A higher income provides much more security to obtaining loans not only faster, but as well the amount of loan one could possibly get. Hence the focus of this analysis is to investigate income levels of borrowers and how it interacts with other variables in the dataset. There is a total of 81 columns in the dataset, however, I will be limiting the analysis to only 9 variables of interest. The respective columns are;

>- **LenderYield**: The lender yield on the loan. Lender yield is equal to the interest rate on the loan less than the service fee
>- **IsBorrowerHomeowner**: A Borrower will be classified as a homeowner if they have a mortage on their credit profile or provide documentation. 
>- **BorrowerRate**: The Borrower's interest rate for this loan.
>- **CurrentlyInGroup**: Specifies whether or not the Borrower was in a group at the time the Listing was created.
>- **AvailableBankcardCredit**: The total available credit via bank card at the time the credit profile was pulled.
>- **BorrowerState**: The two letter abbreviation of the state of the address of the Borrower at the time the Listing was created.
>- **Occupation**: The occupation selected by the Borrower at the time they created the Listing.
>- **EmploymentStatus**: The employment status of the Borrower at the time the posted the Listing.
>- **IncomeRange**: The income range of the Borrower at the time the Listing was created.

## Summary of Findings

> From the analysis, the following are noted: borrower rate generally decreases across income range on average, with the open credit lines taking the opposite of that direction across the income range levels. From the distribution of borrowers' states by income levels, a bulk of borrowers are in the \$25,000-49,999 range, with the least number on \$0. Furthermore, a plot of income range and isborrowerhomeowner suggests that most of the middle to high income earners own homes (\$50,000-99,999), whereas, comparatively, fewer borrowers earning less than this mark own homes. A facet plot of isborrowerhomeowner and borrowerstate indicates a balanced distribution of borrowers who own homes and those who do not. A multivariate plot of borrowerrate, currentlyingroup and isborrowerhomeowner indicates a slightly higher borrower rate on average for borrowers who are home owners but do not belong in groups than borrowers who own homes and belong in groups. Additionally, lenderyield per income range decreases across the currentlyingroup variable with borrowers who do not belong in groups having the highest lenderyield. Also, a multivariate plot of opencreditlines, incomerange and isborrowerhomeowner further indicates a higher number of opencredit lines for borrowers who are home owners as earlier seen in the violin plot of opencreditlines and incomerange, only this time, the third variable amplifies the results.

## Key Insights 

> The relationship between BorrowerRate and IsBorrowerHomeowner: It is observed that there is a higher borrower rate on average linked to borrowers who do not own a home than borrowers who own homes, at the time of the listing.
> The relationship between IncomeRange and IsBorrowerHomeowner: It is observed that most of the borrowers earning atleast \$50,000 are home owners. Fewer Borrowers earning below this mark are home owners.
> The relationship between IncomeRange and BorrowerRate: It is observed from the analysis that the borrower rate decreases across levels of the income range variable on average.
> The CurrentlyInGroup variable indicates that a larger proportion of borrowers belong in a group with a few borrowers not identifying with any group.
> The relationship between LenderYield, IncomeRange and CurrentlyInGroup: A multivariate visualization of these variable indicates that lender yield is higher on the income range for borrowers who do not belong in a group than for than for borrowers who belong in groups.
