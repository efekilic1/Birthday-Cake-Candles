# Birthday-Cake-Candles
You are in charge of the cake for a child's birthday. You have decided the cake will have one candle for each year of their total age. They will only be able to blow out the tallest of the candles. Count how many candles are tallest.




<img width="994" alt="Ekran Resmi 2022-05-20 13 59 03" src="https://user-images.githubusercontent.com/105243448/169515798-455b2d41-85ce-4bbe-9082-cc9a0df40c6e.png">



## Important Part

```
    public static int birthdayCakeCandles(List<int> candles)
    {
        candles.Sort();
        candles.Reverse();

        int num = candles[0];
        int cnt = 0;
        foreach (var candle in candles)
        {
            if (candle >= num)
            {
                cnt++;
            }
        }

        return cnt;


    }
```
