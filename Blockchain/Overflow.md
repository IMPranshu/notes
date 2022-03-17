for Ex- unit8 can store maximum 255.
if we store uint8 val = 255 + 1. it will show error 
but if we will typecast it and say uint8 val = 255 + uint8 (1) . val will be equal to 0.
then if we say uint8 val = 255 + uint8 (100). val will be equal to 99.
Here in the last 2 exaples the values wrap around .

if we are using version below 0.8 we have to make checks for our mathematical storing values. We can use [[Safemath]] to ensure this in version below 0.8.

