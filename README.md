# shells
shell 脚本集合

求平均值：
cat a  |awk '{sum+=$1} END {print "Average = ", sum/NR}'

求最大值：
cat data|awk 'BEGIN {max = 0} {if ($1+0>max+0) max=$1 fi} END {print "Max=", max}'
awk 'BEGIN {min = 1999999} {if ($1<min) min=$1 fi} END {print "Min=", min}'


求和：
cat data|awk '{sum+=$1} END {print "Sum = ", sum}'
