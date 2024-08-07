# F5 Distributed Cloud: API Discovery & Protection

Catatan f5-academy-class-4 https://clouddocs.f5.com/training/community/f5xc/html/class4/class4.html

## Lab-1 

### Task-1: Traffic Generator

```
while true; do 
  for breed in Persian Siamese Rusian Blue; do 
    curl http://__YOUR_NAMESPACE__.lab-sec.f5demos.com/api/CatLookup/GetByBreed?breed=$breed; 
    sleep 1; 
  done; 
done
```

### Task-4: Generate More API Violations

```
while true; do 
  sleep 10; 
  curl http://__YOUR_NAMESPACE__.lab-sec.f5demos.com/api/CatLookup/GetByAge?age=five; 
done
```
## Lab-2 

### Task-1: API Protection Rules

```
while true; do 
  sleep 3; 
  curl http://__YOUR_NAMESPACE__.lab-sec.f5demos.com/api/CatLookup/GetAllCats; 
done
```

### Task-2: API Rate Limiting

```
while true; do
  for i in $(seq 5); do
    curl http://__YOUR_NAMESPACE__.lab-sec.f5demos.com/api/DogLookup/GetAllDogs -v; 
  done; 
  sleep 1m; 
done
```
