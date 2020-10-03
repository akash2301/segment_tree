# segment_tree
segment tree header file 
To construct a segment tree you need to specify the following:
1. The datatype of array for which the tree is being constructed.
2. an array or vector for which the tree is to be constructed.
3. a value that can be used to fill the extra nodes of the tree.
4. a function combine that specifies how the result of left and right child of a node
   should be used to generate the value of current node.

Example usage:
1.int small(int x,int y){return min(x,y);}
  SegmentTree < int > rangeMinQueries(dataVector,INT_MAX,small);
2.
int sum(int x,int y){return x+y;}
SegmentTree < int > rangeSumQueries(dataVector,0,sum);
3.
long long product(long long x,long long y){return x*y;}
SegmentTree < long long > rangeProductQueries(dataVector,1,product);
