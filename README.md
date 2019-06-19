# 2
limit = int(input())

series = []

series.append(1)

series.append(2)

[series.append(series[k-1] + series[k-2]) for k in range(2 , limit)]

print(series)

print(sum(series[i] for i in range(1, len(series),2)))               
