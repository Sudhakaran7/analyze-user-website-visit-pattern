You are given three arrays username, timestamp and website of the same length N where the ith tuple means that the user 
with name username[i] visited the website website[i] at time timestamp[i].
A 3-sequence is a list of not necessarily different websites of length 3 sorted in ascending order by the time of their visits.
Find the 3-sequence visited at least once by the largest number of users. If there is more than one solution, return the lexicographically minimum solution.
A 3-sequence X is lexicographically smaller than a 3-sequence Y if X[0] < Y[0] or X[0] == Y[0] and (X[1] < Y[1] or X[1] == Y[1] and X[2] < Y[2]). 
It is guaranteed that there is at least one user who visited at least 3 websites. No user visits two websites at the same time.

Input Description:
First line contains N. (1<N<100)
Second line contains N elements as string in username[].
Third line contains N timestamps as integers in timestamp[].
Third line contains N elements as string in website[].

Output Decription:
Print the 3-sequence visited at least once by the largest number of users

Sample Input:
10
joe joe joe mary mary mary mary john john john
1 2 3 4 5 6 7 8 9 10
home about career home cart maps home home about career

Sample Output:
home about career

Explanation:
The most three websites home about career which is in the given websites array.

Sample Input:
8
john joe john joe mary mary mary john
1 2 3 4 5 6 7 8
cart cart home contact cotact home cart home

Sample Output:
cart home home

Sample Input:
11
a b c d e f g h i j k
1 2 3 4 5 6 7 8 9 0 1
phone phone web web web contact contact phone home home home

Sample Output:
phone web home

Sample Input:
5
a b c d e
1 2 3 4 5
contact phone phone contact home

Sample Output:
contact phone home

Sample Input:
6
as de rt yu jn hb op
2 3 4 5 6 7
home phone phone contact contact phone

Sample Output:
home phone contact

Sample Input:
7
asz dfr tyh gkj cvb poiuty qwerty
1 2 3 4 5 6 7
phone contact contact phone phone home home

Sample Output:
phone contact home
