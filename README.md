# dm-interviews-07jul23

## Create a spring boot API application with the following:

1) Go to https://rapidapi.com/myapos--FqlEzvrlv/api/dog-breeds2/
2) Login via your gmail and get the API key
3) Implement the call to the API -> 'https://dog-breeds2.p.rapidapi.com/dog_breeds' with your API key based authentication [GET Get All Dog Breeds]
4) Use https://resilience4j.readme.io/docs/retry and implement a RETRY pattern on the above API
4) Parse the response for id, breed, origin, url and store the same locally in your DB of choice with the same column names
5) Introduce the following end-point /v1/dogBreed in your application with one query parameter called 'breed' 
6) Implement a GET operation on the same which first checks if the breed already exists in your DB and if not, then it must make a call to url: 'https://dog-breeds2.p.rapidapi.com/dog_breeds/breed [GET Get Breed Information] and get the breed data and update the local DB.
7) If not found, then throw a 404 saying breed not found
8) Setup postman collection of the end point /v1/dogBreed
9) Commit your code to a new branch in the same github or upload to google-drive (https://drive.google.com/drive/folders/1kYCf86FU02xdtRK5oUTpEzc0lU_kjvKk?usp=sharing)
