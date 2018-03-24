### E 1
a => O(n)
b => O(log n)
c => O(log n)
d => O(n log n)
e => O(n^3)
f => O(n)
g => O(n)

### E 2
a => 

maxSubtraction(a, i = 0; j = a.length)
{
    let maxSub = 0;
    while(j >= i)
    {
        let sub = a[j]-a[i];
        if (sub > maxSub){
            maxSub = sub;
            j--;
            i++;
        }
        
    }
    return maxSub;
}

## E 3
a => O(n^2) - O(n log n) => iterates over each item (x) in array and adds to sort.
b => O(n log n) 