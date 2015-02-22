# boggle-solver
A trie + dynamic programming solution to the Boggle game

The dictionary is stored in a trie (prefix tree). A DFS like traversal is done on the dictionary to find the words. For each word, we use a dynamic programming technique to figure out whether the board contains the word or not.

The runtime of the algorithm is O(Dictionary size * Board dimension * Board dimension * Max word length in dictionary).

On my ~3GHz iMac, it takes 1.8 seconds to run on a dictionary of size ~175K words.

I ran the same dynamic programming algo with C++ code (Described here: http://exceptional-code.blogspot.com/2012/02/solving-boggle-game-recursion-prefix.html) that took much shorter time than this. The C++ approach though used a list instead of a trie to store the dictionary words.
