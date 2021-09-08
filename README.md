# Blockchess: Game of Chess on blockchain

## Summary
Blockchess is a crypto-powered server for playing Chess (in p2p mode).

The service will be hosted on [Polygon Network](https://polygon.technology/) where gas fee make such projects possible.

The crypto component of the service is responsible for:
 * Tracking players, games, and results;
 * Checking the game rules;
 * Calculating and keeping track of players ratings;
 * Matching players with similar ratings;
 * Issuing a token somehow tight with players' ratings; the core idea is that to play with stronger players you will need (stake?) comparable amounts of tokens.

The Web3 component (website) of the service is responsible for:
 * Providing slick and modern UI for all the features;
 * Integrating with browser wallets.

## Dependencies

### Original  Paul Grau's effort
I am aware that Paul Grau already (successfully, I assume) tried to build something like this back in 2016.
And I think I will be reusing some of the Solidity code Paul authored; the license allows it.
I will try to re-evaluate some of his assumptions (e.g. check-mate cannot be proved on the blockchain)
but I suspect that the focus on the project will be shifted from proving that chess can be played on the chain
to a new tokenomics model around rating systems and players matching.

More info:
 * https://medium.com/@graycoding/lessons-learned-from-making-a-chess-game-for-ethereum-6917c01178b6
 * https://github.com/ise-ethereum/on-chain-chess

### Chess UI/UX
The project will probably use some existing Chess UI library, e.g. [Chessground](https://github.com/ornicar/chessground).