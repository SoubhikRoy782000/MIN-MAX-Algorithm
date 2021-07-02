# MIN-MAX-Algorithm

Aim -

To find the optimal value of a given tree of integer values in the most optimal way possible under the time complexity O(n+m) = O(N).

Algorithm –

STEP 1 – Start traversing the given tree in top to bottom manner.

STEP 2 – If node is a leaf node then return the value of the node.

STEP 3 – If isMaximizingPlayer exist then bestVal = -INFINITY

STEP 4 – For each child node, value = minimax(node, depth+1, false, alpha, beta)

STEP 5 – bestVal = max( bestVal, value) and alpha = max( alpha, bestVal)

STEP 6 – If beta <= alpha then stop traversing and return bestVal

STEP 7 – Else, bestVal = +INFINITY

STEP 8 – For each child node, value = minimax(node, depth+1, true, alpha, beta)

STEP 9 – bestVal = min( bestVal, value) and beta = min( beta, bestVal)

STEP 10 – if beta <= alpha the stop traversing and return bestVal.
