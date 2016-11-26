# Team
----------
  Joe Iaquinto iaquij@rpi.edu
  Brendan Courson coursb@rpi.edu
  
  Help from Chris Dower @Cdower

# Description
----------

Drops is a flexible event planning web app that simplifies the process to the 5 W’s: Who, What, When, Where, Why, and How? A Drop created by a user can be as detailed or open-ended as they choose by allowing guests to suggest activities, locations, and times they are available. 
Drops provides a sleeker approach to gathering your friends and taking your group chat plans to the real world because Facebook events are too inflexible and cumbersome to set up. Facebook Events Yes/ Maybe/ No does not give reliable data on when you could reschedule to allow more people to join you. Drops will utilize a built in when-is-good system to help Drop creators democratically decide when is best. Other flexible meeting and event planning solutions like [Fasterplan](http://www.fasterplan.com/) are geared towards the business world and lack integration with major social media platforms.

# Goals
----------
## Create the main Drop screen

This will be the core of the user experience in Drops. Users create, edit, and interact with a Drop. It is critical that the Drop creation process be simple and quick to complete. Hopefully Drops can save people time and energy so they can come together with their friends and turn their online plans into real life experiences. 

## Getting Started

- [ ] Create barebones web-app
- [ ] Create editable fields for the Drop ( 5 W’s)

**Who?**

- [ ] Enable Drop invitations
- [ ] Allow admins to set visibility on Drop
- [ ] Degree of separation set by the creator limits the size of the Drop

**What?**

- [ ] Allow Admins to set an activity for the drop
- [ ] Populate field with searchable suggestions for Drop activities
- [ ] Enable straw poll suggestions from users
- [ ] Enable straw poll voting

**When?**

- [ ] Implement custom When-Is-Good system
- [ ] Allow Admins to adjust duration
- [ ] Allow admins to finalize time
- [ ] Notify users that responded to the when-is-good when time is finalized

**Where?**

- [ ] Allow Admins to set a location or create a poll
- [ ] Add custom Where-Is-Good educated polling
 - [ ] Google Places ratings
 - [ ] Straw poll voting

**Why?**

- [ ] Text field for why the Drop was made

## Home

Outside of the Drop screen, there needs to be a place to manage Drops and see what local public Drops are happening.  There also could be a feed of Drops the user’s friends are going to.

- [ ] Allow users to view invites
- [ ] Allow users to view upcoming and past Drops
- [ ] Allow users to see local public Drops
- [ ] Allow users to see what Drops their friends are going to

## Bonus Drop Features

- [ ] Advanced Drop permission control
 - [ ] Allow admins of the Drop to be set other than the Creator
- [ ] Enable commenting on Drops
 - [ ] Stickied comments for Admins

## Moonshots

- [ ] Make web and mobile web friendly
- [ ] Venmo or Tilt integration for Drop funding
- [ ] Add Messenger and Slack Drops integration to create a drop right from a group chat
- [ ] Automatically make a messenger group/ slack channel for the Drop.
  




# Forked from [Phoenix hipster stack](https://github.com/graphql-elixir/phoenix-hipster-stack)!
* [Phoenix] (http://www.phoenixframework.org/)
* [React] (https://facebook.github.io/react/)
* [Relay](https://facebook.github.io/relay/)
* [GraphQL](https://github.com/facebook/graphql)
* [RethinkDB](https://www.rethinkdb.com/)
* [Webpack](https://webpack.github.io/)
  * Hot module reload
* [Immutable.js](https://facebook.github.io/immutable-js/)
* [Flow](http://flowtype.org/)
* [Eslint](http://eslint.org/)
* [Jest](https://facebook.github.io/jest/)
* [Docker](https://www.docker.com/)

### Example app
Phoenix hipster stack comes with an example app.

The app is a port of the node.js app built in the [Building Data-driven React Applications with Relay, GraphQL, and Flux](http://app.pluralsight.com/courses/react-apps-with-relay-graphql-flux) course from Pluralsight.
The app is running on a 512mb single core droplet on digitalocean.

*More instressed in Elm ?* Check out [elm-hipster-stack](https://github.com/carleryd/elm-hipster-stack)

### Getting Started

Clone this repo then:

1. Install dependencies with `mix deps.get && npm i`
2. Start rethinkDB `rethinkdb`
3. Start Phoenix endpoint with `mix phoenix.server`
4. Create database by going to `localhost:4000/reset`
5. Visit `localhost:4000/graphql` to test the amazing graphiql interface
6. Query the database
  ```
  query myQuery{
    store{
      authors {
        id
        name
      }
    }
  }
  
  ```
7. Visit `localhost:4000` for a basic relay app using the data.

**Jest is not implemented. Feel free to contribute :)**

## DOCKER 
1. `docker-compose build`
2. `docker-compose up`
3. `visit localhost:4001/reset`
4. `visit localhost:4001`

## Make your own project
1. `git clone git@github.com:graphql-elixir/phoenix-hipster-stack.git <name-of-your-project>`
2. `cd <name-of-your-project> rm -rf .git`
3. `git init`
4. `git remote add orgin <your-new-repo>`
5. `git push -u orgin master`

When changeing the graphql schemas run 
`mix CreateSchema` to make a new `schema.json`. 
This `schema.json` is used by Relay.


## Running in production.
```
MyAwesomePrompt> MIX_ENV=prod mix compile
MyAwesomePrompt> MIX_ENV=prod mix phoenix.digest
MyAwesomePrompt> MIX_ENV=prod PORT=4000 mix phoenix.server
```


###Used resourses
* [updated-phoenix-webpack-react-setup](http://mikker.github.io/2016/02/04/updated-phoenix-webpack-react-setup.html)
* GraphQL & RethinkDB
  * [GraphQL-Elixir](https://github.com/joshprice/graphql-elixir)
  * [plug_GraphQL](https://github.com/joshprice/plug_graphql)
  * [graphql-phoenix-rethinkdb] (https://github.com/AdamBrodzinski/graphql-phoenix-rethinkdb)
  * [phoenix-rethinkdb-example](https://github.com/AdamBrodzinski/phoenix-rethinkdb-example)

