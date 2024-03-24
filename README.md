# OOP Problem: Competitive Eating Competition Scoreboard

## Description

In this competitive eating competition, participants earn points based on the amount of three different foods they consume. Each food has a different point value:

- Chickenwings: 5 points
- Hamburgers: 3 points
- Hotdogs: 2 points

The task is to create a function that generates a scoreboard based on the participants' consumption data. The scoreboard should include participants' names and their corresponding scores. If multiple participants have the same score, they should be sorted alphabetically by name.

## Functionality

The function `create_scoreboard(participants)` takes a list of participant objects as input. Each participant object contains the following properties:
- `name`: Participant's name (string)
- `chickenwings`: Number of chicken wings consumed (integer)
- `hamburgers`: Number of hamburgers consumed (integer)
- `hotdogs`: Number of hotdogs consumed (integer)

The function calculates the total score for each participant based on the provided consumption data and returns a scoreboard sorted by score. If scores are equal, participants are sorted alphabetically by name.

## Example

```python
participants = [
    {'name': "Habanero Hillary", 'chickenwings': 5 , 'hamburgers': 17, 'hotdogs': 11},
    {'name': "Big Bob" , 'chickenwings': 20, 'hamburgers': 4, 'hotdogs': 11}
]

scoreboard = create_scoreboard(participants)
print(scoreboard)

## Output
[  {'name': "Big Bob", 'score': 134},  {'name': "Habanero Hillary", 'score': 98}]
