# railRant
A platform where you can rant about trains being late and other IR problems in your favorite language, and join million others (sorry, this broke dev doesn't have enough infra to handle millions, but you can understand the sarcasm), and let the railway officials know everything, without becoming a keyboard warrior or account tag master on twitter.
## Note
*DONE WHILE SITTING IN AN ACTUAL TRAIN
Idea is mine, architecture is mine, implementation is done by AI (yk, time constraints and laziness)
## Architecture
![System architecture](./docs/arc.png)
## Tech stack
Golang (net/http) for audio ingestor, history service
FastAPI for renderer service (easy to implement LOL)
Python worker (with gnan AI stuff) for inference worker
PostgreSQL (through neon) for database
Redis cloud for cache
NextJS for frontend (and some random js libs for maps and stuff, pls ask gemini, i am not a frontend dev)
Amazon S3 for object store
Amazon SQS for message queue


