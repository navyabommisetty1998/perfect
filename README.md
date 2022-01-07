# perfect
#!/bin/bash/
echo "enter the number:"
read n 
sum=0
i=1
while [ $i le $n ]
do
 if [[ (($n % i)) -eq  0 ]]
 then
 sum=$((sum + i))
 fi
  i=$(( i + 1 ))
  done
  if [ $n -eq $sum ]
  then
  echo "$n is a perfect number"
  else
  echo "$n is not a perfect number"
  fi
