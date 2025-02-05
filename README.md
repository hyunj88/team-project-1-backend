# GameHub

GameHub is an online database of information relating to video games.

## Technologies Used

- React
- JavaScript
- Mongoose/MongoDb
- CSS

## MVP User Stories

- As an unregistered user, I would like to sign up with email and password.
- As an unregistered user, I would like to see all the games on the game index
- As an unregistered user, I would like to view all other users' games on the game index.
- As an unregistered user, I want the ability to read more details of individual games.
- As a registered user, I would like to sign in with email and password.
- As a signed in user, I would like to change password.
- As a signed in user, I would like to sign out.
- As a signed in user, I would like to add a video game to the game index.
- As a signed in user, I would like to update my video game on the game index.
- As a signed in user, I would like to delete my video game on the game index.
- As a signed in user, I would like to see all my games on the game index.
- As a signed in user, I want the ability to add games to a favorite list
- As a signed in user, I would like to comment on other users' games
- As a signed in user, I would like to edit my comment on other users' games
- As a signed in user, I would like to delete my comment on other users' games

## Reach Goal(s)

- Allow users to reply to comments
- Allow the users to have the ability to search for specific game from a search bar
- Allow the users to have the ability to click on a link in the game show page that directs them to a store where they can purchase the game.

## Route table for documents

#### Games
| Verb   | URI Pattern            | Controller#Action |
|--------|------------------------|-------------------|
| GET    | `/games`               | `games#index`     |
| GET    | `/games/:id`           | `games#show`      |
| POST   | `/games`               | `games#create`    |
| PATCH  | `/games/:id`           | `games#update`    |
| DELETE | `/games/:id`           | `games#delete`    |

#### Users
| Verb   | URI Pattern            | Controller#Action |
|--------|------------------------|-------------------|
| POST   | `/sign-up`             | `users#signup`    |
| POST   | `/sign-in`             | `users#signin`    |
| PATCH  | `/change-password/`    | `users#changepw`  |
| DELETE | `/sign-out/`           | `users#signout`   |

###### Comments
| Verb   | URI Pattern                    | Controller#Action |
|--------|--------------------------------|-------------------|
| POST   | `/comments/gameId`             | `comments#create` |
| PATCH  | `/comments/:gameId/:commentId` | `comments#update` |
| DELETE | `/commments/:gameId/:commentId`| `comments#delete` |

## Entity Relationship Diagrams (ERDs)
<img width="679" alt="Screen Shot 2023-02-13 at 9 02 45 AM" src="https://user-images.githubusercontent.com/85146023/218494314-b8bb8ea8-8a2e-4615-bd5a-6378e8f48e8c.png">

