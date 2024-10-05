# Dynamic arrays with more index space

Dynamic arrays already use `[]` to specify the size for each instance, but what if you want to specify the maximum
storage space? I was forced to add a comma:

```sql
type myDyArray extends integer array [200] //a normal dynamic array type of size 200
                                           //max 40 instances

type myDyArray extends integer array [200,40000] //an enhanced dynamic array type of size 200
                                                 //max 200 instances
```