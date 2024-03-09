1. sudo docker compose up -d
2. in new terminal $go run producer/producer.go    
3. in new terminal $go run worker/worker.go    

4. in new terminal
curl --location --request POST '0.0.0.0:3000/api/v1/comments' \
--header 'Content-Type: application/json' \
--data-raw '{ "text":"chocolate barrs" }'