Підготував:
Студент Толмачов Антон ІС-01.
Варіант 10.
Умова: 
Знайти всі файли в поточній директорії, імена яких не прописані в list.txt.

Код скрипта:
#!/bin/bash
file="list.txt"
path=$(ls)
for var in $path
do
if !(grep -q "$var" list.txt)
then
echo "$var"
fi
done
