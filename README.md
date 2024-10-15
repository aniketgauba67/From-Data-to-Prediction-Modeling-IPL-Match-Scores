# From Data to Prediction: Modeling IPL Match Scores

## Authors
- **Aniket Gauba**
- **Raiyan Islam**

## Project Overview
In this project, we investigate how the number of wickets remaining and the number of overs left influence the runs scored in an Indian Premier League (IPL) game. The IPL, also known as the Indian Premier League, is a professional Twenty20 cricket league in India. Cricket, a sport with a rich history and strategic depth, depends on making informed decisions during a match. By analyzing IPL match data from 2008 to 2023, we aim to develop a prediction model that forecasts run production based on current game conditions.

This model can provide teams with actionable insights, helping them to strategize more effectively in real time and potentially change the outcome of the game. Accurate predictions of run production based on current match conditions can empower coaches and players with a deeper understanding of potential game progressions. This facilitates strategic decisions such as optimizing batting orders and timing the use of key bowlers. Additionally, the model enhances fan engagement by offering a more immersive and interactive experience, helping spectators appreciate the complexities of strategy and probability playing out in real time.

## Data Source and Preparation
We use an open-source R package called **cricketdata** to download ball-by-ball data from **Cricsheet**, a collection of projects that provide detailed data on cricket. The dataset, named **ipl**, includes extensive variables that capture various aspects of the game. This makes it a powerful tool for building our predictive model. Our primary focus is on the variables `balls_remaining` and `wickets_remaining`, as these variables have a significant impact on run-scoring during different phases of a game.

### Key Data Variables:
- **balls_remaining**: The number of deliveries left in the innings.
- **wickets_remaining**: The number of wickets still available to the batting team.
- **runs_scored**: The number of runs accumulated by the team at a given point.

## Methodology
1. **Data Collection**: We gathered match data for all IPL games from 2008 to 2023 using the cricketdata package.
2. **Data Preprocessing**: The data was cleaned and transformed to focus on key variables (balls remaining, wickets remaining, and runs scored).
3. **Feature Engineering**: Additional features like run rate and over-specific performance were created to improve model performance.
4. **Model Selection**: We explored different machine learning models to predict the final score of the game, using regression models to capture the relationship between game conditions and run scoring.
5. **Evaluation**: The models were evaluated using metrics like **Root Mean Squared Error (RMSE)** and **Mean Absolute Error (MAE)** to measure prediction accuracy.

## Results
Our predictive model demonstrated the ability to accurately forecast the final score of an IPL game based on current match conditions. The results showed that the number of wickets remaining and the number of balls left in the game were critical factors in determining the final score.

## Applications
- **Team Strategy**: Teams can use this model to adjust their game plans in real time, optimizing decisions around batting and bowling orders.
- **Fan Engagement**: Fans can interact with the game on a deeper level, using predictions to analyze potential game outcomes and better understand strategic decisions.
  
## Future Work
Future iterations of this project could involve:
- Incorporating more features, such as **player performance metrics** and **weather conditions**, to improve model accuracy.
- Extending the model to other cricket formats like One Day Internationals (ODIs) and Test matches.

## Installation

To set up and run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone <repository_url>
