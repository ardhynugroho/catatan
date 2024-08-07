# Catatan f5-academy-class-4

## Lab-1 Task-1: Traffic Generator

```
while true; do 
  for breed in Persian Siamese Rusian Blue; do 
    curl http://cute-walrus.lab-sec.f5demos.com/api/CatLookup/GetByBreed?breed=$breed; 
    sleep 1; 
  done; 
done
```

## Lab-1 Task-4: Generate More API Violations

```
while true; do 
  sleep 10; 
  curl http://_YOUR_NAMESPACE_.lab-sec.f5demos.com/api/CatLookup/GetByAge?age=five; 
done
```
