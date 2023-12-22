# GreenChallenge
Gamified ecological sustainability.

## Motivation
Fighting climate change requires colossal efforts across the globe. Impact by individual contributors is limited, which can be demotivating. 
GreenChallenge remedies this by combining the efforts of contributors across the world, creating a grass-roots movement to bring about the necessary change.

## Functional Concept
At the core, players are encouraged to solve one "challenge" per day.

### Challenges
Challenges come in two sizes: big (L) and small (S).

Challenges can take on various forms:
1. petitions - signing a petition.
1. education - reading / watching something or taking a short quiz.
1. donations - e.g. to various initiatives, projects and organizations that tackel ecological sustainability.
1. and many more

Challenges can fall into one or more category:
1. political: putting pressure on decision makers.
1. economic: changing the economic realities can lead to the current state of warming.
1. mitigation: reducing the impact of global warming in one way or another.
1. motivational: motivating other players to solve challenges and join the movement.


### Gamification
GreenChallange will use a social gamification approach for a high long-term engagement among players.

Gamification elements to be used are:
1. points for a sense of **progress**
1. leaderboards for **social comparison**
1. group activities for **social** effects
1. (badges as elements of extrinsic rewards)

## Implementation Concept

Layered architecture of database <> server <> clients.

### Concept Dictionary
**Challenge**: An action that many players across the world should perform. Can be signing a petition, donating for a cause, going to a demonstration or sharing a post on facebook.

**Daily Challenge**: The specific challenge that is to be performed on a given day.

**Player**: Everybody with an account who will solve challenges.

**Player Action**: The action a player took to solve a challenge.

### Database
A simple database of challenges, players and player actions.

Tables:
* challenges_tbl: 
* daily_challenges_tbl:
* players_tbl:
* player_actions_tbl:

### Server
Responsible for communication between clients and database. Provides the common business logic for actions.

### Clients
Platform-specific clients (bots and UIs) for:
* Discord
* Twitter / X
* Mastodon
* Slack
* Internet