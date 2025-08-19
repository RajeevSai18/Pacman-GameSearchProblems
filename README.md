# Pacman Game Search Problems & Spam Classifier

This repository contains a core project completed as part of an Artificial Intelligence work:

1. Pacman Multi-Agent Search – an interactive Pacman environment to experiment with AI agents.

# 📂 Project Structure

Pacman-GameSearchProblems/
│
├── pacman.py # Main entry point for running games
├── autograder.py # Autograder for grading assignments
├── game.py, util.py # Core game mechanics & utilities
├── multiAgents.py # Your implementations of ReflexAgent, Minimax, AlphaBeta, Expectimax
├── layouts/ # Pacman board layouts
├── Spam-Classifier/ # Separate ML project
│ ├── q2_classifier.py # Naive Bayes classifier
│ ├── train, test # Training & test datasets
│ └── q2_output.csv # Sample output file
└── README.md # Project description

🎮 Pacman Multi-Agent Search

This project extends the UC Berkeley Pacman AI framework. The goal is to design agents that make decisions in the Pacman game world.

Features :

ReflexAgent – evaluates moves greedily based on immediate surroundings.

MinimaxAgent – implements adversarial search with a minimax algorithm.

AlphaBetaAgent – optimizes minimax with alpha–beta pruning.

ExpectimaxAgent – models uncertainty by assuming ghosts act stochastically.

KeyboardAgent – allows manual play.

Layouts :

Includes a variety of boards (smallClassic, mediumClassic, originalClassic, openClassic, contestClassic, etc.) to test different strategies.

Example Runs :

# Reflex agent

python pacman.py -l smallClassic -p ReflexAgent

# Minimax agent

python pacman.py -p MinimaxAgent -a depth=2 -l minimaxClassic

# Alpha-Beta agent

python pacman.py -p AlphaBetaAgent -a depth=3 -l contestClassic

# Manual play

python pacman.py -l mediumClassic -p KeyboardAgent

Autograder :

Run the autograder to test correctness:

# run all questions

python autograder.py

# run specific question

python autograder.py -q q1
