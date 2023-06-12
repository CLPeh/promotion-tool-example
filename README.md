# PromotionTool
### Introduction  
Promotion is one of the feature of the project in order to attract new players as well as retaining regular players. Below are the introduction of the promotion:

1. The players could win the prize multiplier that has been set based on the probability, for example x5 x20 x50 times.
2. The prize multiplier will be used to determine the final prize amount (current bet x multiplier won).
3. The chance to win the prizes is the players’ current bet amount must hit the minimum bet required to be eligible.  
For example, the minimum bet set = 10.00 CNY. Hence, the players are only eligible to have a chance to win the prizes when their current bet is at least 10.00 CNY.  
4. However, the maximum bet has also been set. If the player bet exceeds the maximum bet, then the extra bet amount will not be counted.  
**For example**:  
Maximum bet = 100.00 CNY,   
Prize multiplier won = x100,  
Current bet amount = 200.00 CNY  
The player A current bet amount is 200.00 CNY, then the total prize won is 10,000.00 CNY (100.00 CNY x 100).  

### Promotion Type
<details><summary> Money Rain </summary>
   
  No fixed prize within the specific time range set for each day.  
  
  **How the Player Award Prize**
1. The prize amount could be won by the players unlimitedly(no limited prize amount) within the promotion time range.  
i.e. Players could win the prizes without a limit within 1pm-3pm at 30-03-2023 to 03-04-2023.
-------
  
  </details>
<details><summary> Money Rain Daily Bonus </summary>
  
  Prize release in the specific time that has been generated in the prize pool, but the prizes list are not visible by the players, the players are not able to see the prize list.  
  
**How the Player Award Prize**  
1. The prizes were pre-generated and it is distributed evenly among the event period based on the total prize count.  
i.e. If 1-4-2023 00.00.00 am to 1-4-2023 23.59.59 pm total prize count is 24 that means 1 hour will release 1 prize (1 prize/hr);   
If the total prize is 48 that means half hours will release 1 prize (2 prizes/hr).  
  
**How the Settings**
1. A Base Currency(default), Bet Range and Prize Count must be set to generate the prizes pool.
2. Base Currency - To ensure all the prizes generated have a standardized currency.
3. Bet Range - The multiple bet range is set to assign the min bet and max bet for each of the prizes based on the 2 close numbers as the bet range.  
i.e. The bet range is 2, 5, 10, 30, 50, 100. Then, the Min Bet = 2 and Max Bet = 5 or the Min Bet = 5, Max Bet = 10, and etc.
4. Prize Count - To set the prize amount for the different prize multipliers such as 1 prize for x100, 2 prizes for x50, 25 prizes for x30 and etc..
5. Time Before Win Probability Increases - The win probability will increase by dropping the Min Bet required to the smallest bet range if the prize is remaining in undistributed status after the time set.  
i.e Based on Figure 1, the Time Before Win Probability Increases is set at 1 hour, then if the prize is still remaining distributed status the Min Bet will drop to 2 to increase the probability for the players to win the prize.
------
  
  </details>
<details><summary> Daily Cashpot </summary>
  
Prize release in the specific time that has been generated in the prize pool, the prizes are visible by the players, the players are able to see the prize list.  

**How the Player Award Prize**  
The way that players could award the prize of this promotion is basically the same as the Money Rain Daily Bonus.
   
**How the Settings**  
1. The settings of this promotion are the same as the Money Rain Daily Bonus.
------
  
  </details>

### Technologies Used
Front-end: HTML, CSS, JavaScript, React.js  
Back-end: .NET Core, .NET Standard  
Database: MySQL, Redis  
Authentication: JWT (JSON Web Tokens)  
  

## Need Help?
Kindly refer to the guidelines and documentation related to this topic.
<details><summary> Contributing Guidelines </summary>

  - [Question or Problem](./src/contributing-guildelines.md#question)
  - [Issues and Bugs](./src/contributing-guildelines.md#issue)
  - [Feature Requests](./src/contributing-guildelines.md#feature)
  - [Submmiting a Pull Request](./src/contributing-guildelines.md#pullrequest)
  - [Contributor License Agreement](./src/contributing-guildelines.md#cla)

</details>
<details><summary> Development Setup </summary>

  - [Prerequisites](./src/dev-setup.md#prerequisites)
  - [Installation](./src/dev-setup.md#installation)
  - [Database Setup](./src/dev-setup.md#database-setup)
  - [Common Setup Issue](./src/dev-setup.md#failed-to-build-project)
  - [Contributing](./src/dev-setup.md#contributing)

</details>
<details><summary> API and Grpc </summary>

  - [API Endpoints](./src/api-interfaces.md#api-endpoints)
  - [Grpc](./src/api-interfaces.md#grpc-services)
  - [Management Grpc](./src/api-interfaces.md#management-grpc-services)

</details>
<details><summary> Architecture and Design </summary>

  - [Coding Architecture](./src/architecture-design.md#coding-architecture)
  - [Folder Structure](./src/architecture-design.md#folder-structure)
  - [Design Pattern](./src/architecture-design.md#design-patterns)

</details>

- [Testing and Quality Assurance](./src/unit-testing.md)
- [Release Notes](https://github.com/CLPeh/promotion-tool-example/releases)
- [Issues Tracking and Bugs Report](./src/bug-report.md)
