# ChessLife: A JavaScript Chess Engine

## Introduction

ChessLife is a chess engine and AI move finder written in JavaScript, based on the Negamax algorithm. It demonstrates strong performance, outperforming Stockfish Level 6 on Lichess. Its estimated Elo rating ranges from 1800 to 2000, depending on the thinking time allocated.

## Features

ChessLife offers a range of features that contribute to its performance:

- **Negamax Algorithm with Alpha-Beta Pruning:** The engine employs the Negamax algorithm for move searching, enhanced with alpha-beta pruning for more efficient search.
- **Move Ordering with MVV-LVA Heuristic:** ChessLife utilizes the Most Valuable Victim - Least Valuable Aggressor (MVV-LVA) heuristic to improve move ordering and increase pruning efficiency.
- **Principal Variation Search:** The engine uses the Principal Variation (PV) line to prioritize moves that are part of the PV, reducing the search space.
- **Quiescence Search:** ChessLife employs quiescence search to handle the horizon effect by extending search into capturing sequences.
- **Iterative Deepening:** The engine uses iterative deepening to explore deeper levels of the search tree gradually.
- **Piece-Square Tables:** ChessLife incorporates piece-square tables to evaluate the positional strength of pieces on specific squares.
- **Tapered Evaluation:** The evaluation function uses tapering to dynamically adjust material imbalances based on game phases.

## Changelogs

- **1.1:** Improved evaluation function from [Simplified Eval](https://www.chessprogramming.org/Simplified_Evaluation_Function) to [PeSTO's Eval Function](https://www.chessprogramming.org/PeSTO%27s_Evaluation_Function), resulting in significant improvements (~200 Elo).

## Credits

ChessLife wouldn't be possible without the contributions and inspiration from various sources:

- [Chess Engines: A Zero to One](https://www.chessengines.org/): A motivating article that kickstarted the journey into chess programming.
- [Bluefever Software's YouTube series](https://www.youtube.com/watch?v=2eA0bD3wV3Q&list=PLZ1QII7yudbe4gz2gh9BCI6VDA-xafLog): An invaluable 63-part series on chess programming that inspired much of the engine.
- [Chess Programming Wiki](https://www.chessprogramming.org/Main_Page): A valuable resource for chess programming.
- [CM Chessboard](https://github.com/shaack/cm-chessboard): The GUI library used for the engine.

## License

This project is licensed under the [MIT License](LICENSE).

Feel free to contribute, use, and enhance this chess engine as you see fit. Enjoy exploring the world of chess programming!

