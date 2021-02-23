# Laddered

Gaming ladder management system.

## Features

Here's a quick high-level list. More details to come

- Authentication & Authorisation (pretty standard stuff)
- Flexible hierarchical organisation stucture
- Team based ladders
  - ELO rankings
  - Disputes
  - Reporting & Metrics

### Autentication & Authorisation

All the usual things to expect to see, a built in sign-up and sign-in system with support for your proferred social platform.

### Flexible hierarchical organisation structure

We want to be able to supprt small teams and large professional organisations, so we are enabling you to use an org structure to suit your needs. The system will support nested groups, able to have members in all of them which have cascading permissions.

#### Example 1: a simple clan for a game

```
Team 
 └── Members
```
#### Example 2: a gaming community

```
Community
 ├── Members (probably community management)
 └── Team 
     └── Members
```

### Example 3: a large gaming org

```
Organisation
 ├── Members (exec / management)
 ├── Amature Division
 │   ├── Members (management)
 │   ├── Team 1 (Counter-Strike)
 │   │    └── Members
 │   └── Team 2 (Valorant)
 │        └── Members
 └── Pro Division
     ├── Members (management)
     ├── Team 1 (Counter-Strike)
     │    └── Members
     └── Team 2 (Valorant)
          └── Members
```


## Development

```bash
composer install
npm install
npm run watch
```

## Build

```bash
composer install
npm install
npm run prod
```
