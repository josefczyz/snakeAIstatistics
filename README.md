# snakeAIstatistics
Repo for files generated by SnakeAI project. Demonstration of a learning ability of a neural network (NN) using a genetic algorithm.

Project SnakeAI was orginaly developed by Greer Viau https://github.com/greerviau/SnakeAI
and extended for automatization of learning process and trained NN configurations savings by Josef Czyz. https://github.com/josefczyz/SnakeAI

Folders Snakes and BestSnakes contains configurations of trained NN for specific topology.
Snakes500, Snakes2000 and Snakes4000 - the numbers represent how many snakes were generated in each generation.
Csv filename with configuration of trained NN nomenclature:
T**H**x**N**m**M**G**G**R**R**bestSnake.csv

where these values set the NN topology for snake replay in the new condition:

**H** is number of hidden layers

**N** is number of neurons in layer

To replay trained snake:
1.  setup NN topology:

SnakeAI.pde

int hidden_nodes = N;

int hidden_layers = H;

2. in case you are using orginal Greer Viau SnakeAI project skip to step 4.

3. set snake visibility and brain (brain will slow down replay)

boolean showAnimation = true;

boolean brainShow = true;

4. run SnakeAI.pde

5. click Load button and select csv file with snake brain configuration. e.g. T2x16m5G50R1bestSnake.csv

Values used for the genetic algorithm during the training phase. They have no impact on playback

M is % of mutation

G is number of trained generation in each evolution

R represents in each evolution has been snake trained
